# Team

> Điền file này trên repo chung do nhóm trưởng fork. Nhóm điền phần **Thông tin nhóm** và **Thành viên**. Mỗi người tự điền phần của mình trong **Cá nhân**. Không copy file này sang repo khác.

## Thông tin nhóm

- Tên nhóm: H1
- Candidate problem nhóm chọn (1 câu): Khi kết thúc một ngày học, sinh viên phải tự kiểm tra bài tập và deadline rải rác ở LMS, email, nhóm Zalo và Drive (~18 phút/tối), nhưng vẫn bỏ sót thông báo, nhất là tin đổi hạn trong nhóm chat.
- Quyết định cuối (Go / Not Yet / No-Go): Go (phạm vi nhỏ)

## Thành viên

| STT | Họ và tên | MSSV | Vai trò trong nhóm | Tài khoản GitHub |
|---:|---|---|---|---|
| 1 | Vũ Quang Huy | 2A202603782 | Phụ trách CP5 — vẽ quy trình trước/sau, viết Problem Statement v0; hỗ trợ phản biện | huyvu-03 |
| 2 | Nguyễn Văn Minh | 2A202603771 | Phụ trách CP4 — Kiểm chứng & Research; hỗ trợ phản biện | |
| 3 | Phùng Văn Thanh Cao | 2A202603741 | Phụ trách CP6 — mức can thiệp AI, Problem Statement v1, quyết định; hỗ trợ các phần còn lại | ththanh8888 |
| 4 | | | | |

Không ghi email hay số điện thoại vào bảng này, vì repo có thể để public.

Gợi ý vai trò (một người có thể giữ nhiều vai): điều phối thời gian, ghi chép, người phản biện chính, phụ trách kiểm chứng (phỏng vấn/survey), phụ trách research, vẽ quy trình, viết Problem Statement.

## Phân công theo checkpoint

| Checkpoint | Người chính | Người hỗ trợ | Sản phẩm |
|---|---|---|---|
| CP3 — Hội tụ nhóm | | | Cluster, cây OST, bảng chấm điểm |
| CP4 — Kiểm chứng | Nguyễn Văn Minh | Vũ Quang Huy, Phạm Lê Chuẩn, Phùng Văn Thanh Cao | Assumption map, snapshot hoặc survey |
| CP4 — Research | Nguyễn Văn Minh | | Bảng research có link |
| CP5 — Quy trình trước/sau | Vũ Quang Huy | Phùng Văn Thanh Cao (viết lại cho bài deadline) | Quy trình + bảng before/after |
| CP5 — Problem Statement v0 | Vũ Quang Huy | Phùng Văn Thanh Cao (viết lại cho bài deadline) | Problem Statement v0 |
| CP6 — Mức can thiệp + Problem Statement v1 | Phùng Văn Thanh Cao | | Ma trận, AI Canvas, eval, Problem Statement v1 |
| CP6 — Quyết định | Phùng Văn Thanh Cao | | 4 rủi ro + Go/Not Yet/No-Go |

## Cá nhân

Mỗi thành viên thêm một mục theo mẫu dưới đây, tiêu đề là `HoVaTen-MSSV`.

### VuQuangHuy-2A202603782

**Phần việc phụ trách:**

- CP5 — Quy trình trước/sau và Problem Statement v0.
- Hỗ trợ phản biện candidate và rà soát tính nhất quán của bài nhóm.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Mô tả quy trình hiện tại 6 bước và quy trình tương lai 5 bước.
- Xác định bottleneck, bảng before/after, boundary, HITL và phương án quay về.
- Viết Problem Statement v0 với baseline, target và cách đo.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`, mục 4–5.
- `report/individual/2A202603782_VuQuangHuy.md`, mục 4–5.

**Điều mình học được từ phần nhóm:**

- Cần tách rõ problem khỏi solution, dùng bằng chứng để chốt metric và giữ bước con người kiểm tra khi AI có thể sai.

### NguyenVanMinh-2A202603771

**Phần việc phụ trách:**

- CP4 — Kiểm chứng và Research giải pháp đã có.
- Hỗ trợ phản biện candidate và cùng nhóm chốt ranh giới can thiệp AI.

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- Xây dựng Assumption Map 5 giả định và chọn 3 giả định rủi ro cao để kiểm chứng trước.
- Thu thập 3 Interview Snapshot thực tế (Minh, Huy, Chuẩn) theo chuẩn The Mom Test và khảo sát 8 sinh viên.
- Research 3 công cụ tương đồng có link hoạt động (Canvas iCal, Motion, n8n) và đề xuất pivot quy trình sang Daily Digest.

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md`, mục 3.
- `report/individual/2A202603771_NguyenVanMinh.md`, mục 4–5.

**Điều mình học được từ phần nhóm:**

- Đi phỏng vấn thực tế các thành viên trong tem mới thấy thông tin bị nghẽn/miss ở các tin nhắn chat Zalo/LMS/Discord rất nhiều người bị, giúp nhóm hiểu được rõ hơn vấn đề mà người dùng đang mắc phải

### PhungVanThanhCao-2A202603741

**Phần việc phụ trách:**

- Người chính CP6: mức can thiệp AI, Problem Statement v1, tiêu chí đánh giá và quyết định Go / Not Yet / No-Go (`group_report.md` mục 6–8)
- Trao đổi, hỗ trợ các thành viên ở các checkpoint còn lại (CP3–CP5)

**Đóng góp cụ thể** (mình đã làm gì, ra sản phẩm gì):

- CP6: ma trận độ mơ hồ × độ phức tạp, bảng so sánh No AI / Rule / Workflow / Agent, AI Canvas, 2 câu hỏi PAIR, Problem Statement v1 + bảng thay đổi so với v0, 5 tiêu chí đánh giá, chấm 4 rủi ro, quyết định và ngưỡng dừng
- CP3: pitch 5 candidate (#8–#12), trong đó có candidate được nhóm chốt (#9 — tổng hợp bài tập và deadline từ nhiều nguồn)
- CP4: khảo sát trực tiếp 10 sinh viên ngoài nhóm về việc bỏ sót bài tập (8/10 từng bị sót); thay tên thật trong 3 interview snapshot bằng vai trò
- CP5 (hỗ trợ): viết lại quy trình trước/sau và Problem Statement v0 cho bài deadline sau khi nhóm chốt lại candidate
- Mục 9–10 báo cáo nhóm: hạn chế, hướng tiếp theo, tài liệu tham khảo

**Bằng chứng** (phần nào trong `group_report.md`, file nào trong `report/assets/`, commit nào):

- `report/team/group_report.md` mục 6, 7, 8 (CP6)
- `report/individual/2A202603741_PhungVanThanhCao.md` (CP1, CP2)
- `report/team/group_report.md` mục 2.1: candidate #8–#12 do mình pitch
- `report/team/group_report.md` mục 2.4 "Xử lý bất đồng": cùng Huy phản biện việc chọn bài "Khắc phục lỗi code"

**Điều mình học được từ phần nhóm:**

- Vấn đề phải có số đo thực tế mới có thể bảo vệ được. Một ý tưởng dù hợp lý vẫn cần bằng chứng về tần suất, thời gian và mức độ ảnh hưởng; các số liệu ước tính chỉ nên xem là giả thuyết ban đầu, không thay thế được dữ liệu khảo sát hoặc đo lường thực tế.
- Không đưa giải pháp vào Job Story. Khi xác định vấn đề, cần tập trung vào hoàn cảnh, nhu cầu và kết quả người dùng mong muốn thay vì mặc định phải dùng AI hay một công nghệ cụ thể; xác định đúng problem giúp nhóm có nhiều lựa chọn giải pháp và tránh solution-first.
- Không phải vấn đề nào cũng cần AI. Cần so sánh AI với Rule và No AI để xác định công nghệ có thực sự tạo thêm giá trị hay không.
- Nội dung do AI tạo ra cần được kiểm chứng: AI có thể sai số liệu, lệch phạm vi hoặc đưa ra giải pháp không phù hợp; người sử dụng phải chịu trách nhiệm kiểm tra và chọn kết quả cuối cùng.
