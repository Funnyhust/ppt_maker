# Project Context & Handoff

## Cập nhật 24/07/2026 — Quy hoạch lại Tool Design

- Deck vẫn có 23 trang nhưng chỉ còn 4 nhóm dự án chính: KNX, Auto Test, Tool Design và MSB Office.
- Đã bỏ IoT Team khỏi danh mục dự án độc lập.
- Tool Design hiện bao gồm tool nguồn DC, loader Luto, tool test/tool loader Lumes V2 và tool test Smart Lighting.
- Trang 15, 16 và 18 lần lượt là `Tool Design — Loader sản xuất`, `Tool Design — Tool test nguồn Lumes V2` và `Tool Design — Tool test Smart Lighting`.
- Bản xuất mới nhất: `exports/review_nhan_su_t7_redesign_20260724_210106.pptx`.
- Postflight: `passed-with-warnings`, quality gate passed, 23 slides; SVG quality 23/23 passed, 0 lỗi.

## Cập nhật 24/07/2026 — KNX Partner

Phần cập nhật này thay thế số trang, bản xuất mới nhất và thứ tự trang ở các mục trạng thái/cấu trúc bên dưới:

- Deck hiện có 23 trang; trang 11 là `KNX Partner — Chứng chỉ & năng lực`, nằm ngay sau phần dự án KNX.
- Thành tích: KNX Partner No. 147063; hoàn thành KNX Basic ngày 31/05/2026, lý thuyết 88,5% và thực hành 96%.
- Bản xuất mới nhất: `exports/review_nhan_su_t7_redesign_20260724_204315.pptx`.
- Postflight: `passed-with-warnings`, quality gate passed, 23 slides; SVG quality 23/23 passed, 0 lỗi.
- Trang mới đã được kiểm tra trực quan từ SVG final nhúng ảnh tại `validation/knx_partner_certificate_preview.png`; chứng chỉ và bảng điểm hiển thị đúng, không crop và không chồng chữ.
- Từ trang Auto Test trở đi, số thứ tự cũ tăng thêm 1; trang kết là trang 23.

## 1. Mục tiêu

Tạo deck review nhân sự tháng 7 cho Nguyễn Văn Dương, tổng hợp công việc từ 20/03/2026 đến 22/07/2026. Deck giữ nhận diện LUMI và tinh thần của template cũ nhưng tái cấu trúc nội dung để dễ đọc, không chồng chữ và có nhiều nhóm nội dung hơn.

## 2. Trạng thái hiện tại

- Route: Generate PPTX, SVG → native DrawingML PPTX.
- Canvas: PPT 16:9, 1280 × 720.
- Số trang: 23.
- Font: Arial.
- Màu chính: LUMI green `#008C4F`, blue `#1456F0`, white `#FFFFFF`.
- Chế độ đọc: balanced.
- Cấu trúc PPTX: flat; chữ và shape được xuất thành đối tượng PowerPoint editable.
- Kiểm tra SVG: 23/23 trang passed, 0 lỗi; cảnh báo còn lại là advisory về group/bounds.
- Postflight PPTX: `passed-with-warnings`, quality gate passed, 23 slides.
- Bản mới nhất đã quy hoạch lại Tool Design: `exports/review_nhan_su_t7_redesign_20260724_210106.pptx`.
- Bản chính thức dùng chế độ `--no-merge` để giữ từng dòng chữ độc lập khi chuyển sang DrawingML.
- Bản 23 trang có chứng chỉ trước đó đã render đầy đủ bằng Microsoft PowerPoint tại `validation/pptx_render_20260724_204315/`; bản Tool Design hiện tại đã qua SVG quality gate và PPTX postflight.

## 3. Dữ liệu nguồn và số liệu khóa

Nguồn công việc chính là `sources/List_task.csv`. Deck sử dụng các số liệu:

- 114 task được ghi nhận.
- 102 task Done, tương đương 89,5%.
- 98 task thuộc KNX.
- 4 nhóm dự án chính: KNX, Auto Test, Tool Design và MSB. Loader Luto, tool test/tool loader Lumes V2 và tool test Smart Lighting được xếp dưới Tool Design.
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
- Screenshot giao diện quan trọng phải có trang bằng chứng riêng, chiếm khoảng 65–80% diện tích slide; không ép nhiều ảnh nhỏ vào một trang.
- Trang tổng hợp chỉ trình bày công việc/kết quả. Các trang 06–08, 10 và 13 là prototype ảnh lớn để áp dụng cho ảnh dự án bổ sung sau này.

## 5. Cấu trúc 23 trang

1. Bìa Review nhân sự — giữ template gốc, thêm ngày/giai đoạn review.
2. Nội dung — điện thoại và bốn ô số cắt góc của template cũ.
3. Danh mục 4 dự án chính và timeline 20/03–22/07.
4. KNX — tổng quan, thời gian, KPI và thành tích.
5. KNX — tổng hợp công việc chính và kết quả.
6–8. KNX Benchmark — ba screenshot lớn: bảng điều khiển, tạo test case và báo cáo.
9. KNX — kỹ năng, tư duy, bài học, khó khăn và KNX Basic.
10. KNX — screenshot lớn tool nạp code.
11. KNX Partner — chứng chỉ chính thức, Partner No. 147063, cấp ngày 31/05/2026; kết quả Passed với 88,5% lý thuyết và 96% thực hành.
12. Auto Test — review đầy đủ.
13. Tool Design — tổng quan các nhánh tool test và tool loader.
14. Tool Design — screenshot lớn giao diện vận hành.
15. Tool Design — loader sản xuất Luto và Lumes V2.
16. Tool Design — tool test nguồn Lumes V2.
17. MSB Office — review đầy đủ.
18. Tool Design — tool test Smart Lighting, ghi rõ Ongoing.
19. Sử dụng AI trong công việc.
20. Tự đánh giá ưu, nhược điểm.
21. Bài học và khó khăn xuyên dự án.
22. Mục tiêu sắp tới.
23. Cảm ơn — giữ nguyên template kết cũ.

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
