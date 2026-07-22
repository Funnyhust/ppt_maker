<!-- ppt-master-schema: design-spec/v1 -->
# Review nhân sự T7 - Design Spec

## I. Project Information

| Item | Value |
| --- | --- |
| Project Name | Review nhân sự T7 — Nguyễn Văn Dương |
| Canvas Format | PPT 16:9, 1280 × 720 px |
| Page Count | 15 |
| Target Audience | Quản lý trực tiếp, quản lý kỹ thuật và HR tham gia kỳ review nhân sự tháng 7. |
| Communication Intent | Báo cáo kết quả từ 20/03 đến 22/07, làm rõ phạm vi đóng góp và năng lực đã phát triển, sau đó thống nhất trọng tâm giai đoạn tiếp theo. |
| Desired Audience Outcome | Người xem nhanh chóng nắm được quy mô công việc, kết quả theo từng nhóm dự án, giá trị đóng góp và các ưu tiên tiếp theo. |
| Core Message / Ask / Action | Khối lượng công việc lớn đã được hoàn thành với trọng tâm KNX, đồng thời mở rộng sang Auto Test, Tool Design, IoT, MSB và Smart Lighting. |
| Delivery Context | Trình bày trực tiếp trong buổi review khoảng 15–20 phút; deck cũng cần tự đọc được khi gửi lại sau cuộc họp. |
| Artifact Afterlife | Tài liệu lưu hồ sơ review nhân sự và làm mốc đối chiếu cho kỳ review tiếp theo. |
| Reading Mode | balanced |
| Content Strategy | Được phép tái cấu trúc và mở rộng số trang, nhưng phải giữ đúng dữ liệu nguồn, nhận diện LUMI và tinh thần của trang mục lục mẫu. |
| Design Style | LUMI refined: swiss-minimal, nhiều khoảng trắng, phân cấp mạnh, số liệu và ảnh bằng chứng nổi bật. |
| Formula Policy | text-only |
| AI Image Acquisition Path | not applicable |
| Generation Mode | continuous |
| Spec Refinement | disabled |
| Created Date | 2026-07-22 |

## II. Canvas Specification

| Property | Value |
| --- | --- |
| Format | PPT 16:9 |
| Dimensions | 1280 × 720 |
| viewBox | `0 0 1280 720` |
| Margins | 56 px trái/phải; 46 px trên; 34 px dưới |
| Content Area | x=56–1224, y=46–676 |

## III. Visual Theme

### Theme Style

- **Mode**: briefing
- **Visual style**: swiss-minimal
- **Theme**: LUMI refined — giữ logo, màu xanh LUMI và ngôn ngữ điện thoại/nhãn số của mẫu; tái cấu trúc thành hệ thống module gọn.
- **Tone**: Tin cậy, kỹ thuật, sáng sủa, có bằng chứng nhưng không nặng báo cáo bảng biểu.

### Color Scheme

| Role | HEX | Purpose |
| --- | --- | --- |
| Background | #FFFFFF | Nền chính |
| Secondary background | #F4F7F5 | Card, vùng phân nhóm |
| Primary | #008C4F | Tiêu đề, số mục, điểm nhấn LUMI |
| Accent | #1456F0 | Trạng thái, mốc dữ liệu phụ |
| Secondary accent | #79C6A3 | Đường nối, nhãn nhẹ, vùng phụ |
| Body text | #1F2329 | Nội dung chính |

## IV. Typography System

### Font Plan

| Role | Chinese | English | Fallback tail |
| --- | --- | --- | --- |
| Title | Arial | Arial | sans-serif |
| Body | Arial | Arial | sans-serif |

- **Title stack**: Arial, sans-serif
- **Body stack**: Arial, sans-serif
- **Role rationale**: Arial giữ đúng template LUMI, hỗ trợ tiếng Việt ổn định và giảm sai lệch khi mở trên Windows/PowerPoint.

### Font Size Hierarchy

| Purpose | Anchor Size (px) |
| --- | ---: |
| Body | 24 |
| Title | 42 |
| Subtitle | 32 |
| Annotation | 18 |
| Compact body | 21 |
| Eyebrow | 15 |
| Footer | 14 |
| TOC item | 29 |
| TOC item compact | 27 |
| KPI number | 54 |

## V. Layout Principles

### Page Structure

- **Header area**: Logo LUMI ở góc trái, tiêu đề một dòng bắt đầu quanh x=360 hoặc x=430; không cho tự xuống dòng.
- **Content area**: Lưới 12 cột; tối đa 3 khối thông tin chính/trang; nội dung dài tách trang thay vì thu chữ.
- **Footer area**: Chỉ dùng số trang và đường mảnh xám; không đặt nội dung quan trọng dưới y=665.

### Spacing Specification

| Element | Current Project |
| --- | --- |
| Safe margin | 56 px |
| Content block gap | 24–32 px |
| Icon-text gap | 12–16 px |

## VI. Icon Usage Specification

- **Primary bundled library**: tabler-outline

| Purpose | Icon Path | Page |
| --- | --- | --- |
| Trạng thái hoàn thành | tabler-outline/circle-check | P04, P14 |
| Firmware và mã nguồn | tabler-outline/code | P06 |
| Tool và Jig | tabler-outline/tool | P07, P11 |
| Kiểm thử | tabler-outline/test-pipe | P08 |
| Đào tạo | tabler-outline/school | P09, P10 |

## VIII. Image Resource List

| Filename | Dimensions | Ratio | Purpose | Type | Layout pattern | Crop Policy | Acquire Via | Status | Reference | text_policy | page_role |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| image_8fa7a601c29ca778.png | 262×76 | 3.45 | Logo LUMI lặp lại | PNG | brand-header | no-crop | user | Sourced | Deck nguồn | no embedded text | brand |
| image_b3ef018bf0b10f2b.png | 1143×1143 | 1.00 | Họa tiết vòng tròn trang bìa/kết | PNG | hero-accent | no-crop | user | Sourced | Deck nguồn | no embedded text | atmosphere |
| image_010fcf8f9f909b91.png | 465×926 | 0.50 | Khung điện thoại trang mục lục | PNG | portrait-left | no-crop | user | Sourced | Deck nguồn | no embedded text | hero |
| image_3db7369d2c1e7d49.jpg | 1372×784 | 1.75 | Thiết bị KNX | JPG | right-evidence | no-crop | user | Sourced | Deck nguồn | no embedded text | evidence |
| image_6519313ef59a5f53.png | 1111×619 | 1.79 | Sơ đồ hệ thống KNX | PNG | wide-diagram | no-crop | user | Sourced | Deck nguồn | preserve legibility | evidence |
| image_bc82a45d35f49412.jpg | 960×540 | 1.78 | Jig/tool kiểm thử | JPG | right-evidence | adaptive | user | Sourced | Deck nguồn | no embedded text | evidence |
| image_9f31c49d5ae33b66.jpg | 422×714 | 0.59 | Jig Auto Test | JPG | portrait-right | adaptive | user | Sourced | Deck nguồn | no embedded text | evidence |
| image_5a1205fbd766d78e.png | 291×625 | 0.47 | UI ứng dụng LUMI | PNG | portrait-right | no-crop | user | Sourced | Deck nguồn | preserve UI text | evidence |
| image_deea19358d7d9df9.jpg | 1024×906 | 1.13 | Công tắc cơ LUMI | JPG | right-evidence | adaptive | user | Sourced | Deck nguồn | no embedded text | evidence |

## IX. Content Outline

### Part 1: Mở đầu và định hướng

#### Slide 01 - Review nhân sự tháng 7

- **Audience move**: Chưa có bối cảnh → biết rõ kỳ đánh giá, người trình bày và khoảng thời gian.
- **Layout**: Bìa trắng, logo trái trên, tiêu đề lớn bên trái và vòng tròn LUMI lớn lệch phải.
- **Title**: REVIEW NHÂN SỰ
- **Core message**: Tổng kết công việc giai đoạn 20/03–22/07/2026.
- **Content**: Họ và tên: Nguyễn Văn Dương; Review tháng 7/2026; giai đoạn dữ liệu 20/03–22/07.
- **Images**: image_8fa7a601c29ca778.png; image_b3ef018bf0b10f2b.png.
- **Cover impact**: Nhận diện LUMI rõ, tối giản và tự tin.

#### Slide 02 - Nội dung 1/2

- **Audience move**: Chưa biết cấu trúc → hiểu bốn phần đầu của câu chuyện.
- **Layout**: Khung điện thoại cao bên trái có chữ “NỘI DUNG”; bên phải là 4 nhãn số vector theo mẫu gốc, khoảng cách đều.
- **Title**: NỘI DUNG
- **Core message**: Bắt đầu từ kết quả tổng quan rồi đi sâu vào KNX.
- **Content**: 01 Tổng quan kết quả; 02 Thiết bị & firmware KNX; 03 Tool/Jig & benchmark; 04 Kiểm thử hệ thống.
- **Images**: image_8fa7a601c29ca778.png; image_010fcf8f9f909b91.png.

#### Slide 03 - Nội dung 2/2

- **Audience move**: Biết phần đầu → thấy đầy đủ bảy nhóm nội dung, không hiểu nhầm deck chỉ có bốn ý.
- **Layout**: Giữ nguyên khung điện thoại và nhãn số; 3 mục lớn, thoáng hơn, thêm chỉ báo “2/2”.
- **Title**: NỘI DUNG
- **Core message**: Phần sau bao quát đào tạo, dự án khác và định hướng phát triển.
- **Content**: 05 Đào tạo & tài liệu; 06 Dự án/tool khác; 07 Năng lực & bước tiếp theo.
- **Images**: image_8fa7a601c29ca778.png; image_010fcf8f9f909b91.png.

### Part 2: Kết quả tổng quan

#### Slide 04 - Kết quả nổi bật

- **Audience move**: Biết cấu trúc → nắm quy mô và tỷ lệ hoàn thành trong vài giây.
- **Layout**: Một câu kết luận lớn, bốn KPI card 2×2, dải nhóm dự án ở cuối.
- **Title**: Kết quả nổi bật
- **Core message**: 102/114 task đã Done, phần lớn tập trung vào KNX nhưng phạm vi đã mở rộng đáng kể.
- **Content**: 114 task được ghi nhận; 102 Done = 89,5%; 98 task KNX; 7 nhóm dự án gồm KNX, Auto Test, Tool Design, IoT, LumesV2, MSB, Smart Lighting. Trạng thái còn lại: 5 Ongoing, 4 Not yet started, 2 Late, 1 Closed.
- **Visualization**: KPI cards và thanh trạng thái tỷ lệ; data-driven từ CSV.
- **Fact IDs**: CSV-COUNT-114, CSV-DONE-102, CSV-KNX-98, CSV-GROUPS-7.

#### Slide 05 - Hành trình 20/03–22/07

- **Audience move**: Biết tổng số → hiểu nhịp phát triển theo thời gian và sự chuyển dịch phạm vi.
- **Layout**: Timeline ngang 4 chặng với các thẻ bằng chứng ngắn; không dùng bảng.
- **Title**: Hành trình 20/03–22/07
- **Core message**: Công việc tiến từ firmware thiết bị sang tool/hệ thống, rồi đào tạo và mở rộng Auto Test.
- **Content**: 20/03–30/04: firmware và thiết bị KNX; 05/2026: Jig, tool, code loader và test hệ thống; 06/2026: benchmark, giáo trình, ETS/Quiz; 07/2026: LUKA Q&A/Topology và Auto Test servo/cảm biến.
- **Visualization**: Timeline data-driven theo ngày bắt đầu/kết thúc trong CSV.

### Part 3: Trọng tâm KNX

#### Slide 06 - Thiết bị & firmware KNX

- **Audience move**: Biết KNX là trọng tâm → thấy rõ đầu ra kỹ thuật cụ thể.
- **Layout**: Cột trái là 4 thẻ đầu ra; cột phải là ảnh sản phẩm KNX lớn; một dải “impact” ở cuối.
- **Title**: Thiết bị & firmware KNX
- **Core message**: Đã tham gia xuyên suốt từ firmware, thiết bị đến file sản phẩm để sẵn sàng kiểm thử và tích hợp.
- **Content**: Firmware thiết bị 2/4 nút, Rèm và Actuator; phát triển KNOB; tạo/chỉnh sửa file .knxprod; xử lý lỗi và cập nhật hành vi thiết bị qua các vòng test.
- **Images**: image_3db7369d2c1e7d49.jpg.
- **Fact IDs**: CSV-KNX-DEVICE.

#### Slide 07 - Tool, Jig & code loader

- **Audience move**: Thấy đầu ra thiết bị → hiểu các công cụ giúp rút ngắn vòng lặp phát triển.
- **Layout**: 3 module nối theo flow Build → Load → Verify, ảnh Jig bên phải; số thứ tự lớn.
- **Title**: Tool, Jig & code loader
- **Core message**: Tool hóa các bước nạp code và kiểm tra giúp tăng tốc lặp và giảm thao tác thủ công.
- **Content**: Phát triển Jig KNX; tool/code loader; hỗ trợ nạp firmware; benchmark thao tác; hoàn thiện flow kiểm tra và tài liệu sử dụng.
- **Images**: image_bc82a45d35f49412.jpg.
- **Fact IDs**: CSV-KNX-TOOLS.

#### Slide 08 - Benchmark & kiểm thử hệ thống

- **Audience move**: Biết tool hỗ trợ phát triển → thấy chiều sâu kiểm thử hệ thống và xử lý rủi ro.
- **Layout**: Sơ đồ KNX rộng ở nửa phải; nửa trái là ba lớp kiểm thử và hộp “vấn đề đã xử lý”.
- **Title**: Benchmark & kiểm thử hệ thống
- **Core message**: Phạm vi kiểm thử đã mở rộng từ thiết bị đơn lẻ sang hành vi hệ thống và tương tác bus.
- **Content**: Benchmark Jig/tool; test hệ thống; xử lý GA delay/miss; kiểm tra Coupler và GA secure; tái hiện lỗi, đối chiếu và xác nhận sau sửa.
- **Images**: image_6519313ef59a5f53.png.
- **Fact IDs**: CSV-KNX-SYSTEM-TEST.

### Part 4: Chia sẻ tri thức và mở rộng phạm vi

#### Slide 09 - Đào tạo KNX

- **Audience move**: Thấy năng lực triển khai → nhận ra đóng góp vào khả năng tự chủ của đội ngũ.
- **Layout**: Một đường học tập 4 bước: nền tảng → ETS → topology → thực hành; thẻ số lượng đầu ra.
- **Title**: Đào tạo KNX
- **Core message**: Kiến thức KNX được hệ thống hóa thành hành trình học có thể dùng lại.
- **Content**: Giáo trình/khóa đào tạo KNX; slide ETS; Quiz; Topology; LUKA Q&A; hỗ trợ Tester và App; chuẩn hóa nội dung cho người mới.
- **Visualization**: Learning path khái niệm, không phải biểu đồ dữ liệu.
- **Fact IDs**: CSV-KNX-TRAINING.

#### Slide 10 - Tài liệu & khả năng bàn giao

- **Audience move**: Biết có hoạt động đào tạo → thấy các tài sản cụ thể phục vụ bàn giao và tái sử dụng.
- **Layout**: 4 “document cards” dạng trang giấy, mỗi card có loại tài liệu và người dùng chính; kết luận lớn bên phải.
- **Title**: Tài liệu & khả năng bàn giao
- **Core message**: Đầu ra không dừng ở code; tài liệu giúp chuyển giao, kiểm thử và vận hành nhất quán.
- **Content**: Tài liệu API/flow; hướng dẫn tool/Jig; slide đào tạo và Quiz; Q&A/Topology; người dùng chính: Dev, Tester, App và nhân sự mới.
- **Fact IDs**: CSV-DOCS.

#### Slide 11 - Auto Test & Tool Design

- **Audience move**: Hiểu trọng tâm KNX → thấy năng lực được chuyển sang tự động hóa kiểm thử.
- **Layout**: Ảnh Jig dọc bên phải; cột trái có kiến trúc 3 lớp và 4 đầu việc.
- **Title**: Auto Test & Tool Design
- **Core message**: Đang xây nền cho hệ thống Auto Test với servo, cảm biến và mạch điều khiển.
- **Content**: API servo/cảm biến; mô tả luồng hoạt động; module servo/cảm biến; chức năng trên mạch điều khiển; 5 task Ongoing tại thời điểm 22/07 tập trung vào giai đoạn tiếp theo.
- **Images**: image_9f31c49d5ae33b66.jpg.
- **Fact IDs**: CSV-AUTOTEST.

#### Slide 12 - Các dự án & tool khác

- **Audience move**: Biết Auto Test → thấy phạm vi đóng góp đa dự án nhưng vẫn có logic chung.
- **Layout**: Bốn quadrant theo dự án, ảnh sản phẩm/app làm điểm neo; mỗi quadrant một đầu ra ngắn.
- **Title**: Các dự án & tool khác
- **Core message**: Kinh nghiệm firmware, tool và test được tái sử dụng trên nhiều nhóm sản phẩm.
- **Content**: LumesV2 — test/source/programming; MSB — Jig kiểm tra lỗi năng lượng và factory checking; IoT — Luto loader và phối hợp Auto Test; Smart Lighting — tool test Deep Dimming/CCT Tunable.
- **Images**: image_deea19358d7d9df9.jpg; image_5a1205fbd766d78e.png.
- **Fact IDs**: CSV-OTHER-PROJECTS.

### Part 5: Năng lực và bước tiếp theo

#### Slide 13 - Năng lực được củng cố

- **Audience move**: Biết danh sách việc → hiểu năng lực hình thành từ chuỗi đầu ra.
- **Layout**: 5 năng lực xếp theo dạng “radar” không số, nối tới các bằng chứng task cụ thể.
- **Title**: Năng lực được củng cố
- **Core message**: Giá trị nổi bật là khả năng nối firmware, tool, test hệ thống và chia sẻ tri thức thành một chuỗi hoàn chỉnh.
- **Content**: Firmware & thiết bị; Tool/Jig automation; System testing & debugging; Documentation & training; Phối hợp đa nhóm. Mỗi năng lực có 1–2 bằng chứng ngắn từ các slide trước.
- **Visualization**: Capability map khái niệm, không dùng thang điểm tự đánh giá giả.

#### Slide 14 - Trọng tâm tiếp theo

- **Audience move**: Hiểu năng lực hiện tại → có kế hoạch hành động ngắn hạn rõ ràng.
- **Layout**: Ba horizon Now / Next / Scale; bên trái có snapshot 5 Ongoing và phần việc còn lại.
- **Title**: Trọng tâm tiếp theo
- **Core message**: Ưu tiên hoàn tất Auto Test, đóng các task còn mở và chuẩn hóa tài sản dùng lại.
- **Content**: Now: hoàn thành module servo/cảm biến và chức năng mạch điều khiển; Next: đóng Not yet started/Late và xác nhận chất lượng; Scale: chuẩn hóa tool, tài liệu, test case và chia sẻ nội bộ. Chỉ số theo dõi: task Done, thời gian vòng lặp test, số tài sản dùng lại.
- **Visualization**: Roadmap 3 horizon; snapshot trạng thái data-driven từ CSV.

#### Slide 15 - Kết luận

- **Audience move**: Có kế hoạch → ghi nhớ một thông điệp tổng kết và sẵn sàng trao đổi.
- **Layout**: Nền trắng, logo và vòng tròn LUMI, ba dòng kết luận ngắn, “Cảm ơn” lớn.
- **Title**: CẢM ƠN
- **Core message**: Đã tạo kết quả rõ ràng ở KNX, mở rộng năng lực sang automation/tool và có lộ trình tiếp theo cụ thể.
- **Content**: 102 task Done; 7 nhóm dự án; trọng tâm tiếp theo: Auto Test và chuẩn hóa tài sản dùng lại; mời trao đổi.
- **Images**: image_8fa7a601c29ca778.png; image_b3ef018bf0b10f2b.png.
- **Closing impact**: Khép lại bằng kết quả, phạm vi và hành động tiếp theo.

## X. Speaker Notes Requirements

- **Filename**: match each SVG filename under `notes/`
- **Content**: Mỗi trang 50–100 từ tiếng Việt; giải thích thêm chi tiết từ CSV nhưng không đọc lại toàn bộ chữ trên trang; nêu rõ số liệu theo nguồn task list.
- **Total duration**: 15–20 phút
- **Notes style**: conversational, concise, evidence-led
- **Presentation purpose**: report, explain, align
