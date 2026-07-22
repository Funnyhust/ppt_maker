# Project Context & Handoff

## 1. Mục tiêu

Tạo deck review nhân sự tháng 7 cho Nguyễn Văn Dương, tổng hợp công việc từ 20/03/2026 đến 22/07/2026. Deck giữ nhận diện LUMI và tinh thần của template cũ nhưng tái cấu trúc nội dung để dễ đọc, không chồng chữ và có nhiều nhóm nội dung hơn.

## 2. Trạng thái hiện tại

- Route: Generate PPTX, SVG → native DrawingML PPTX.
- Canvas: PPT 16:9, 1280 × 720.
- Số trang: 15.
- Font: Arial.
- Màu chính: LUMI green `#008C4F`, blue `#1456F0`, white `#FFFFFF`.
- Chế độ đọc: balanced.
- Cấu trúc PPTX: flat; chữ và shape được xuất thành đối tượng PowerPoint editable.
- Kiểm tra SVG: 15/15 trang passed, 0 lỗi, 0 cảnh báo.
- Postflight PPTX: passed, 15 slides, 0 warning categories.
- Bản xuất hiện tại: `exports/review_nhan_su_t7_redesign_20260722_215349.pptx`.

## 3. Dữ liệu nguồn và số liệu khóa

Nguồn công việc chính là `sources/List_task.csv`. Deck sử dụng các số liệu:

- 114 task được ghi nhận.
- 102 task Done, tương đương 89,5%.
- 98 task thuộc KNX.
- 7 nhóm dự án: KNX, Auto Test, Tool Design, IoT, LumesV2, MSB và Smart Lighting.
- Trạng thái còn lại tại 22/07: 5 Ongoing, 4 Not yet started, 2 Late, 1 Closed.

Deck LUMI tham chiếu nằm tại `sources/review_nhan_su_alignment_20260722_202409.pptx`. Các ảnh đã tách và chuẩn hóa nằm trong `images/`; không cần tách lại khi chỉnh slide thông thường.

## 4. Quyết định thiết kế đã chốt

- Giữ logo, màu sắc, ảnh sản phẩm và phong cách LUMI.
- Mục lục được tách thành hai trang để trình bày đủ 7 nhóm nội dung mà không nhồi chữ.
- Trang mục lục giữ khung điện thoại bên trái và nhãn số dạng connector giống template mẫu.
- Không dùng bảng chữ dày; thay bằng KPI card, timeline, flow, capability map và roadmap.
- Tiêu đề ưu tiên một dòng; nội dung dài phải chia card hoặc tách trang, không giảm chữ xuống mức khó đọc.
- Chỉ sử dụng ảnh có sẵn trong source; không dùng ảnh AI hoặc ảnh web.

## 5. Cấu trúc 15 trang

1. Review nhân sự tháng 7.
2. Nội dung 1/2: tổng quan và ba nhóm KNX.
3. Nội dung 2/2: đào tạo, dự án khác, năng lực và bước tiếp theo.
4. Kết quả nổi bật.
5. Hành trình 20/03–22/07.
6. Thiết bị và firmware KNX.
7. Tool, Jig và code loader.
8. Benchmark và kiểm thử hệ thống.
9. Đào tạo KNX.
10. Tài liệu và khả năng bàn giao.
11. Auto Test và Tool Design.
12. Các dự án và tool khác.
13. Năng lực được củng cố.
14. Trọng tâm tiếp theo.
15. Kết luận.

Chi tiết nội dung, ảnh và layout từng trang nằm trong `design_spec.md` mục IX. Các token bắt buộc cho Executor nằm trong `spec_lock.md`.

## 6. Quy tắc chỉnh sửa

- Chỉnh slide trực tiếp tại `svg_output/*.svg`.
- Giữ `viewBox="0 0 1280 720"` và các `data-pptx-bounds` của root group.
- Dùng raw Unicode cho tiếng Việt; escape ký tự XML như `&amp;`.
- Không dùng `foreignObject`, CSS external, `<style>`, mask hoặc script.
- Khi thay ảnh, đặt ảnh mới trong `images/`, cập nhật `design_spec.md` phần VIII và `spec_lock.md` phần images nếu đó là tài nguyên lặp lại.
- Khi thay nội dung/chiến lược lớn, cập nhật `design_spec.md` trước rồi mới sửa SVG.
- `svg_output/` là nguồn editable; `svg_final/` và `exports/` là đầu ra có thể tái tạo.

## 7. Kiểm tra và build lại

Chạy từ root của repo:

```powershell
python skills/ppt-master/scripts/project_manager.py validate projects/review_nhan_su_t7_redesign_ppt169_20260722
python skills/ppt-master/scripts/svg_quality_checker.py projects/review_nhan_su_t7_redesign_ppt169_20260722 --json
python skills/ppt-master/scripts/total_md_split.py projects/review_nhan_su_t7_redesign_ppt169_20260722
python skills/ppt-master/scripts/finalize_svg.py projects/review_nhan_su_t7_redesign_ppt169_20260722
python skills/ppt-master/scripts/svg_to_pptx.py projects/review_nhan_su_t7_redesign_ppt169_20260722
```

Để xem và chỉnh trực quan:

```powershell
python skills/ppt-master/scripts/svg_editor/server.py projects/review_nhan_su_t7_redesign_ppt169_20260722 --live --daemon
```

Để render ảnh kiểm tra từng trang, cần Playwright và Chromium:

```powershell
python -m pip install playwright
python -m playwright install chromium
python skills/ppt-master/scripts/visual_review.py projects/review_nhan_su_t7_redesign_ppt169_20260722
```

## 8. Handoff sang máy khác

Sau khi clone repo:

1. Cài dependency từ `requirements.txt` của repo.
2. Đọc file này, `design_spec.md` và `spec_lock.md`.
3. Chạy `project_manager.py validate` để kiểm tra project đầy đủ.
4. Khởi động live preview hoặc sửa SVG trực tiếp.
5. Chạy chuỗi build ở mục 7 để xuất PPTX mới.

Để không tải toàn bộ thư mục `examples/` nặng hàng trăm MB, có thể clone theo chế độ sparse:

```powershell
git clone --filter=blob:none --sparse <YOUR_REPOSITORY_URL> ppt-master
cd ppt-master
git sparse-checkout set skills docs projects/review_nhan_su_t7_redesign_ppt169_20260722
```

Git vẫn lấy các file ở root như `AGENTS.md`, `requirements.txt` và `.gitignore`, nhưng không checkout kho ví dụ lớn. Khi cần examples, chạy `git sparse-checkout add examples`.

Prompt tiếp tục gợi ý:

```text
Đọc AGENTS.md và skills/ppt-master/SKILL.md, sau đó tiếp tục chỉnh project projects/review_nhan_su_t7_redesign_ppt169_20260722. Đọc PROJECT_CONTEXT.md, design_spec.md và spec_lock.md trước khi sửa. Giữ nhận diện LUMI và chạy validation đầy đủ sau thay đổi.
```

## 9. Phạm vi Git

Được version:

- `sources/`, `analysis/`, `images/`, `icons/`, `templates/`.
- `design_spec.md`, `spec_lock.md`, `PROJECT_CONTEXT.md`.
- `svg_output/`, `svg_final/`, `notes/`.
- `confirm_ui/recommendations.json`, `confirm_ui/result.json`.
- `validation/`, `exports/`.

Không version vì có thể tái tạo:

- `.preview/`, `.review/`, `backup/`, `live_preview/`.
- Runtime locks, server logs và Python caches.

## 10. Lưu ý bảo mật

Project có tên nhân sự, danh sách task và thông tin công việc nội bộ. Repository nên để private. Nếu bắt buộc public, cần rà soát và ẩn danh source trước khi push.
