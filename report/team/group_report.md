# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi kết thúc một ngày học, sinh viên phải tự kiểm tra bài tập và deadline rải rác ở LMS, email, nhóm Zalo và Drive (~18 phút/tối), nhưng vẫn bỏ sót thông báo, nhất là tin đổi hạn trong nhóm chat.
- Quyết định cuối: **Go (phạm vi nhỏ)** (xem mục 8)

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
| --- | --- | --- | --- | --- | --- |
| 1 | Nguyễn Văn Minh | Muốn tóm tắt nhanh tiền sử bệnh để bác sĩ nắm ngay. | Mẹ/người thân, bác sĩ | Tìm lại thông tin từ giấy khám cũ (tốn thời gian lúc khám). | "Nhóm học IT, có đủ chuyên môn y tế để đánh giá bản tóm tắt đúng/sai không?" (Chuẩn) |
| 2 | Phạm Lê Chuẩn | Muốn biết nhanh hệ thống lỗi ở đâu để khắc phục ngay. | IT, kĩ thuật | Dò lỗi cú pháp hoặc tìm nguyên nhân gây lỗi (20-30 phút). | "Dùng AI chỉ lỗi luôn thì sinh viên có bị lười tư duy đi không?" (Cao) |
| 3 | Phạm Lê Chuẩn | Muốn tự động sắp xếp lịch trình, đặt lịch, nhắc hẹn. | Mọi người | Tự kiểm tra, đối chiếu lịch thủ công. | "Làm sao AI truy cập được tin nhắn Zalo cá nhân để lấy lịch?" (Huy) |
| 4 | Phạm Lê Chuẩn | Muốn điểm danh đầu/cuối ca học nhanh chóng. | Sinh viên, Giảng viên/trợ giảng | Xếp hàng chờ quét mã/gọi tên (15-20 phút). | "Bài này dùng mã QR tĩnh (Rule) là đủ, cần gì AI?" (Minh) |
| 5 | Vũ Quang Huy | Muốn xác định chủ đề trọng tâm từ đề cương ôn tập dài. | Sinh viên/Học sinh | Đọc dàn trải số lượng trang đề cương lớn. | "Mỗi môn cấu trúc khác nhau, đo lường độ chính xác của trọng tâm thế nào?" (Cao) |
| 6 | Vũ Quang Huy | Muốn nắm bài tập và deadline sắp tới để không bỏ sót. | Sinh viên/Học sinh | Phải lội 2-3 nguồn (LMS, nhóm lớp) mỗi tuần. | "Nếu trường đổi API của LMS thì giải pháp có sập không?" (Chuẩn) |
| 7 | Vũ Quang Huy | Muốn nắm thông tin quan trọng từ nhiều kênh thông báo của GV. | Sinh viên/Học sinh | Bỏ lỡ thông báo do trôi tin nhắn trên nhiều kênh. | "Quyền truy cập dữ liệu đa kênh cá nhân lấy ở đâu?" (Minh) |
| 8 | Phùng Văn Thanh Cao | Muốn lên kế hoạch học tập buổi tối theo deadline, độ khó. | Sinh viên | Mất 10-20 phút xếp việc nhưng vẫn miss deadline. | "Độ khó là cảm nhận chủ quan, hệ thống đo lường kiểu gì?" (Huy) |
| 9 | Phùng Văn Thanh Cao | Muốn tổng hợp deadline từ LMS, email, nhóm lớp. | Sinh viên | Lướt nhiều nguồn mỗi tối dễ bị sót thông tin. | "Có trùng lặp ý tưởng với bài toán quản lý deadline của Huy không?" (Cao) |
| 10 | Phùng Văn Thanh Cao | Muốn có hướng dẫn phân tích, từng bước tiếp cận bài khó. | Sinh viên | Tốn 1-2 tiếng kẹt lại không tìm được hướng giải. | "Làm sao ngăn chặn việc AI giải hộ luôn thay vì chỉ hướng dẫn?" (Minh) |
| 11 | Phùng Văn Thanh Cao | Muốn tổng hợp kiến thức trọng tâm cuối ngày học. | Sinh viên | Mất 45-60 phút tự đọc lại slide. | "Nếu input là file ghi âm bài giảng thì xử lý thế nào?" (Huy) |
| 12 | Phùng Văn Thanh Cao | Muốn theo dõi tiến độ task để không ảnh hưởng nhóm. | Sinh viên, thành viên nhóm | Nhắc nhở thủ công, trùng lặp công việc. | "Đây là vấn đề ý thức hay do thiếu công cụ quản lý?" (Huy) |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
| --- | --- | --- |
| A | Hỗ trợ học tập / Ôn thi (5, 10, 11) | Rút gọn, tóm tắt và phân tích khối lượng tài liệu học thuật lớn. |
| B | Quản lý lịch & Deadline (3, 6, 7, 8, 9, 12) | Gom thông tin rải rác từ nhiều nguồn (LMS, Zalo, Email) để lập kế hoạch. |
| C | Tối ưu quy trình & Kỹ thuật (1, 2, 4) | Giảm thao tác lặp lại tốn thời gian ở một bước xử lý/đọc dữ liệu cụ thể. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thời gian sinh viên IT/kỹ thuật bị kẹt lại khi hệ thống báo lỗi / lỗi code bài lab.
├── Opportunity A: Thông báo lỗi (log) của hệ thống quá dài và chứa nhiều thông tin rác.
├── Opportunity B: Việc copy mã lỗi lên Google trả về quá nhiều luồng ý kiến, phải tự chắt lọc.
└── Opportunity C: Sinh viên không xác định được chính xác dòng code nào là nguyên nhân gốc rễ.

```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

* "Tích hợp công cụ debug bằng AI vào thẳng phần mềm VS Code"
* "Chatbot tự động viết lại code cho đúng"

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Theo dõi tiến độ task nhóm (Cao) | 5 | 4 | 5 | 5 | 4 | 5 | 5 | **33** |
| Khắc phục lỗi hệ thống/code bài lab (Chuẩn) | 5 | 5 | 4 | 4 | 3 | 4 | 3 | **28** |
| Tóm tắt tiền sử bệnh án (Minh) | 4 | 4 | 3 | 3 | 5 | 4 | 2 | **25** |

**Candidate được chọn (vòng CP3):**
Theo dõi tiến độ task nhóm để không ảnh hưởng kết quả chung (Phùng Văn Thanh Cao). *Sau CP4, nhóm đã chốt lại sang candidate #9, xem phần "Cập nhật sau CP4" ở cuối mục này.*

**Vì sao chọn:**
Đây là nỗi đau (pain point) cực kỳ phổ biến mà bất kỳ sinh viên nào cũng gặp phải ("gánh team", trễ deadline do không ai nhắc, trùng lặp công việc). Bài toán có đối tượng rất rõ ràng, dễ dàng tìm người phỏng vấn để lấy bằng chứng ngay trong lớp. Impact đo lường được định lượng thông qua số lần trễ hạn hoặc số phút phải bỏ ra để họp nhóm/nhắn tin nhắc nhở mỗi tuần. Đặc biệt, bài toán này rất dễ để so sánh các mức can thiệp: từ No AI (chỉ dùng Trello/Excel), Rule (bot tự động nhắc giờ), đến Workflow (AI tự tóm tắt tiến độ từ tin nhắn chat và cập nhật trạng thái).

**Vì sao loại các candidate còn lại:**

* Bài "Khắc phục lỗi code bài lab": Dù quy trình rõ ràng, nhưng các lỗi (bug) có độ khó rất khác nhau, dẫn đến việc đo lường baseline thời gian trung bình thiếu chính xác. Hơn nữa, mức độ phức tạp của bài lab có thể vượt quá khả năng đánh giá của một số thành viên trong nhóm, dẫn đến rủi ro khó kiểm định chất lượng đầu ra của AI.
* Bài "Tóm tắt bệnh án": Bị loại do nhóm hoàn toàn không có chuyên môn y tế, rủi ro đánh giá sai tính sinh mạng (Feasibility/Viability rất cao).

**Xử lý bất đồng (nếu có):**
Chuẩn ban đầu muốn giữ bài "Khắc phục lỗi code" vì mang đậm tính kỹ thuật IT. Tuy nhiên, Cao và Huy đã phản biện và chỉ ra rằng bài "Theo dõi task nhóm" dễ thu thập dữ liệu (input) từ các đoạn chat nhóm trên Zalo/Discord hơn là việc trích xuất log lỗi hệ thống trên các môi trường máy ảo khác nhau. Nhóm đi đến thống nhất chọn bài Task Nhóm vì tệp người dùng rộng hơn, tính khả thi cao và "vừa sức lab" hơn để thiết kế một quy trình (workflow) hoàn chỉnh.

**Cập nhật sau CP4 — nhóm chốt lại candidate:**
Khi kiểm chứng ở CP4, toàn bộ bằng chứng thu được đều xoay quanh việc **bỏ sót bài tập và deadline từ nhiều nguồn** (candidate #9, cùng pattern với #6 của Huy, cluster B): 8/10 sinh viên ngoài nhóm từng bị sót bài tập; 6/8 sinh viên trong micro survey từng sót hoặc suýt trễ deadline trong tháng trước; 7/8 phải theo dõi từ 3 nguồn trở lên. Trong khi đó, bài "Theo dõi task nhóm" chưa có bằng chứng từ người ngoài nhóm. Vì vậy nhóm chốt lại candidate cuối cùng là **#9 — Tổng hợp bài tập và deadline từ LMS, email, nhóm Zalo và Drive** (gộp với #6). Các mục CP5–CP6 bên dưới được viết cho candidate này.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | Sinh viên học từ 4–5 môn/kỳ đều mất từ 20–30 phút mỗi tối để lướt kiểm tra bài tập và deadline từ nhiều nguồn rời rạc (LMS, Zalo, Teams, Email). | Value | 5 | 2 | ✅ |
| 2 | Đa số các lần bị trễ hạn hoặc bỏ sót deadline xuất phát từ các thông báo không có cấu trúc (dặn dò trong nhóm chat Zalo/Teams, slide bài giảng) chứ không phải bài tập chính thức đã tạo trên LMS. | Value | 5 | 2 | ✅ |
| 3 | Sinh viên sẵn sàng dành 2–3 phút mỗi tối để xem lại và bấm duyệt danh sách deadline do hệ thống tổng hợp thay vì tự đi tìm thủ công. | Usability | 4 | 3 | — |
| 4 | Có thể lấy dữ liệu bài tập từ LMS tự động qua chuẩn lịch iCal, và trích xuất ngày giờ hạn nộp từ tin nhắn ngôn ngữ tự nhiên bằng Rule/LLM. | Feasibility | 4 | 4 | — |
| 5 | Sinh viên lo ngại rủi ro bảo mật thông tin cá nhân và không sẵn sàng cấp quyền truy cập toàn bộ tài khoản chat Zalo cá nhân cho một ứng dụng bên thứ ba. | Viability | 5 | 1 | ✅ |

Giả định nhóm kiểm chứng trong buổi này: **Giả định #1, #2 và #5** (nhóm giả định có độ quan trọng cao nhưng bằng chứng thực tế còn thấp).

### 3.2. Kiểm chứng

**Cách đã dùng:** Phỏng vấn 3 sinh viên là **thành viên trong nhóm** (thành viên A, B, C) về trải nghiệm thực tế đã xảy ra, theo 3 luật The Mom Test + khảo sát trực tiếp 10 sinh viên ngoài nhóm + khảo sát nhanh (micro-survey) 8 sinh viên trong lớp L3B.

*Lưu ý: đề yêu cầu không phỏng vấn thành viên nhóm mình. Vì vậy nhóm dùng **hai khảo sát với người ngoài nhóm (18 sinh viên)** làm bằng chứng chính; 3 snapshot dưới đây chỉ dùng để mô tả chi tiết quy trình và các workaround. Hạn chế này được ghi ở mục 9.*

#### Interview Snapshot #1 — Thành viên A (trong nhóm)

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 2 ngành AI / Kỹ thuật (thành viên trong nhóm), đang theo học các môn lab thực hành và đồ án dự án |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Sợ nhất là hạn nộp bài trên LMS ghi là Chủ nhật, nhưng tối thứ Sáu trợ giảng ghim tin nhắn trong nhóm Zalo bảo nộp sớm vào sáng thứ Bảy để chấm bù; mình mà không lướt Zalo lúc 23h đêm là coi như sáng hôm sau mất trắng 20% điểm."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước ở môn Lập trình/AI, suýt bị trễ hạn nộp bài lab vì thông báo cập nhật rubric và hạn nộp của trợ giảng bị trôi sau hàng chục tin nhắn thảo luận bài của các bạn trong nhóm chat Zalo. |
| Hiện đang xử lý bằng cách nào (workaround)? | Chụp ảnh màn hình các đoạn tin nhắn quan trọng gửi vào mục "Cloud của tôi" trên Zalo hoặc tự copy paste vào ứng dụng Google Keep/Notion cá nhân. |
| Mất bao lâu, bao lần? | Mỗi tối mất 20–25 phút trước giờ ngủ (khoảng 22h–23h) mở lần lượt Canvas LMS, nhóm Zalo lớp và Teams để rà soát; lặp lại đều đặn 4–5 buổi/tuần. |
| Insight / opportunity rút ra | Nỗi đau lớn nhất không nằm ở việc thiếu lịch của LMS (LMS đã có lịch rõ ràng), mà nằm ở việc thông tin bài tập bị phân mảnh ở **các kênh chat phi chính thức (Zalo/Teams)** với định dạng văn bản tự do, rất dễ trôi mất nếu không đọc kịp. |

#### Interview Snapshot #2 — Thành viên B (trong nhóm)

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 2 ngành Công nghệ Thông tin (thành viên trong nhóm), theo dõi nhiều kênh học tập và thông báo môn học cùng lúc |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Thông báo thì giảng viên gửi qua Email trường, bài tập thì nộp trên LMS, còn lịch dời ca học hay dặn dò bài tập lớn thì trợ giảng lại nhắn vào nhóm Zalo; mỗi tối mở đủ 3 cái ứng dụng để check bài là hết cả buổi tối."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Đợt vừa rồi giảng viên gửi email thông báo thay đổi đề cương và dời hạn nộp bài tập lớn, nhưng vì hòm thư sinh viên nhận quá nhiều email thông báo tự động từ trường nên email quan trọng bị trôi mất, dẫn đến bị nộp trễ 1 ngày. |
| Hiện đang xử lý bằng cách nào (workaround)? | Dùng một cuốn sổ tay nhỏ đặt trên bàn học để tự ghi lại danh sách deadline đầu tuần; tuy nhiên giữa tuần giảng viên đổi lịch đột xuất là sổ tay bị sai lệch ngay. |
| Mất bao lâu, bao lần? | Đầu mỗi tuần mất khoảng 30–40 phút ngồi gom bài; mỗi buổi tối mất thêm 15–20 phút kiểm tra lại các kênh; kỳ trước từng bị trễ 1 bài tập quan trọng. |
| Insight / opportunity rút ra | Thông tin quan trọng thường bị "chôn vùi" trong biển thông báo; giải pháp cần có tính năng **bóc tách chính xác nội dung chứa bài tập/hạn chót** thay vì bắt sinh viên phải tự đọc và lọc thủ công hàng chục thông báo mỗi ngày. |

#### Interview Snapshot #3 — Thành viên C (trong nhóm)

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | Sinh viên năm 2 ngành Kỹ thuật Hệ thống / IT (thành viên trong nhóm), thường xuyên làm bài tập kỹ thuật và đồ án nhóm |
| Câu nói đáng nhớ nhất (nguyên văn) | *"Mình muốn có một công cụ nhìn vào là biết tối nay và ngày mai phải nộp bài gì ngay lập tức, chứ không muốn mất thời gian tự tay ngồi gõ từng đầu việc vào ứng dụng nhắc việc."* |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Thứ Sáu tuần trước, ngồi sửa lỗi code cho bài lab đến tận 1h sáng nên quên bẵng mất có một bài kiểm tra trắc nghiệm lý thuyết ngắn phải hoàn thành trước 23h59 trên LMS. |
| Hiện đang xử lý bằng cách nào (workaround)? | Dùng ứng dụng nhắc việc trên điện thoại (Apple Reminders / Google Tasks) nhưng vì phải tự gõ tay từng bài nên nhiều hôm mệt mỏi quên không nhập, dẫn đến app không nhắc được. |
| Mất bao lâu, bao lần? | Mất 15–20 phút tự đối chiếu và kiểm tra lịch mỗi ngày; tháng trước bị trễ 2 bài quiz trắc nghiệm do không ai nhắc. |
| Insight / opportunity rút ra | Sinh viên có tâm lý ngại nhập liệu thủ công; việc tổng hợp bài tập phải diễn ra **tự động hoặc bán tự động (tối thiểu thao tác nhập tay)**, và phải làm nổi bật những việc sắp hết hạn trong vòng 24 giờ tới. |

#### Tổng hợp kết quả kiểm chứng:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| Phỏng vấn sâu (The Mom Test) — thành viên trong nhóm | 3 (thành viên A, B, C) | Cả 3/3 sinh viên xác nhận mất 15–25 phút mỗi tối để rà soát bài tập; việc bỏ sót deadline đều do thông báo bị phân mảnh ở nhiều kênh (LMS, Zalo, Teams, Email). | Thành viên C phản bác: Nếu giải pháp yêu cầu cấp mật khẩu hoặc quyền đọc toàn bộ tin nhắn Zalo cá nhân thì sẽ không dùng vì lo ngại an toàn dữ liệu riêng tư.<br>Thành viên A và B phản bác: Nếu bot tự động gom quá nhiều thông báo rác (lời cảm ơn, chat chit trong nhóm lớp) thì sẽ làm ngập lụt thông báo và bị tắt chuông. |
| Khảo sát trực tiếp (Phùng Văn Thanh Cao thực hiện) | 10 sinh viên ngoài nhóm | 8/10 sinh viên cho biết từng bị sót bài tập hoặc deadline | 2/10 sinh viên cho biết họ thường xuyên tự kiểm tra thông tin nên tránh được việc bỏ sót. Câu hỏi còn chung chung ("có hoàn thành hết bài tập hay bị sót phần nào không"), chưa hỏi lần gần nhất và nguyên nhân |
| Micro survey trong lớp | 8 sinh viên lớp L3B | 7/8 sinh viên xác nhận phải theo dõi bài tập từ 3 nguồn trở lên; 6/8 người từng bị sót hoặc suýt trễ deadline ít nhất 1 lần trong tháng trước. | 1/8 sinh viên cho biết lớp họ giảng viên cam kết 100% chỉ dùng Canvas LMS nên chỉ cần xem LMS là đủ; 2/8 người đề nghị phải có chế độ tóm tắt ngắn gọn dưới 5 dòng mỗi tối thay vì gửi danh sách quá dài. |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**
1. **Thu hẹp ranh giới (Boundary) và cách lấy dữ liệu:** Nhóm hủy bỏ ý tưởng "tự động đọc mọi tin nhắn từ Zalo cá nhân" (vướng rào cản bảo mật và quyền riêng tư theo phản bác của thành viên C ở Giả định #5). Thay vào đó, nhóm chuyển sang mô hình lai: **Tự động đồng bộ bài tập chính thức từ LMS qua chuẩn iCal/RSS + Cho phép sinh viên chủ động forward/dán tin nhắn dặn dò vào bot để AI bóc tách ngày giờ hạn nộp.**
2. **Cơ chế xác nhận con người (Human-in-the-loop):** Để tránh việc AI trích xuất nhầm hoặc làm phiền sinh viên (theo phản bác của thành viên A và B, cùng 2/8 sinh viên trong micro survey, về ngập lụt thông báo), nhóm bổ sung bước: Hệ thống chỉ gửi **1 bản tin Daily Digest ngắn gọn vào lúc 22h00** tóm tắt các task sắp tới, sinh viên kiểm tra và bấm xác nhận trước khi lưu vào lịch cá nhân.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Canvas LMS Calendar Feed (iCal)** | https://community.canvaslms.com/t5/Student-Guide/How-do-I-subscribe-to-the-Calendar-feed-using-Google-Calendar/ta-p/522 | Bước 1: Lấy bài tập chính thức từ LMS Canvas đồng bộ về Google/Apple Calendar. | Chuẩn iCal toàn cầu, hoàn toàn tự động, độ trễ thấp, ổn định 100%, không tốn chi phí và không cần AI. | Hoàn toàn không lấy được bài tập dặn dò qua Zalo, Teams, slide hay email của giảng viên. | **Không dùng AI cho phần LMS**. Bước này chỉ cần dùng Rule (iCal feed) có sẵn, vừa chính xác tuyệt đối vừa tiết kiệm tài nguyên. |
| **Motion (usemotion.com)** | https://www.usemotion.com/ | Bước tự động tính toán và xếp lịch làm bài tập vào các khoảng thời gian trống trong ngày. | Thuật toán xếp lịch và phân bổ thời gian theo mức độ ưu tiên và deadline rất thông minh. | Chi phí quá đắt ($19/tháng), không phù hợp sinh viên; người dùng vẫn phải tự gõ task thủ công; không có khả năng đọc hiểu tin nhắn chat tiếng Việt. | Sinh viên không cần một hệ thống xếp lịch đắt tiền, nhu cầu cốt lõi nằm ở bước **thu thập và trích xuất thông tin rải rác từ các kênh chat/email tiếng Việt**. |
| **Template n8n: AI Message Summarizer & Task Extractor** | https://n8n.io/workflows/1888-summarize-messages-using-openai/ | Bước 2–3: Đọc tin nhắn từ kênh chat (webhook), dùng LLM trích xuất deadline thành cấu trúc JSON. | Kiến trúc Workflow định sẵn rõ ràng, dùng AI bóc tách ngôn ngữ tự nhiên thành dữ liệu có cấu trúc rất hiệu quả. | Zalo hạn chế API bot cá nhân; nếu AI trích xuất sai ngày giờ deadline mà tự động tạo lịch sẽ gây hậu quả bỏ sót bài. | Áp dụng mô hình Workflow của n8n nhưng **bắt buộc phải có bước sinh viên duyệt lại (Human-in-the-loop)** trước khi đưa task vào lịch chính thức. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
HIỆN TẠI — 5 bước, ~18 phút/tối, 5/5 bước thủ công, lặp lại 4–5 tối/tuần

[1 Mở LMS xem bài mới: 3']
→ [2 Kiểm tra email trường: 2']
→ [3 Đọc các nhóm Zalo lớp/môn: 6'] ← BOTTLENECK
→ [4 Xem Drive/tài liệu môn học: 3']
→ [5 Ghi deadline vào sổ/ghi chú cá nhân: 4']
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Handoff / ghi chú |
|---:|---|---|---|---|---|
| 1 | Sinh viên | Trang LMS các môn đang học | Danh sách bài tập chính thức mới và hạn nộp | ~3 phút/tối, 4–5 tối/tuần | Thông tin có cấu trúc, ít khi sót; chuyển sang bước 5 để ghi lại |
| 2 | Sinh viên | Hộp thư email trường | Thông báo của giảng viên: đổi đề cương, dời hạn | ~2 phút/tối | Email quan trọng dễ bị chìm giữa email tự động của trường (CP4, snapshot #2) |
| 3 | Sinh viên | Các nhóm Zalo lớp/môn | Tin dặn dò bài tập, tin đổi hạn hoặc nộp sớm | ~6 phút/tối | **Bottleneck:** thông báo lẫn trong tin trò chuyện, viết dạng tự do, dễ trôi; đây là nguồn chính của các lần sót (CP4, giả định #2) |
| 4 | Sinh viên | Drive/tài liệu môn học | Đề bài, rubric, yêu cầu nộp | ~3 phút/tối | Thường phải mở sau khi thấy nhắc trong Zalo hoặc email |
| 5 | Sinh viên | Kết quả bước 1–4 | Danh sách deadline trong sổ/ghi chú | ~4 phút/tối | Không có handoff; nếu giữa tuần đổi hạn thì danh sách bị sai mà không ai báo |

**Bottleneck chính:** Bước 3, đọc các nhóm Zalo (~6 phút/tối). Thông báo bài tập và tin đổi hạn bị lẫn trong tin trò chuyện, viết bằng ngôn ngữ tự do, nên dễ trôi và dễ sót. CP4 xác nhận phần lớn các lần sót đến từ kênh chat và email, không phải từ LMS (giả định #2; snapshot #1, #2). Số phút từng bước là ước tính từ trải nghiệm của người đề xuất (Problem Card #1), khớp với khoảng 15–25 phút/tối ghi nhận ở CP4.

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
TƯƠNG LAI — 6 bước, mục tiêu dưới 5 phút thao tác mỗi tối,
2/6 bước có thao tác của sinh viên

[1 Đồng bộ bài tập LMS sang Google Calendar qua iCal feed: tự động]      ← RULE
→ [2 Sinh viên chọn và dán/forward tin dặn dò Zalo, email trong ngày: 1–2'] ← CON NGƯỜI
→ [3 Trích "môn – bài – hạn – loại (mới/đổi hạn) – câu nguồn": < 1']      ← AI
→ [4 Gộp trùng với lịch LMS, đánh dấu đổi hạn, tạo Daily Digest 22h ≤ 5 dòng: tự động] ← RULE
→ [5 Sinh viên duyệt digest, sửa nếu cần, bấm xác nhận: ~2']             ← CON NGƯỜI (HITL)
→ [6 Lưu mục đã xác nhận vào lịch; nhắc trước hạn 24 giờ: tự động]       ← RULE

BOUNDARY:
- AI chỉ xử lý văn bản do sinh viên chủ động dán hoặc forward; không đăng nhập,
  không đọc tài khoản Zalo, email hay LMS.
- Dữ liệu LMS đi qua iCal (Rule), không qua AI.
- Nguồn không nêu rõ môn hoặc hạn thì AI ghi "thiếu thông tin", không tự suy đoán.
- Hạn trên LMS khác hạn trong tin nhắn thì hiện cả hai, sinh viên quyết định.
- AI không tự tạo, sửa, xóa lịch và không tự gửi nhắc; chỉ mục sinh viên đã xác nhận
  mới vào lịch.

PHƯƠNG ÁN QUAY VỀ:
- AI trích sai, thiếu hoặc không hoạt động → sinh viên bỏ bản nháp, quay về checklist
  4 nguồn thủ công (bước 2–5 của quy trình hiện tại). Lịch LMS từ iCal và Rule nhắc hạn
  vẫn chạy bình thường vì không phụ thuộc AI.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | 5 | 6 | Thêm bước tự động (Rule) nhưng giảm thao tác tay |
| Tổng thời gian thao tác | ~18 phút/tối | Dưới 5 phút/tối | Chỉ còn bước dán tin (1–2') và duyệt digest (~2') |
| Số bước thủ công | 5/5 | 2/6 | Sinh viên vẫn chọn nguồn và xác nhận cuối cùng |
| Bottleneck chính | Đọc nhóm Zalo, dễ sót tin đổi hạn | Sinh viên duyệt digest | Điểm kiểm tra của con người được giữ để bảo đảm không sót |
| Rủi ro mới phát sinh | — | AI trích sai hạn hoặc bỏ sót tin đổi hạn; sinh viên quên dán tin; digest dài gây ngập thông báo; lộ nội dung chat của lớp | Xử lý bằng boundary, HITL ở bước 5, giới hạn digest ≤ 5 dòng và phương án quay về |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên phải theo dõi bài tập và deadline từ nhiều kênh (LMS, email trường, nhóm Zalo lớp/môn, Drive) |
| **Quy trình** | Mỗi tối, sinh viên lần lượt mở LMS, kiểm tra email trường, đọc các nhóm Zalo, xem Drive tài liệu, rồi tự ghi deadline vào sổ/ghi chú cá nhân |
| **Bottleneck** | Bước đọc các nhóm Zalo (~6 phút/tối): thông báo bài tập và tin đổi hạn bị lẫn trong tin trò chuyện, viết dạng tự do, dễ trôi và dễ sót |
| **Impact** | ~18 phút/tối ≈ 1,8 giờ/tuần; sót ~1 deadline/tháng và bị trừ điểm. CP4: 8/10 sinh viên ngoài nhóm từng bị sót bài tập; 6/8 sinh viên trong micro survey từng sót hoặc suýt trễ deadline trong tháng trước |
| **Success Metric** (baseline → target, cách đo) | Thời gian rà soát bài tập mỗi tối từ ~18 phút xuống dưới 5 phút; số deadline bị sót từ ~1/tháng xuống 0 trong 4 tuần. Đo bằng cách sinh viên tự bấm giờ mỗi tối và ghi số deadline bị sót (đối chiếu với LMS và thông báo gốc) trong 4 tuần |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI không đăng nhập hay đọc tài khoản Zalo, email cá nhân; không tự tạo lịch và không tự gửi nhắc. Sinh viên phải xác nhận từng deadline trước khi lưu vào lịch |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- **Phản biện từ AI (Claude):** Metric chỉ đo thời gian và số lần sót, chưa đo chất lượng đầu ra của bước trích xuất. Nhanh hơn mà phải sửa nhiều thì không đạt. → **Đồng ý**, bổ sung metric "≤ 10% mục phải sửa" ở v1.
- **Phản biện từ AI (Claude):** Actor "sinh viên" quá rộng. CP4 có 1/8 sinh viên chỉ cần xem LMS là đủ, nên không gặp pain này. → **Đồng ý**, v1 thu hẹp actor về sinh viên học 4–6 môn/kỳ, theo dõi từ 3 kênh trở lên.
- **Phản biện từ AI (Claude):** Boundary chưa nói AI xử lý gì khi nguồn thiếu thông tin hoặc khi hạn trên LMS mâu thuẫn với tin nhắn. → **Đồng ý**, bổ sung ở v1: không suy đoán, hiện cả hai hạn.
- **Phản biện từ AI (Claude):** Baseline 18 phút là ước tính của một người. → **Đồng ý một phần**: giữ 18 phút làm baseline vì nằm trong khoảng 15–25 phút ghi nhận ở CP4, nhưng sẽ đo lại thật trong pilot.

---


## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ phức tạp cao × Độ mơ hồ thấp** → *Workflow nhiều bước rõ ràng, chưa chắc cần Agent*.

Vì sao:

- **Độ phức tạp cao:** thông tin bài tập nằm ở **4 nguồn** (LMS, email trường, nhóm Zalo lớp/môn, Drive tài liệu). Quy trình có nhiều bước nối tiếp: lấy dữ liệu → trích deadline → so với lịch LMS để phát hiện trùng hoặc đổi hạn → tổng hợp → sinh viên xác nhận. Bước sau phụ thuộc kết quả bước trước.
- **Độ mơ hồ thấp ở đầu ra:** một deadline trích ra hoặc **đúng, hoặc sai** (đúng môn, đúng bài, đúng ngày giờ), kiểm tra được bằng cách đối chiếu câu nguồn. Không có kiểu "nhiều đáp án đều chấp nhận được" như viết narrative.
- **Phần khó nằm ở đầu vào:** tin nhắn Zalo và email dặn dò viết bằng tiếng Việt tự do ("thứ 6 tuần sau nộp nhé", "dời sang CN", "bài lab 3 nộp sớm sáng thứ 7"). Đây là lý do cần AI ở **đúng một bước** trích xuất. Còn các bước khác cố định, nên chỉ cần Workflow, không cần Agent.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | Lớp trưởng ghim mọi thông báo bài tập; Google Sheet deadline chung của lớp; bật thông báo LMS; sinh viên dùng checklist kiểm tra 4 nguồn mỗi tối | Khi lớp có người cập nhật Sheet đều đặn, hoặc giảng viên chỉ dùng LMS (1/8 sinh viên trong micro survey ở CP4 thuộc trường hợp này) | Phụ thuộc lớp trưởng; tin dặn dò và đổi hạn trong Zalo vẫn trôi; sinh viên vẫn mất ~18 phút/tối | Không làm giải pháp chính; **dùng làm phương án quay về** |
| **Rule** | Đồng bộ bài tập LMS sang Google Calendar qua iCal feed (mục 3.3); lọc email theo người gửi là giảng viên/trợ giảng và từ khóa "hạn nộp", "deadline"; nhắc tự động trước hạn 24 giờ | Khi deadline nằm ở nguồn có cấu trúc (LMS, email có tiêu đề rõ) | Không bóc tách được tin nhắn Zalo viết tự do; lọc từ khóa bỏ sót các câu như "nộp sớm sáng thứ 7" | **Có**, cho bước 1 (LMS) và bước 4 (gộp, nhắc hạn) |
| **Workflow** | Các bước cố định: Rule lấy lịch LMS → sinh viên dán/forward tin nhắn, email dặn dò → **AI trích "môn – bài – hạn – loại (mới / đổi hạn) – câu nguồn"** → Rule so với lịch LMS để gộp trùng, đánh dấu đổi hạn và tạo Daily Digest 22h (≤ 5 dòng) → sinh viên duyệt, bấm xác nhận rồi mới lưu vào lịch | Khi AI trích đúng phần lớn deadline và sinh viên duyệt xong trong 2–3 phút | AI trích sai ngày hoặc bỏ sót tin đổi hạn; digest quá dài gây ngập thông báo; sinh viên quên dán tin nhắn | **✅ Chọn** |
| **Agent** | AI tự đăng nhập LMS, email, Zalo; tự đọc mọi nhóm chat; tự tạo, sửa lịch và tự nhắc | Không cần cho bài này | Cần mật khẩu hoặc quyền đọc toàn bộ Zalo cá nhân, điều sinh viên đã phản bác ở CP4 (giả định #5); AI tự tạo lịch sai thì sinh viên bỏ sót mà không biết | ❌ Không chọn |

**Mức chọn:** **Workflow**, AI chỉ làm 1 bước (trích deadline từ tin nhắn/email dạng văn bản tự do), kết hợp **Rule** cho phần LMS, gộp trùng và nhắc hạn.

**Vì sao không chọn mức đơn giản hơn:**

- **Rule không đủ:** iCal chỉ lấy được bài tập chính thức trên LMS. Theo giả định #2 ở CP4, phần lớn các lần sót lại đến từ **thông báo không có cấu trúc** trong Zalo và email. Bottleneck trong Card #1 cũng là bước đọc Zalo (6 phút/tối, dễ sót tin đổi hạn). Từ khóa cố định không bắt được các cách viết tự do này.
- **No AI không đủ:** checklist và Sheet chung vẫn để sinh viên tự đọc từng nguồn mỗi tối. Đây đúng là việc đang làm, mất ~18 phút/tối, mà 8/10 sinh viên được hỏi vẫn từng bị sót bài.
- **Phần nào Rule làm được thì không dùng AI:** toàn bộ dữ liệu LMS đi qua iCal, không qua AI, theo bài học từ research Canvas iCal ở mục 3.3.

**Vì sao không chọn Agent:** các bước đã biết trước và cố định, không có bước nào cần AI tự quyết làm gì tiếp. Agent còn đòi quyền truy cập tài khoản cá nhân, điều sinh viên đã phản bác ở CP4.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | Từ đoạn tin nhắn hoặc email sinh viên dán vào, tạo danh sách: **môn – bài – hạn (ngày, giờ) – loại (mới / đổi hạn) – câu nguồn trích nguyên văn**. Không xác định được môn hoặc hạn thì ghi "thiếu thông tin" |
| **Judgment** — con người cân nhắc, quyết định gì? | Sinh viên quyết định: mục nào đúng, có đúng là bài của lớp/nhóm mình không, và khi hạn trên LMS khác hạn trong Zalo thì tin theo hạn nào (có thể hỏi lại giảng viên/trợ giảng) |
| **Action** — hành động cuối cùng là gì, ai làm? | Sinh viên bấm xác nhận từng mục, mục đã xác nhận mới được lưu vào lịch cá nhân. Rule nhắc trước hạn 24 giờ. AI không tự tạo, sửa hay xóa lịch |
| **Outcome** — đo kết quả bằng gì? | (1) Thời gian rà soát mỗi tối (baseline ~18 phút); (2) số deadline bị sót mỗi tháng (baseline ~1); (3) tỉ lệ mục trong digest sinh viên phải sửa |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | (1) Văn bản tin nhắn Zalo/email do sinh viên **tự chọn và dán vào**: có sẵn, nhưng sinh viên phải thao tác vì Zalo hạn chế API cho tài khoản cá nhân (mục 3.3); (2) **ngày gửi tin**, để quy đổi "thứ 6 tuần sau" ra ngày cụ thể: có sẵn; (3) **danh sách môn đang học**: có sẵn; (4) **lịch LMS từ iCal**, để gộp trùng và phát hiện đổi hạn: có sẵn. Chưa hỗ trợ: ảnh chụp màn hình, slide (ngoài phạm vi) |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Các mục sinh viên sửa, xóa hoặc tự thêm khi duyệt digest; các deadline bị sót phát hiện sau đó (ghi lại tin nguồn). Mỗi tuần dùng các lỗi lặp lại để chỉnh hướng dẫn (prompt) và danh sách từ khóa của Rule |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
  - **Augment**, nhưng giảm tối đa thao tác. Sinh viên **không muốn giao hẳn**: ở CP4 có ý kiến phản bác việc cấp quyền đọc toàn bộ Zalo cá nhân, và 2/8 sinh viên muốn bản tóm tắt dưới 5 dòng để tự xem. Họ cũng **không muốn tự gõ tay** từng bài (workaround hiện tại là chụp màn hình hoặc tự ghi sổ, rồi bị sai khi đổi hạn).
  - Vì vậy thiết kế để AI làm phần đọc và trích, còn sinh viên giữ quyền xác nhận trong 2–3 phút mỗi tối. Giả định "sinh viên chịu duyệt 2–3 phút mỗi tối" (giả định #3, bằng chứng 3/5) cần được đo trong pilot.
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:
  - **Bỏ sót tệ hơn.** Một deadline hay một tin đổi hạn bị bỏ sót nghĩa là sinh viên nộp trễ hoặc mất điểm, đúng là pain gốc. Báo nhầm thì sinh viên thấy ngay khi duyệt và xóa được.
  - **Nhưng báo nhầm quá nhiều cũng nguy hiểm.** Ở CP4, sinh viên phản bác rằng digest ngập tin rác thì họ sẽ tắt thông báo, và khi đó lại dẫn tới bỏ sót.
  - **Thiết kế:** AI phải liệt kê cả mục chưa chắc (nhãn "cần xác nhận") thay vì tự bỏ. Mọi tin đổi hạn hiện cả hạn cũ (LMS) và hạn mới. Rule gộp trùng với lịch LMS, và digest giới hạn ≤ 5 dòng, chỉ gồm deadline trong 7 ngày tới.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | Sinh viên học 4–6 môn/kỳ, phải theo dõi bài tập từ ít nhất 3 kênh (LMS, email trường, nhóm Zalo lớp/môn, Drive) |
| **Quy trình** | Mỗi tối: mở LMS xem bài mới (3') → kiểm tra email trường (2') → đọc các nhóm Zalo lớp/môn (6') → xem Drive/tài liệu (3') → ghi deadline vào sổ/ghi chú (4'); khoảng 18 phút/tối, 5/5 bước thủ công |
| **Bottleneck** | Bước đọc nhóm Zalo (~6 phút/tối): thông báo bài tập và tin đổi hạn bị lẫn trong tin trò chuyện, viết dạng tự do, dễ trôi và dễ sót |
| **Impact** | ~18 phút/tối ≈ 1,8 giờ/tuần cho mỗi sinh viên; sót ~1 deadline/tháng và bị trừ điểm. Kiểm chứng: 8/10 sinh viên ngoài nhóm từng bị sót bài tập; 6/8 sinh viên trong micro survey từng sót hoặc suýt trễ deadline trong tháng trước; 7/8 phải theo dõi từ 3 nguồn trở lên |
| **Success Metric** (baseline → target, cách đo) | **Thời gian:** rà soát bài tập mỗi tối từ ~18 phút xuống dưới 5 phút. **Kết quả:** số deadline bị sót từ ~1/tháng xuống 0 trong 4 tuần. **Chất lượng:** không quá 10% mục trong digest phải sửa. **Cách đo:** 3–5 sinh viên pilot tự bấm giờ mỗi tối và ghi vào bảng theo dõi; cuối mỗi tuần đối chiếu danh sách đã xác nhận với LMS và thông báo gốc để đếm deadline bị sót và số mục phải sửa |
| **Boundary** | AI chỉ xử lý văn bản do sinh viên **chủ động dán hoặc forward**; không đăng nhập, không đọc tài khoản Zalo, email hay LMS. AI không tự tạo, sửa, xóa lịch và không tự gửi nhắc. Khi nguồn không rõ môn hoặc hạn thì ghi "thiếu thông tin", không suy đoán. Khi hạn LMS và hạn trong tin nhắn khác nhau thì hiện cả hai, để sinh viên quyết định. Sinh viên xác nhận từng mục trước khi lưu vào lịch (HITL) |
| **AI intervention point** | Duy nhất bước trích deadline từ tin nhắn/email dạng văn bản tự do. Phần LMS do Rule (iCal) xử lý, không qua AI |
| **Mức chọn** | **Workflow** (AI ở 1 bước) + **Rule** (iCal LMS, gộp trùng, nhắc hạn 24 giờ) |
| **Rủi ro & người kiểm tra** | **Rủi ro:** AI bỏ sót hoặc trích sai hạn, nhất là tin đổi hạn; sinh viên quên dán tin nhắn; lộ nội dung chat của lớp khi dán vào dịch vụ AI. **Người kiểm tra:** chính sinh viên khi duyệt digest 22h, đối chiếu câu nguồn. **Khi AI sai hoặc không dùng được:** quay về checklist 4 nguồn thủ công; lịch LMS từ iCal vẫn chạy bình thường |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | Sinh viên phải theo dõi bài tập từ nhiều kênh | Sinh viên học 4–6 môn/kỳ, theo dõi từ ít nhất 3 kênh | Phản biện v0: actor quá rộng; CP4 có 1/8 sinh viên chỉ cần xem LMS nên không gặp pain này |
| Success Metric | Thời gian 18 → < 5 phút/tối; deadline bị sót ~1/tháng → 0 trong 4 tuần | Thêm metric chất lượng: ≤ 10% mục trong digest phải sửa; cách đo cụ thể với 3–5 sinh viên pilot | Phản biện v0: nhanh hơn mà phải sửa nhiều thì không đạt; cần đo chất lượng đầu ra của AI |
| Boundary | AI không đọc tài khoản Zalo/email; không tự tạo lịch, không tự gửi nhắc; sinh viên xác nhận trước khi lưu | Thêm: AI chỉ xử lý văn bản sinh viên tự dán; nguồn thiếu thông tin thì không suy đoán; hạn LMS và hạn trong tin nhắn khác nhau thì hiện cả hai | PAIR (6.4): bỏ sót và đoán sai hạn là kiểu sai tệ nhất; tiêu chí eval #3, #4 cần boundary này |
| AI intervention point | (chưa có) | Chỉ bước trích deadline từ tin nhắn/email tự do; LMS đi qua Rule (iCal) | So sánh 4 mức (6.2) và research Canvas iCal (3.3): phần LMS có cấu trúc, Rule chính xác hơn và không tốn chi phí |
| Mức chọn, Rủi ro & người kiểm tra | (chưa có) | Workflow + Rule; sinh viên kiểm tra khi duyệt digest; quay về checklist 4 nguồn khi AI sai | Kết quả phân tích CP6 |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | Không bỏ sót | Mọi bài tập/deadline có trong đoạn tin nhắn dán vào đều xuất hiện trong danh sách (kể cả dưới nhãn "cần xác nhận") | Có ít nhất 1 deadline trong nguồn không xuất hiện trong danh sách |
| 2 | Đúng hạn | Ngày giờ khớp nguồn; cách nói tương đối được quy đổi đúng theo ngày gửi tin ("thứ 6 tuần sau" → đúng ngày) | Sai ngày/giờ, quy đổi sai, hoặc AI tự đặt hạn |
| 3 | Phát hiện đổi hạn | Tin đổi hạn được gắn nhãn "đổi hạn" và hiện cả hạn cũ (LMS) lẫn hạn mới | Tin đổi hạn bị coi là bài mới, hoặc ghi đè hạn cũ mà không báo |
| 4 | Không bịa, có nguồn | Mỗi mục kèm câu nguồn trích nguyên văn; nguồn thiếu môn hoặc hạn thì ghi "thiếu thông tin" | Có mục không truy được về câu nguồn, hoặc AI tự điền thông tin không có trong nguồn |
| 5 | Digest gọn | Tối đa 5 dòng, chỉ gồm deadline trong 7 ngày tới, không chứa tin trò chuyện | Quá 5 dòng, lặp mục đã có trong LMS, hoặc lẫn tin không phải bài tập |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | **TB** | Pain có bằng chứng từ người thật: 8/10 sinh viên ngoài nhóm từng bị sót bài tập; 6/8 trong micro survey từng sót hoặc suýt trễ trong tháng trước; 7/8 theo dõi từ 3 nguồn trở lên. Vẫn để TB vì câu hỏi khảo sát còn chung chung ("có bị sót không"), chưa đo thời gian của người ngoài nhóm, và có tín hiệu phản bác (1/8 chỉ cần xem LMS; 2/10 tự kiểm tra thường xuyên nên ít bị sót) |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | **TB** | Đầu ra ngắn, có câu nguồn nên dễ đối chiếu và sửa. Nhưng sinh viên phải tự dán tin nhắn; CP4 cho thấy sinh viên ngại nhập tay và hay quên khi mệt. Giả định "chịu duyệt 2–3 phút mỗi tối" chưa được đo |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | **Thấp** | iCal feed LMS có sẵn (mục 3.3); trích deadline từ văn bản bằng trợ lý AI phổ thông là pattern đã có (n8n, mục 3.3); Google Calendar/Sheet miễn phí. Không cần lập trình phức tạp cho pilot. Zalo hạn chế API nên dùng cách dán thủ công |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | **TB** | Chi phí gần như 0 (gói miễn phí). Không truy cập tài khoản cá nhân. Tuy vậy, tin nhắn nhóm lớp có nội dung của người khác, nên chỉ dán phần thông báo bài tập, không dán thông tin cá nhân. Mỗi sinh viên tự vận hành cho mình, không cần trường hay lớp duy trì |

### 8.2. Kết luận

**Quyết định:** **Go (phạm vi nhỏ)**

**Lý do:** Không có rủi ro nào ở mức Cao. Value đã có bằng chứng từ 18 sinh viên (10 + 8). Feasibility thấp vì dùng công cụ có sẵn. Usability và Viability ở mức TB, đã có biện pháp: boundary, HITL qua digest, phương án quay về. Vì vậy nhóm **không tự xây ứng dụng** mà pilot bằng công cụ có sẵn trong một quy trình bán thủ công.

**Nếu Go — pilot nhỏ nhất:** 3–5 sinh viên trong 1 lớp, 2 tuần. (1) Đăng ký iCal feed LMS vào Google Calendar. (2) Mỗi tối, sinh viên dán các tin nhắn/email dặn dò trong ngày vào trợ lý AI với một prompt cố định, nhận danh sách theo đúng 5 tiêu chí ở mục 7. (3) Sinh viên duyệt, rồi tự thêm các mục đã xác nhận vào Calendar. (4) Ghi thời gian, số mục phải sửa và số deadline bị sót vào bảng theo dõi.

**Nếu Not Yet — cần kiểm chứng gì trước:** Không áp dụng. Song song với pilot, nhóm vẫn phỏng vấn thêm 2–3 sinh viên ngoài nhóm theo The Mom Test ("lần gần nhất bạn sót bài là khi nào, vì sao, đang xử lý thế nào") để củng cố bằng chứng Value.

**Nếu No-Go — nên làm gì thay AI:** Không áp dụng. Nếu chạm ngưỡng dừng, dùng phương án No AI + Rule: iCal LMS + Google Sheet deadline chung của lớp do lớp trưởng cập nhật + nhắc hạn tự động.

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

Nếu sau **2 tuần pilot** xảy ra **một trong các điều sau**, nhóm dừng bước AI và quay về **iCal LMS + Google Sheet deadline chung của lớp + checklist 4 nguồn** (No AI + Rule):

- thời gian rà soát vẫn **≥ 10 phút/tối**;
- có **≥ 1 deadline bị sót** do AI trích thiếu mà sinh viên không phát hiện khi duyệt;
- sinh viên phải sửa **> 30% mục** trong danh sách;
- **quá một nửa** sinh viên pilot bỏ bước dán tin nhắn từ tuần thứ 2.

---

## 9. Hạn chế và hướng tiếp theo

**Hạn chế:**

- **Phỏng vấn sâu mới thực hiện với thành viên trong nhóm.** 3 snapshot ở CP4 là thành viên nhóm, không đúng yêu cầu của đề. Bằng chứng chính vì vậy dựa vào hai khảo sát với người ngoài nhóm (10 + 8 sinh viên).
- **Câu hỏi khảo sát còn chung chung.** Khảo sát 10 sinh viên chỉ hỏi "có hoàn thành hết bài tập hay bị sót phần nào không", chưa hỏi lần gần nhất, nguyên nhân và thời gian dành cho việc kiểm tra.
- **Số phút từng bước là ước tính** từ trải nghiệm của người đề xuất (Problem Card #1), chưa được bấm giờ thật.
- **Đổi candidate muộn.** Nhóm chọn bài "Theo dõi task nhóm" ở CP3 khi chưa có bằng chứng, đến CP4 mới chốt lại bài deadline, nên phải làm lại CP5–CP6.
- **Phạm vi hẹp:** mới khảo sát sinh viên trong một lớp; chưa xử lý thông báo dạng ảnh chụp màn hình hoặc slide.

**Hướng tiếp theo:**

1. Phỏng vấn 2–3 sinh viên ngoài nhóm theo The Mom Test ("lần gần nhất bạn sót bài là khi nào, vì sao, đang xử lý thế nào") và bấm giờ thật quy trình hiện tại của họ.
2. Chạy pilot 2 tuần với 3–5 sinh viên như mục 8.2, ghi thời gian, số mục phải sửa và số deadline bị sót.
3. Sau pilot, so sánh với ngưỡng dừng ở mục 8.2 để quyết định mở rộng, điều chỉnh hay quay về phương án No AI + Rule.

## 10. Tài liệu tham khảo

- Design Council — [Framework for Innovation (Double Diamond)](https://www.designcouncil.org.uk/resources/framework-for-innovation/)
- Intercom, Alan Klement — [How we accidentally invented Job Stories](https://www.intercom.com/blog/accidentally-invented-job-stories/)
- Teresa Torres — [Opportunity Solution Trees](https://www.producttalk.org/opportunity-solution-trees/); [The Interview Snapshot](https://www.producttalk.org/interview-snapshot/)
- David Bland, Strategyzer — [Assumptions mapping](https://www.strategyzer.com/library/how-assumptions-mapping-can-focus-your-teams-on-running-experiments-that-matter)
- Rob Fitzpatrick — [The Mom Test](https://www.momtestbook.com/)
- Jeff Gothelf — [Business Problem vs Opportunity Statements](https://jeffgothelf.com/blog/business-problem-statement-opportunity-statement/)
- Google PAIR — [People + AI Guidebook: User Needs](https://pair.withgoogle.com/chapter/user-needs/)
- Anthropic — [Building effective agents](https://www.anthropic.com/research/building-effective-agents)
- Agrawal, Gans, Goldfarb — [A Simple Tool to Start Making Decisions with the Help of AI (HBR)](https://hbr.org/2018/04/a-simple-tool-to-start-making-decisions-with-the-help-of-ai)
- Marty Cagan, SVPG — [The Four Big Risks](https://www.svpg.com/four-big-risks/)
- Các công cụ đã research ở mục 3.3: Canvas LMS Calendar Feed (iCal), Motion, n8n (link trong bảng research)
