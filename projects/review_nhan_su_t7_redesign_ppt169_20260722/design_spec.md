<!-- ppt-master-schema: design-spec/v1 -->
# Review nhân sự T7 V2 - Design Spec

## I. Project Information

| Item | Value |
| --- | --- |
| Project Name | Review nhân sự T7 — Nguyễn Văn Dương — V2 |
| Canvas Format | PPT 16:9, 1280 × 720 px |
| Page Count | 17 |
| Target Audience | Quản lý trực tiếp, quản lý kỹ thuật và HR tham gia kỳ review nhân sự tháng 7. |
| Communication Intent | Báo cáo theo từng dự án: thời gian, công việc, kết quả, kỹ năng, tư duy, bài học, khó khăn và thành tích; sau đó tự đánh giá và thống nhất mục tiêu tiếp theo. |
| Desired Audience Outcome | Người xem hiểu rõ đóng góp của từng dự án và có đủ bằng chứng để đánh giá năng lực, tiến bộ và định hướng phát triển. |
| Core Message / Ask / Action | Giai đoạn 20/03–22/07 tạo ra kết quả rõ ràng ở KNX và mở rộng sang Auto Test, Tool Design, IoT, LumesV2, MSB và Smart Lighting. |
| Delivery Context | Review trực tiếp ngày 23/07/2026, thời lượng 15–20 phút; file dùng lại sau buổi họp. |
| Artifact Afterlife | Hồ sơ review nhân sự và mốc đối chiếu cho kỳ review tiếp theo. |
| Reading Mode | balanced |
| Content Strategy | Giữ cấu trúc, bìa, trang nội dung và kết của template gốc; làm đẹp phần thân nhưng không thay đổi tinh thần LUMI. |
| Design Style | Original LUMI refined — giữ template gốc, tăng phân cấp và khoảng thở trong các trang dự án. |
| Formula Policy | text-only |
| AI Image Acquisition Path | not applicable |
| Generation Mode | continuous |
| Spec Refinement | disabled |
| Created Date | 2026-07-23 |

## II. Canvas Specification

| Property | Value |
| --- | --- |
| Format | PPT 16:9 |
| Dimensions | 1280 × 720 |
| viewBox | `0 0 1280 720` |
| Margins | 42 px bìa/kết; 56 px trang nội dung |
| Content Area | x=56–1224, y=42–666 |

## III. Visual Theme

### Theme Style

- **Mode**: briefing
- **Visual style**: swiss-minimal
- **Theme**: LUMI original — bìa/kết xanh, thân trắng, logo góc trái, tiêu đề xanh và motif điện thoại/đường bao số.
- **Tone**: Kỹ thuật, rõ ràng, có bằng chứng, gần template review cũ.

### Color Scheme

| Role | HEX | Purpose |
| --- | --- | --- |
| Background | #FFFFFF | Nền trang nội dung |
| Secondary background | #F4F7F5 | Card và vùng phân nhóm |
| Primary | #008C4F | Xanh LUMI, tiêu đề và nhấn chính |
| Accent | #1456F0 | Trạng thái, kết quả phụ |
| Secondary accent | #79C6A3 | Viền số, connector, nhấn nhẹ |
| Body text | #1F2329 | Nội dung chính |
| Cover background | #008C4F | Bìa và trang kết |
| White text | #FFFFFF | Chữ trên nền xanh |

## IV. Typography System

### Font Plan

| Role | Chinese | English | Fallback tail |
| --- | --- | --- | --- |
| Title | Arial | Arial | sans-serif |
| Body | Arial | Arial | sans-serif |

- **Title stack**: Arial, sans-serif
- **Body stack**: Arial, sans-serif
- **Role rationale**: Arial giữ đúng template gốc và ổn định tiếng Việt khi mở trên PowerPoint Windows.

### Font Size Hierarchy

| Purpose | Anchor Size (px) |
| --- | ---: |
| Body | 22 |
| Title | 36 |
| Subtitle | 28 |
| Annotation | 17 |
| Compact body | 19 |
| Eyebrow | 15 |
| Footer | 14 |
| TOC item | 28 |
| KPI number | 48 |

## V. Layout Principles

### Page Structure

- **Header area**: Logo trái, tiêu đề xanh nằm một dòng, nhãn dự án/phần ở mép phải.
- **Content area**: Trang dự án dùng dải thời gian và lưới review 2×3; KNX được tách ba trang để tránh nhồi chữ.
- **Footer area**: Đường mảnh xám và số trang; bìa/kết dùng www.lumi.vn giống mẫu.

### Spacing Specification

| Element | Current Project |
| --- | --- |
| Safe margin | 56 px |
| Content block gap | 18–28 px |
| Icon-text gap | 10–14 px |

## VI. Icon Usage Specification

- **Primary bundled library**: tabler-outline

| Purpose | Icon Path | Page |
| --- | --- | --- |
| Công việc | tabler-outline/tool | P04–P12 |
| Kết quả | tabler-outline/circle-check | P04–P12 |
| Kỹ năng | tabler-outline/brain | P04–P15 |
| Khó khăn | tabler-outline/alert-triangle | P06–P15 |

## VIII. Image Resource List

| Filename | Dimensions | Ratio | Purpose | Type | Layout pattern | Crop Policy | Acquire Via | Status | Reference | text_policy | page_role |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| image_bb7dad2eee78ee9d.png | 262×76 | 3.42 | Logo LUMI trắng | PNG | cover-brand | no-crop | user | Sourced | Template gốc | no embedded text | brand |
| image_8fa7a601c29ca778.png | 262×76 | 3.45 | Logo LUMI xanh | PNG | content-brand | no-crop | user | Sourced | Template gốc | no embedded text | brand |
| image_b3ef018bf0b10f2b.png | 1143×1143 | 1.00 | Motif vòng tròn bìa/kết | PNG | hero-accent | no-crop | user | Sourced | Template gốc | no embedded text | atmosphere |
| image_010fcf8f9f909b91.png | 465×926 | 0.50 | Điện thoại mục lục | PNG | portrait-left | no-crop | user | Sourced | Template gốc | no embedded text | hero |
| image_3db7369d2c1e7d49.jpg | 1372×784 | 1.75 | Thiết bị KNX | JPG | right-evidence | no-crop | user | Sourced | Template gốc | no embedded text | evidence |
| image_6519313ef59a5f53.png | 1111×619 | 1.79 | Sơ đồ hệ thống KNX | PNG | wide-diagram | no-crop | user | Sourced | Template gốc | preserve text | evidence |
| image_bc82a45d35f49412.jpg | 960×540 | 1.78 | Jig/tool | JPG | right-evidence | adaptive | user | Sourced | Template gốc | no embedded text | evidence |
| image_9f31c49d5ae33b66.jpg | 422×714 | 0.59 | Jig Auto Test | JPG | portrait-right | adaptive | user | Sourced | Template gốc | no embedded text | evidence |
| image_deea19358d7d9df9.jpg | 1024×906 | 1.13 | Công tắc Lumes/MSB | JPG | right-evidence | adaptive | user | Sourced | Template gốc | no embedded text | evidence |
| image_cd22578ee1f97165.png | 359×687 | 0.52 | Màn hình music trên điện thoại | PNG | closing-collage | no-crop | user | Sourced | Template gốc | preserve UI | evidence |
| image_5a1205fbd766d78e.png | 291×625 | 0.47 | Màn hình app Lumi | PNG | closing-collage | no-crop | user | Sourced | Template gốc | preserve UI | evidence |
| image_3f64fe1646839cff.png | 330×656 | 0.50 | Khung điện thoại | PNG | closing-collage | no-crop | user | Sourced | Template gốc | no embedded text | evidence |
| du_an_knx/tool_becnh_mark/bang_dieu_khien.png | 1871×899 | 2.08 | Giao diện điều khiển benchmark KNX | PNG | evidence-filmstrip | no-crop | user | Sourced | Ảnh công việc thực tế | preserve UI | evidence |
| du_an_knx/tool_becnh_mark/tao_test_case.png | 1857×881 | 2.11 | Giao diện tạo test case benchmark KNX | PNG | evidence-filmstrip | no-crop | user | Sourced | Ảnh công việc thực tế | preserve UI | evidence |
| du_an_knx/tool_becnh_mark/bao_cao.png | 1899×891 | 2.13 | Báo cáo benchmark KNX | PNG | evidence-filmstrip | no-crop | user | Sourced | Ảnh công việc thực tế | preserve UI | evidence |
| du_an_knx/tool_nap_code_knx/image.png | 1893×997 | 1.90 | Tool nạp code KNX | PNG | evidence-column | no-crop | user | Sourced | Ảnh công việc thực tế | preserve UI | evidence |
| knx_certificate/course_result.png | 476×305 | 1.56 | Kết quả khóa học KNX Basic | PNG | evidence-inset | no-crop | user | Sourced | Chứng nhận/kết quả đào tạo | preserve text | evidence |
| du_an_tool_design/tool_nap_code/image.png | 1898×982 | 1.93 | Giao diện tool nạp code | PNG | side-evidence | no-crop | user | Sourced | Ảnh công việc thực tế | preserve UI | evidence |

### Image presentation rule

- Ảnh giao diện và chứng nhận là bằng chứng công việc, không dùng như ảnh trang trí.
- Luôn giữ đủ khung hình bằng `meet`/`no-crop`; đặt trên nền trung tính, viền xanh mảnh và chú thích ngắn.
- Khi có nhiều ảnh cùng một luồng, dùng dải bằng chứng đánh số; khi có một đến hai ảnh, dùng cột hoặc panel bằng chứng riêng.
- Các phiên bản sau tiếp tục ngôn ngữ này để có thể bổ sung ảnh theo từng dự án mà không phá bố cục.
- Tiêu đề trang bằng chứng dùng vai trò `evidence_title` 32 px để nhường tối đa diện tích cho screenshot.

## IX. Content Outline

### Part 1: Mở đầu

#### Slide 01 - Review nhân sự
- **Audience move**: Chưa có bối cảnh → biết người review, ngày review và giai đoạn đánh giá.
- **Layout**: Giữ nguyên bìa xanh gốc; chỉ thêm hai dòng thời gian nhỏ dưới tên.
- **Title**: REVIEW NHÂN SỰ
- **Core message**: Review Nguyễn Văn Dương cho giai đoạn 20/03–22/07/2026.
- **Content**: Họ và tên; Ngày review 23/07/2026; Giai đoạn review 20/03–22/07/2026; www.lumi.vn.
- **Images**: white logo và vòng tròn template.
- **Cover impact**: Giống bìa gốc, chỉ bổ sung thông tin cần thiết.

#### Slide 02 - Nội dung
- **Audience move**: Chưa biết cấu trúc → hiểu đúng bốn phần của template gốc.
- **Layout**: Điện thoại trái; bốn ô số viền cắt góc có connector và hatch chéo giống mẫu; nội dung bên phải.
- **Title**: NỘI DUNG
- **Core message**: Giữ nguyên cấu trúc review quen thuộc.
- **Content**: 01 Các dự án tham gia và kết quả; 02 Sử dụng AI trong công việc; 03 Tự đánh giá ưu, nhược điểm; 04 Mục tiêu sắp tới.
- **Images**: green logo và điện thoại mục lục.

### Part 2: Các dự án tham gia và kết quả

#### Slide 03 - Danh mục dự án
- **Audience move**: Biết bốn phần → thấy toàn bộ 7 dự án và thời gian triển khai.
- **Layout**: Timeline portfolio 20/03–22/07, mỗi dự án là một lane ngắn; KPI 114 task và 102 Done.
- **Title**: Các dự án tham gia và kết quả
- **Core message**: 7 nhóm dự án trải từ firmware, tool đến automation và kiểm thử.
- **Content**: KNX; Auto Test; Tool Design; IoT; LumesV2; MSB; Smart Lighting; mốc bắt đầu/kết thúc tương ứng.
- **Visualization**: Timeline data-driven từ CSV.

#### Slide 04 - KNX: Tổng quan dự án
- **Audience move**: Biết KNX là trọng tâm → hiểu thời gian, phạm vi và thành tích chính.
- **Layout**: Dải thời gian 20/03–22/07; ảnh sản phẩm; KPI 98 task/91 Done; ba achievement cards.
- **Title**: 1. Dự án KNX — Tổng quan
- **Core message**: Đóng góp xuyên suốt sản phẩm, tool, hệ thống và đào tạo.
- **Content**: Thời gian; phạm vi; kết quả nổi bật; thành tích: firmware nhiều thiết bị, tool/Jig và benchmark, giáo trình/đào tạo.
- **Images**: thiết bị KNX.

#### Slide 05 - KNX: Công việc và kết quả
- **Audience move**: Biết tổng quan → thấy các đầu việc và đầu ra cụ thể.
- **Layout**: Ba cột lớn Thiết bị / Tool & hệ thống / Tài liệu & đào tạo; không đặt screenshot nhỏ ở trang tổng hợp.
- **Title**: KNX — Công việc chính & kết quả
- **Core message**: Đầu ra KNX bao phủ toàn chuỗi phát triển và vận hành.
- **Content**: Firmware 2/4 nút, Rèm, Actuator, KNOB và .knxprod; Jig/loader/benchmark/GA/Coupler; giáo trình, ETS, Quiz, Q&A, Topology.
- **Images**: Không dùng; ba screenshot được tách thành các trang 06–08.

#### Slide 06 - KNX Benchmark: Bảng điều khiển
- **Audience move**: Biết các nhóm công việc → nhìn rõ giao diện điều khiển benchmark.
- **Layout**: Screenshot no-crop chiếm 65–80% diện tích; một dòng mục đích phía dưới.
- **Title**: KNX Benchmark — Bảng điều khiển
- **Core message**: Theo dõi thiết bị và trạng thái benchmark tập trung.
- **Images**: bang_dieu_khien.png.

#### Slide 07 - KNX Benchmark: Tạo test case
- **Audience move**: Thấy bảng điều khiển → hiểu cách chuẩn hóa dữ liệu kiểm thử.
- **Layout**: Screenshot no-crop chiếm 65–80% diện tích; một dòng kết quả phía dưới.
- **Title**: KNX Benchmark — Tạo test case
- **Core message**: Chuẩn hóa đầu vào và thao tác tạo test case.
- **Images**: tao_test_case.png.

#### Slide 08 - KNX Benchmark: Báo cáo
- **Audience move**: Hiểu cách tạo test → thấy đầu ra báo cáo và truy vết.
- **Layout**: Screenshot no-crop chiếm 65–80% diện tích; một dòng đầu ra phía dưới.
- **Title**: KNX Benchmark — Báo cáo kết quả
- **Core message**: Tổng hợp pass/fail và bằng chứng kiểm thử.
- **Images**: bao_cao.png.

#### Slide 09 - KNX: Kỹ năng, tư duy và bài học
- **Audience move**: Thấy đầu ra → hiểu năng lực, cách tư duy và khó khăn thực tế.
- **Layout**: Bốn thẻ nội dung 2×2 ở trái; cột thành tích và kết quả khóa học ở phải.
- **Title**: KNX — Năng lực & bài học
- **Core message**: Học được cách nhìn hệ thống và biến vấn đề thành quy trình kiểm chứng.
- **Content**: Firmware/ETS/debugging; tư duy end-to-end; bài học chuẩn hóa test; khó khăn GA delay/miss, secure, Coupler và lỗi download; xử lý bằng tái hiện–đo–đối chiếu–xác nhận; thành tích 91 task Done và hoàn thành KNX Basic.
- **Images**: knx_certificate/course_result.png; không crop.

#### Slide 10 - KNX: Tool nạp code
- **Audience move**: Hiểu năng lực → nhìn rõ tool vận hành thực tế.
- **Layout**: Screenshot no-crop chiếm 65–80% diện tích; một dòng giá trị phía dưới.
- **Title**: KNX — Tool nạp code
- **Core message**: Gom cấu hình, điều khiển nhiều máy và log vận hành.
- **Images**: tool_nap_code_knx/image.png.

#### Slide 11 - Auto Test
- **Audience move**: Hiểu KNX → thấy dự án automation mới và trạng thái hiện tại.
- **Layout**: Dải thời gian 06/07–25/07 dự kiến; ảnh Jig; lưới 2×3 review dự án.
- **Title**: 2. Dự án Auto Test
- **Core message**: Xây nền Auto Test với cảm biến màu, servo và mạch điều khiển.
- **Content**: Công việc; kết quả; kỹ năng; tư duy modular/API-first; bài học và khó khăn tích hợp phần cứng; thành tích 4/5 task Done trong phạm vi review.
- **Images**: Jig Auto Test.

#### Slide 12 - Tool Design
- **Audience move**: Biết Auto Test → hiểu đóng góp với tool nguồn nhà máy.
- **Layout**: Dải thời gian 21/05–27/05; bốn thẻ review 2×2 và KPI thành tích; screenshot chuyển sang trang riêng.
- **Title**: 3. Dự án Tool Design
- **Core message**: Chỉnh sửa tool nguồn DC để phù hợp vận hành nhà máy.
- **Content**: Hai task Done; hai task chưa khởi tạo trong dữ liệu; kỹ năng phần cứng/tool; tư duy ưu tiên khả năng bảo trì; bài học về yêu cầu nhà máy; khó khăn thiếu mô tả ở các task mở; thành tích hoàn tất hai vòng chỉnh sửa.
- **Images**: Không dùng ở trang tổng hợp.

#### Slide 13 - Tool Design: Bằng chứng giao diện
- **Audience move**: Hiểu đóng góp → nhìn rõ giao diện tool sau hai vòng chỉnh sửa.
- **Layout**: Screenshot no-crop chiếm 65–80% diện tích; một dòng thành tích phía dưới.
- **Title**: Tool Design — Giao diện vận hành
- **Core message**: Ưu tiên flow nhà máy, ổn định và khả năng bảo trì.
- **Images**: du_an_tool_design/tool_nap_code/image.png.

#### Slide 14 - IoT Team
- **Audience move**: Hiểu tool nhà máy → thấy khả năng hỗ trợ team khác.
- **Layout**: Dải thời gian 26/05–15/06; lưới 2×3 review, nhấn 2/2 Done.
- **Title**: 4. Dự án IoT
- **Core message**: Hoàn thành tool nạp code Luto và phối hợp định hướng Auto Test.
- **Content**: Công việc; kết quả 2/2 Done; kỹ năng loader và phối hợp; tư duy tái sử dụng; bài học làm rõ interface; khó khăn đồng bộ nhiều team; thành tích bàn giao tool.

#### Slide 15 - LumesV2
- **Audience move**: Biết IoT → thấy đầu ra tool cho công tắc cơ smart.
- **Layout**: Dải thời gian 18/05–16/06; ảnh sản phẩm; lưới 2×3 review.
- **Title**: 5. Dự án LumesV2
- **Core message**: Hoàn thành tool test nguồn và tool nạp code cho mạch main V2.
- **Content**: Hai đầu việc Done; kỹ năng test nguồn/nạp code; tư duy tách công đoạn; bài học về flow nhà máy; khó khăn tương thích mạch; thành tích 2/2 Done.
- **Images**: ảnh công tắc Lumes.

#### Slide 16 - MSB Office
- **Audience move**: Hiểu Lumes → thấy năng lực xử lý lỗi Jig tại nhà máy.
- **Layout**: Dải thời gian 07/04–10/04; ảnh Jig; lưới 2×3 review.
- **Title**: 6. Dự án MSB Office
- **Core message**: Fix lỗi đo sai năng lượng và hỗ trợ kiểm tra Jig tại nhà máy.
- **Content**: Công việc; kết quả; kỹ năng đo lường/debug Jig; tư duy dựa trên dữ liệu; bài học về hiệu chuẩn; khó khăn tái hiện lỗi thực địa; thành tích xử lý lỗi đo sai.
- **Images**: ảnh Jig/tool.

#### Slide 17 - Smart Lighting
- **Audience move**: Biết MSB → thấy dự án mới đang triển khai.
- **Layout**: Dải thời gian từ 20/07, trạng thái Ongoing; lưới 2×3 review với phần dự kiến rõ ràng.
- **Title**: 7. Dự án Smart Lighting
- **Core message**: Khởi động tool test cho Driver Deep Dimming/CCT Tunable.
- **Content**: Công việc chính; kết quả hiện tại là xác định phạm vi; kỹ năng cần dùng; tư duy test theo dải; bài học ban đầu; khó khăn chưa đủ dữ liệu; thành tích là dựng nền tool test.

### Part 3: AI và tự đánh giá

#### Slide 18 - Sử dụng AI trong công việc
- **Audience move**: Biết kết quả dự án → hiểu AI hỗ trợ nhưng không thay thế kiểm chứng kỹ thuật.
- **Layout**: Ba use-case lớn: code/debug, tài liệu, học nhanh; một nguyên tắc kiểm chứng.
- **Title**: Sử dụng AI trong công việc
- **Core message**: AI rút ngắn thời gian tìm hiểu và soạn thảo; kết quả kỹ thuật vẫn được kiểm thử thực tế.
- **Content**: Gợi ý code và test case; tóm tắt tài liệu/ETS; chuẩn hóa API/flow/Q&A; nguyên tắc không dùng AI thay cho đo và xác nhận.

#### Slide 19 - Tự đánh giá: Kỹ năng & tư duy
- **Audience move**: Biết cách dùng AI → thấy điểm mạnh và điểm cần cải thiện.
- **Layout**: Hai cột Ưu điểm / Cần cải thiện; dải bằng chứng từ dự án.
- **Title**: Tự đánh giá ưu, nhược điểm
- **Core message**: Điểm mạnh là end-to-end và chủ động; cần cải thiện ưu tiên, ước lượng và đóng task đúng hạn.
- **Content**: Ưu điểm: firmware–tool–test–tài liệu, học nhanh, phối hợp; hạn chế: phân tán nhiều luồng, một số task Late/Not started, cần chuẩn hóa kế hoạch.

#### Slide 20 - Bài học & khó khăn xuyên dự án
- **Audience move**: Biết điểm mạnh/yếu → hiểu các bài học hành động được.
- **Layout**: Bốn cặp Khó khăn → Bài học, nối bằng mũi tên.
- **Title**: Bài học & khó khăn
- **Core message**: Chuẩn hóa interface, test và tài liệu sớm giúp giảm vòng lặp sửa lỗi.
- **Content**: Hệ thống nhiều thiết bị; lỗi khó tái hiện; yêu cầu nhà máy thay đổi; phối hợp đa team; bài học tương ứng về logging, benchmark, checklist và handoff.

### Part 4: Mục tiêu và kết

#### Slide 21 - Mục tiêu sắp tới
- **Audience move**: Hiểu bài học → có kế hoạch cụ thể cho kỳ tiếp theo.
- **Layout**: Now / Next / Scale với chỉ số theo dõi.
- **Title**: Mục tiêu sắp tới
- **Core message**: Hoàn tất Auto Test và Smart Lighting, đóng task còn mở, chuẩn hóa tài sản dùng lại.
- **Content**: Now: Auto Test/Smart Lighting; Next: xử lý Late/Not started; Scale: chuẩn hóa tool, test case, tài liệu và đào tạo; KPI theo dõi.

#### Slide 22 - Cảm ơn
- **Audience move**: Có kế hoạch → kết thúc bằng nhận diện template gốc và sẵn sàng trao đổi.
- **Layout**: Giữ nguyên trang kết xanh, motif vòng tròn và collage ba điện thoại.
- **Title**: CẢM ƠN!
- **Core message**: Kết thúc ngắn gọn, đúng template cũ.
- **Content**: www.lumi.vn.
- **Images**: white logo, vòng tròn và ba màn hình điện thoại.
- **Closing impact**: Khớp trang kết gốc.

## X. Speaker Notes Requirements

- **Filename**: match each SVG filename under `notes/`
- **Content**: 60–100 từ/trang; giải thích bằng chứng từ CSV, phân biệt kết quả thực tế và mục tiêu/dự kiến.
- **Total duration**: 15–20 phút
- **Notes style**: conversational, evidence-led
- **Presentation purpose**: report, explain, align
