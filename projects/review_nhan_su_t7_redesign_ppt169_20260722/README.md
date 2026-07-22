# Review nhân sự T7 — Nguyễn Văn Dương

Project PPT Master có thể tiếp tục chỉnh sửa và build lại trên máy khác. Đây không chỉ là thư mục chứa file PPTX cuối: source, ảnh, SVG editable, notes, đặc tả thiết kế và bằng chứng validation đều được version cùng nhau.

## Bắt đầu nhanh

1. Đọc [`PROJECT_CONTEXT.md`](PROJECT_CONTEXT.md).
2. Chỉnh nội dung trong `svg_output/`, `notes/total.md`, `design_spec.md` hoặc `spec_lock.md` tùy phạm vi thay đổi.
3. Chạy validation và build theo các lệnh trong `PROJECT_CONTEXT.md`.

## File quan trọng

- `PROJECT_CONTEXT.md`: bối cảnh, quyết định thiết kế, cấu trúc slide và hướng dẫn handoff.
- `sources/List_task.csv`: danh sách task nguồn cho kỳ review.
- `sources/review_nhan_su_alignment_20260722_202409.pptx`: deck LUMI tham chiếu.
- `design_spec.md`: đặc tả nội dung và thiết kế 15 trang.
- `spec_lock.md`: các token và ràng buộc thực thi ổn định.
- `svg_output/`: nguồn slide editable.
- `notes/`: speaker notes tổng và từng trang.
- `images/`: ảnh làm việc được SVG sử dụng.
- `analysis/`: dữ liệu phân tích tự động từ source và ảnh.
- `confirm_ui/`: quyết định đã xác nhận trong giai đoạn Strategist.
- `validation/`: báo cáo kiểm tra SVG và PPTX.
- `exports/`: file PPTX đã xuất.

## Dữ liệu không version

`.preview/`, `.review/`, `backup/`, `live_preview/` và log runtime được tạo lại tự động. Chúng không phải nguồn chỉnh sửa và không cần khi chuyển máy.

> Project chứa dữ liệu review nhân sự và danh sách công việc nội bộ. Nên lưu trong repository private hoặc kiểm tra lại nội dung trước khi public.
