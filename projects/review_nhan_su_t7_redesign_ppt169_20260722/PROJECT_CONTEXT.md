# Project Context & Handoff

## 1. Mục tiêu

Tạo deck review nhân sự tháng 7 cho Nguyễn Văn Dương, tổng hợp công việc từ 20/03/2026 đến 22/07/2026. Deck giữ nhận diện LUMI và tinh thần của template cũ nhưng tái cấu trúc nội dung để dễ đọc, không chồng chữ và có nhiều nhóm nội dung hơn.

## 2. Trạng thái hiện tại

- Route: Generate PPTX, SVG → native DrawingML PPTX.
- Canvas: PPT 16:9, 1280 × 720.
- Số trang: 17.
- Font: Arial.
- Màu chính: LUMI green `#008C4F`, blue `#1456F0`, white `#FFFFFF`.
- Chế độ đọc: balanced.
- Cấu trúc PPTX: flat; chữ và shape được xuất thành đối tượng PowerPoint editable.
- Kiểm tra SVG: 17/17 trang passed, 0 lỗi; cảnh báo còn lại là advisory về group/bounds, không có lỗi tràn hoặc chồng chữ.
- Postflight PPTX: `passed-with-warnings`, quality gate passed, 17 slides. Cảnh báo thuộc nhóm cấu trúc SVG advisory.
- Bản review phong cách ảnh mới nhất: `exports/review_nhan_su_t7_redesign_20260724_202044.pptx`.
- Bản chính thức dùng chế độ `--no-merge` để giữ từng dòng chữ độc lập khi chuyển sang DrawingML.
- Đã render lại toàn bộ 17 trang bằng chính Microsoft PowerPoint tại `validation/pptx_render_20260724_202044/`; ảnh được nhúng đúng, không phát hiện chồng chữ hoặc lệch khung.

## 3. Dữ liệu nguồn và số liệu khóa

Nguồn công việc chính là `sources/List_task.csv`. Deck sử dụng các số liệu:

- 114 task được ghi nhận.
- 102 task Done, tương đương 89,5%.
- 98 task thuộc KNX.
- 7 nhóm dự án: KNX, Auto Test, Tool Design, IoT, LumesV2, MSB và Smart Lighting.
- Trạng thái còn lại tại 22/07: 5 Ongoing, 4 Not yet started, 2 Late, 1 Closed.

Deck LUMI tham chiếu nằm tại `sources/review_nhan_su_alignment_20260722_202409.pptx`. Các ảnh đã tách và chuẩn hóa nằm trong `images/`; không cần tách lại khi chỉnh slide thông thường.

## 4. Quyết định thiết kế đã chốt

- Giữ nguyên bố cục bìa xanh và trang kết xanh của template cũ; bìa chỉ bổ sung ngày review và giai đoạn review.
- Mục lục giữ đúng bốn phần của template cũ trên một trang.
- Trang mục lục giữ điện thoại bên trái và khôi phục ô số cắt góc, connector, hatch chéo giống mẫu gốc.
- Mỗi dự án có thời gian bắt đầu/kết thúc hoặc trạng thái đang triển khai.
- Mỗi dự án trình bày theo cùng hệ 2×3: công việc chính, kết quả, kỹ năng, tư duy, bài học & khó khăn, thành tích nổi bật.
- Không dùng bảng chữ dày; thay bằng KPI card, timeline, flow, capability map và roadmap.
- Tiêu đề ưu tiên một dòng; nội dung dài phải chia card hoặc tách trang, không giảm chữ xuống mức khó đọc.
- Chỉ sử dụng ảnh có sẵn trong source; không dùng ảnh AI hoặc ảnh web.
- Ảnh giao diện/chứng nhận được trình bày như bằng chứng công việc: luôn `no-crop`, đặt trong khung trung tính viền xanh và có chú thích ngắn.
- Với nhiều ảnh cùng một luồng dùng dải bằng chứng đánh số; với một đến hai ảnh dùng panel/cột bằng chứng. Trang 5, 6 và 8 là các prototype đã chốt để mở rộng cho ảnh dự án về sau.

## 5. Cấu trúc 17 trang

1. Bìa Review nhân sự — giữ template gốc, thêm ngày/giai đoạn review.
2. Nội dung — điện thoại và bốn ô số cắt góc của template cũ.
3. Danh mục 7 dự án và timeline 20/03–22/07.
4. KNX — tổng quan, thời gian, KPI và thành tích.
5. KNX — công việc chính, kết quả và dải ba ảnh benchmark.
6. KNX — kỹ năng, tư duy, bài học, khó khăn; cột bằng chứng tool nạp code và kết quả KNX Basic.
7. Auto Test — review đầy đủ theo lưới 2×3.
8. Tool Design — review 2×2 và panel ảnh giao diện tool lớn.
9. IoT — review đầy đủ theo lưới 2×3.
10. LumesV2 — review đầy đủ theo lưới 2×3.
11. MSB Office — review đầy đủ theo lưới 2×3.
12. Smart Lighting — review đầy đủ, ghi rõ Ongoing.
13. Sử dụng AI trong công việc.
14. Tự đánh giá ưu, nhược điểm.
15. Bài học và khó khăn xuyên dự án.
16. Mục tiêu sắp tới.
17. Cảm ơn — giữ nguyên template kết cũ.

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
python skills/ppt-master/scripts/svg_to_pptx.py projects/review_nhan_su_t7_redesign_ppt169_20260722 --no-merge
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
- Các báo cáo trong `validation/` và toàn bộ `exports/`.

Không version vì có thể tái tạo:

- `.preview/`, `.review/`, `backup/`, `live_preview/`.
- Ảnh render PowerPoint tạm trong `validation/pptx_render_*/` và preview tổng hợp trong `validation/final_preview_project/`.
- Runtime locks, server logs và Python caches.

## 10. Lưu ý bảo mật

Project có tên nhân sự, danh sách task và thông tin công việc nội bộ. Repository nên để private. Nếu bắt buộc public, cần rà soát và ẩn danh source trước khi push.
