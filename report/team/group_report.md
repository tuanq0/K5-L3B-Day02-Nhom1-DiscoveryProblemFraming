# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

*   Tên nhóm: Nhóm 1
*   Thành viên: Đào Hồng Thắng, Nguyễn Trung Dũng, Trần Văn Tuấn, Nguyễn Quốc Toàn, Bùi Phước Anh
*   Candidate problem được chọn (1 câu): Tự động hóa quá trình phân loại, tổng hợp dữ liệu ticket từ Intercom thành báo cáo Voice of Customer (VoC) hàng tuần cho Product Manager (PM).
*   Quyết định cuối: Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

*Top 3 của Nguyễn Trung Dũng được báo cáo cá nhân ghi là đề xuất tạm thời, cần xác nhận.*

| \# | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
| ---: | --- | --- | --- | --- | --- |
| 1 | Đào Hồng Thắng | Khi làm banner quảng cáo, muốn tự điền nội dung Excel vào template để khỏi copy thủ công. | Người làm banner / người thuê | Tìm ảnh và điền lặp lại; khoảng 1 giờ cho 100 dòng. | Vì sao phải dùng AI thay vì tạo Script/Rule tự động điền template cố định? |
| 2 | Đào Hồng Thắng | Khi phát sinh thu chi hàng ngày, muốn theo dõi đầy đủ để biết tiền được dùng vào đâu. | Bản thân | Có thể quên ghi hoặc ghi thiếu; mỗi lần ghi mất vài phút. | Chưa có thông tin trong báo cáo cá nhân. |
| 3 | Đào Hồng Thắng | Khi cân nhắc mua sản phẩm giá trị lớn/trả góp, muốn hiểu tổng chi phí và nghĩa vụ thanh toán để đánh giá khả năng chi trả. | Bản thân | Phải đọc, tổng hợp giá, lãi suất, phí và điều kiện từ nhiều nguồn; chưa đo thời gian. | Chưa có thông tin trong báo cáo cá nhân. |
| 4 | Trần Văn Tuấn | Khi chờ xe buýt, muốn biết bao giờ xe đến để quyết định tiếp tục chờ hay làm việc riêng. | Người đi xe buýt | Có thể phải đứng chờ đến 30 phút ở bến vắng. | Cách tính toán thời gian thế nào cho hợp lý khi phụ thuộc vào điều kiện giao thông thật? |
| 5 | Trần Văn Tuấn | Khi ôn thi một môn, muốn tổng hợp nội dung cần học để không phải dò từng chương trong sách. | Người học / học sinh ôn thi | Phải tự tìm nội dung liên quan trong sách; báo cáo chưa nêu thời gian cụ thể. | Chưa có thông tin trong báo cáo cá nhân. |
| 6 | Trần Văn Tuấn | Khi con học tiểu học/THCS, phụ huynh muốn biết nội dung học và bài tập chưa nộp để không phải hỏi con hoặc đợi giáo viên nhắn. | Phụ huynh bận đi làm, giáo viên chủ nhiệm | Thông tin phân tán ở nhóm Zalo, sổ liên lạc và lời kể của con. | Chưa có thông tin trong báo cáo cá nhân. |
| 7 | Nguyễn Quốc Toàn | Khi di chuyển giờ cao điểm, muốn biết tuyến đường ít ùn tắc để đến trường/nơi làm đúng giờ. | Sinh viên, người đi làm thường xuyên di chuyển | So sánh tình hình giao thông mất khoảng 5 phút; ùn tắc có thể làm chậm thêm 15–30 phút. | Chưa có thông tin trong báo cáo cá nhân. |
| 8 | Nguyễn Quốc Toàn | Khi ôn thi học phần, muốn tổng hợp kiến thức từ giáo trình, slide và ghi chép để nắm nội dung trọng tâm. | Sinh viên chuẩn bị thi giữa kỳ/cuối kỳ | So sánh và chọn kiến thức trọng tâm mất khoảng 60 phút do tài liệu dài, trùng lặp. | Chưa có thông tin trong báo cáo cá nhân. |
| 9 | Nguyễn Quốc Toàn | Khi di chuyển lúc mưa lớn, muốn biết đoạn đường ngập và tìm tuyến thay thế an toàn để đến nơi đúng giờ. | Sinh viên, người đi làm, người tham gia giao thông | Tìm thông tin đoạn đường ngập mất khoảng 10 phút vì nguồn phân tán/cập nhật chậm. | Làm thế nào để cập nhật chính xác và real-time tình trạng ngập thay đổi liên tục? |
| 10 | Bùi Phước Anh | Khi đến chiều thứ Sáu, muốn có danh sách top 3 tính năng bị phàn nàn nhiều nhất tuần kèm bối cảnh để gửi báo cáo VoC cho PM trước 16h. | CS Executive, PM | Đọc và gắn tag thủ công mất 60–80 phút; trích xuất context thêm khoảng 20 phút. | Làm sao để "dạy" AI hiểu đúng taxonomy (hệ thống tag) của công ty mà không bịa ra tag mới? |
| 11 | Bùi Phước Anh | Khi nhận khiếu nại dài từ khách VIP, muốn tóm tắt lịch sử hỗ trợ để trả lời đúng bối cảnh. | CS Executive hỗ trợ khách VIP | Cuộn đọc lịch sử chat cũ mất khoảng 15–20 phút. | Chưa có thông tin trong báo cáo cá nhân. |
| 12 | Bùi Phước Anh | Khi có nhiều người dùng báo lỗi, muốn Tech nhận cảnh báo kèm pattern lỗi để ưu tiên xử lý kịp thời. | Tech Lead, CS Executive | Nhận ra pattern và báo Tech trễ khoảng 15–20 phút từ lúc lỗi bắt đầu bùng phát. | Chưa có thông tin trong báo cáo cá nhân. |
| 13 | Nguyễn Trung Dũng | Khi review PR của đồng đội, muốn hiểu logic mới và phần code bị chồng lấn để chọn cách triển khai mà không làm hỏng chức năng. | Developer / reviewer | Đọc và so sánh logic, xử lý phần code overlap mất khoảng 10–15 phút với PR conflict. | Vấn đề thực sự nằm ở việc thiếu thông tin logic hay do cách chia module kém? |
| 14 | Nguyễn Trung Dũng | Khi tổng kết chi tiêu, muốn đối chiếu giao dịch từ các nguồn tiền để biết số dư và mức chi thực tế. | Cá nhân tự quản lý tài chính | Khó nhớ giao dịch tiền mặt/nhỏ lẻ và đối chiếu; đôi khi lệch hàng trăm nghìn đồng. | Chưa có thông tin trong báo cáo cá nhân. |
| 15 | Nguyễn Trung Dũng | Khi cần họp nhóm học tập, muốn thống nhất lịch phù hợp để mọi người tham gia và tránh hủy sát giờ. | 6 thành viên nhóm học tập | Phản hồi chậm, lịch trùng trong bước hỏi lịch và chốt giờ; chưa đo thời gian. | Chưa có thông tin trong báo cáo cá nhân. |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
| --- | --- | --- |
| A. Điền dữ liệu vào đầu ra có cấu trúc | #1 Điền dữ liệu Excel vào template banner (Đào Hồng Thắng) | Chuyển dữ liệu có sẵn theo từng dòng vào một mẫu cố định; trọng tâm là giảm thao tác copy/paste và tạo đầu ra đồng nhất. |
| B. Ghi nhận và đối soát giao dịch cá nhân | #2 Theo dõi thu chi (Đào Hồng Thắng); #14 Đối chiếu giao dịch giữa các nguồn tiền (Nguyễn Trung Dũng) | Ghi nhận, phân loại hoặc đối chiếu giao dịch từ nhiều nguồn để có bức tranh chi tiêu đầy đủ; rủi ro là quên giao dịch nhỏ hoặc lệch số dư. |
| C. So sánh chi phí để ra quyết định mua | #3 Mua sản phẩm giá trị lớn/trả góp (Đào Hồng Thắng) | Tổng hợp giá, lãi suất, phí và điều kiện từ nhiều nguồn để so sánh nghĩa vụ thanh toán trước khi quyết định. |
| D. Tổng hợp kiến thức phục vụ ôn tập | #5 Tổng hợp nội dung ôn thi (Trần Văn Tuấn); #8 Tổng hợp kiến thức học phần (Nguyễn Quốc Toàn) | Lọc và hệ thống hóa kiến thức từ sách, giáo trình, slide hoặc ghi chép; cần đảm bảo nội dung trọng tâm không bị thiếu hoặc sai lệch. |
| E. Theo dõi trạng thái học tập của con | #6 Theo dõi nội dung học và bài tập chưa nộp (Trần Văn Tuấn) | Gom thông tin học tập đang phân tán để phụ huynh nắm tiến độ mà không phải hỏi nhiều kênh; cần cân bằng khả năng theo dõi với sự riêng tư/tự chủ của trẻ. |
| F. Cập nhật tình trạng giao thông để chọn tuyến | #4 Tra cứu thời gian xe buýt đến (Trần Văn Tuấn); #7 Chọn tuyến ít ùn tắc và #9 Tìm tuyến tránh ngập (Nguyễn Quốc Toàn) | Dựa vào thông tin vị trí/tình trạng đường có tính thời điểm để quyết định chờ hay chọn tuyến; độ mới và độ tin cậy của dữ liệu ảnh hưởng trực tiếp đến quyết định. |
| G. Phân tích tín hiệu khách hàng cho CS/PM | #10 Tổng hợp báo cáo VoC tuần và #11 Tóm tắt lịch sử hỗ trợ khách VIP (Bùi Phước Anh) | Đọc dữ liệu hội thoại để rút ra vấn đề hoặc bối cảnh cần thiết cho nhân viên; cần giữ được chi tiết quan trọng và khả năng truy vết về nguồn. |
| H. Phát hiện sự cố và chuyển cảnh báo | #12 Phát hiện lỗi diện rộng, cảnh báo Tech (Bùi Phước Anh) | Phát hiện mẫu bất thường từ nhiều báo cáo theo thời gian gần thực và chuyển cảnh báo đúng lúc; cần hạn chế bỏ sót sự cố lẫn cảnh báo giả. |
| I. Hiểu thay đổi và xử lý xung đột trong cộng tác code | #13 Review PR có phần code chồng lấn (Nguyễn Trung Dũng) | Reviewer cần hiểu logic thay đổi và vùng overlap để đưa ra quyết định an toàn; thời gian tăng khi PR có conflict. |
| J. Phối hợp lịch nhóm | #15 Thống nhất lịch họp học tập (Nguyễn Trung Dũng) | Thu thập khả năng tham gia từ nhiều người, xử lý lịch trùng và chờ xác nhận; điểm nghẽn là phản hồi chậm và thay đổi sát giờ. |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Tối ưu hóa hiệu suất xử lý thông tin để giảm thời gian lãng phí vào các tác vụ chân tay/chờ đợi.
├── Opportunity A: Giảm thiểu thao tác phân loại, đọc và trích xuất dữ liệu văn bản thủ công định kỳ.
├── Opportunity B: Tăng tốc độ phân tích, đối chiếu logic kỹ thuật giữa các thành viên.
└── Opportunity C: Cung cấp thông tin dự báo môi trường (giao thông, thời tiết) để chủ động lịch trình.
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

*   Sử dụng ứng dụng tránh tắc đường bằng AI
*   Dùng tool báo lỗi tự động

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| Báo cáo VoC (Anh) | 5 | 5 | 5 | 5 | 5 | 5 | 5 | 35 |
| Review PR (Dũng) | 5 | 4 | 5 | 4 | 3 | 4 | 5 | 30 |
| Tránh đường ngập (Toàn) | 5 | 4 | 4 | 4 | 2 | 4 | 4 | 27 |

**Candidate được chọn:** Báo cáo VoC tuần (Phước Anh).

**Vì sao chọn:** Bài toán có quy trình AS-IS cực kỳ rõ ràng, lặp lại cố định vào thứ Sáu; trigger và outcome định nghĩa chắc chắn (Đầu vào: CSV Intercom, Đầu ra: Docs). Thời gian nghẽn đo lường được (bottleneck khoảng 60-80 phút). Đóng khung gọn trong tác vụ xử lý text, rất phù hợp với năng lực LLM và vừa sức làm pilot trong Lab.

**Vì sao loại các candidate còn lại:** Vấn đề đường ngập và xe bus đòi hỏi cơ sở hạ tầng dữ liệu thời gian thực phức tạp, khó test chuẩn xác. Vấn đề Review PR gặp trở ngại khi phải tích hợp vào repo private chứa mã nguồn nhạy cảm của công ty, khó thu thập đủ dataset để test trong ngắn hạn.

**Xử lý bất đồng (nếu có):** Nhóm đồng thuận với ưu tiên chọn bài toán Báo cáo VoC vì tính khả thi và dữ liệu test dễ kiếm.

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| \# | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
| ---: | --- | --- | ---: | ---: | --- |
| 1 | LLM có khả năng đọc nguyên file CSV hội thoại, phân tích intent và gán tag (Bug, UX...) chính xác, không tự bịa tag. | Feasibility | 5 | 2 | Có |
| 2 | Báo cáo tạo ra đủ bối cảnh (trích dẫn khách hàng) để PM tin tưởng mà không cần hỏi lại CS. | Value | 5 | 2 | Có |
| 3 | Có thể kết nối tự động thành Workflow để chạy mỗi thứ Sáu mà không cần CS upload file thủ công. | Feasibility | 4 | 3 | Không |

Giả định nhóm kiểm chứng trong buổi này: Giả định 1 & 2

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
| --- | --- |
| Người được hỏi (vai trò, không ghi tên thật) | CS Executive, Product Manager (PM) |
| Câu nói đáng nhớ nhất (nguyên văn) | "Tôi rất ghét chiều thứ Sáu vì phải ngồi đọc lại cả trăm ticket để gán tag bù do trong tuần bận quá quên tag." |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước, gửi báo cáo trễ, PM hỏi lại bối cảnh của 2 lỗi nhưng không nhớ rõ, phải tra lại lịch sử rất lâu. |
| Hiện đang xử lý bằng cách nào (workaround)? | CS xuất file CSV ra Google Sheets, dùng hàm đếm hoặc Pivot table, sau đó lọc đọc lại bằng mắt rồi copy context. Đôi khi quản lý ép KPI gán tag ngay nhưng dễ sót lúc cao điểm. |
| Mất bao lâu, bao lần? | 120 phút mỗi thứ Sáu. PM hỏi lại 4/5 báo cáo gần nhất. |
| Insight / opportunity rút ra | Không thể ép quy trình No AI (bắt CS không được quên gán tag). Việc gán tag và viết báo cáo là 2 bottleneck tách biệt nhưng có thể để AI giải quyết đồng thời. PM đặc biệt quan trọng "bối cảnh khách nói gì", chứ không chỉ cần đếm số lượng lỗi. |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
| --- | ---: | --- | --- |
| Phỏng vấn | 2 | Xác nhận nỗi đau mất thời gian và thiếu bối cảnh. |  |

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Tách rõ 2 yêu cầu bắt buộc đối với đầu ra của AI: (1) Đếm đúng Top 3 tag và (2) Phải trích xuất được nguyên văn bối cảnh (context) cho PM đọc.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
| --- | --- | --- | --- | --- | --- |
| Zapier / Make.com tích hợp OpenAI | - | Khâu xử lý file CSV và sinh template báo cáo | Tự động hóa hoàn toàn luồng đẩy file, không cần code. | API có giới hạn token nếu ném toàn bộ CSV log chat nặng; dễ bị rớt context. | Cần tạo prompt tách biệt: 1 prompt phân loại, 1 prompt trích xuất context. |
| Intercom Fin AI / AI Insights | - | Trực tiếp gán tag lúc chat. | Native tích hợp, độ trễ thấp. | Thường yêu cầu gói cước Enterprise đắt đỏ; khó custom template báo cáo gửi PM theo format riêng. | Thiết kế workflow linh hoạt từ ngoài qua webhook/CSV rẻ và dễ tuỳ biến hơn. |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text
(1) Export CSV Intercom -> (2) Đọc lướt & gán tag thủ công trên Sheets -> (3) Chạy Pivot Table lấy top 3 -> (4) Copy paste trích dẫn làm context -> (5) Điền Template Docs -> (6) Gửi Slack cho PM.
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
| ---: | --- | --- | --- | --- | --- |
| 1 | CS | Intercom Log | File CSV | 2-3 phút (hàng tuần) |  |
| 2 | CS | File CSV | Bảng đã gán tag | **60-80 phút** | **Bottleneck 1:** Phải đọc lướt thủ công |
| 3 | CS | Bảng gán tag | Top 3 Issue | 5 phút |  |
| 4 | CS | Ticket Top 3 | Trích dẫn context | **20 phút** | **Bottleneck 2:** Lọc ngược tìm lý do |
| 5 | CS | Data tổng hợp | File báo cáo Docs | 10 phút |  |

**Bottleneck chính:** Đọc lướt & gán tag thủ công trên Sheets (60-80 phút).

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text
[Con người] Xuất CSV/Kích hoạt -> [AI Workflow] Đọc, phân loại Tag, Đếm Top 3, Sinh nháp báo cáo -> [Con người (HITL)] Duyệt nội dung -> [Rule] Đẩy qua Slack cho PM.
```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
| --- | ---: | ---: | --- |
| Số bước | 6 bước | 4 bước | Gộp bước gán tag và sinh template |
| Tổng thời gian | ~120 phút | < 30 phút | Tiết kiệm 90 phút |
| Số bước thủ công | 5 bước | 2 bước | Chỉ xuất dữ liệu và Review |
| Bottleneck chính | Đọc gán tag (80p) | AI Processing (1-2p) | Trọng tâm chuyển sang bước Duyệt của CS |
| Rủi ro mới phát sinh | - | AI gán sai tag | Cần định nghĩa taxonomy kỹ trong system prompt |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
| --- | --- |
| **Actor** | CS Executive và PM tại EdTech Startup |
| **Quy trình** | Từ lúc kết thúc tuần giao dịch đến khi gửi báo cáo VoC cho PM. |
| **Bottleneck** | CS mất 60-80 phút rà đọc và phân loại dữ liệu phi cấu trúc (ticket text) bằng mắt thường, 20 phút lọc ngược để trích xuất ngữ cảnh. |
| **Impact** | Tốn thời gian manual của CS; PM thiếu ngữ cảnh để ra quyết định cải tiến sản phẩm. |
| **Success Metric** (baseline → target, cách đo) | - Thời gian làm báo cáo: 120 phút → dưới 30 phút. - Số lần PM nhắn hỏi thêm context: 4 lần/tháng → 0 lần. |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ sinh bản nháp báo cáo (Draft). Con người (CS Executive) BẮT BUỘC (HITL) phải đọc duyệt, chỉnh sửa trước khi cấp quyền gửi sang kênh của PM. |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

*   Success metric "giảm thời gian xuống 30 phút" hơi chủ quan. Cần định nghĩa rõ chất lượng báo cáo đầu ra. -> Đồng ý. Đã thêm tiêu chí về trích xuất context.

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: Độ phức tạp thấp - Độ mơ hồ cao.

Vì sao: Quy trình đầu vào/đầu ra cực kỳ rõ ràng, tĩnh (cố định vào thứ Sáu) nhưng dữ liệu cần xử lý là ngôn ngữ tự nhiên (log chat khách hàng), vốn mơ hồ, nhiều ngữ cảnh và không có quy tắc if-else cố định để lập trình rule-based.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
| --- | --- | --- | --- | --- |
| **No AI** (sửa quy trình) | Ép KPI bắt buộc CS gán tag chính xác ngay sau khi kết thúc phiên chat. | Khi CS có dư dả thời gian sau mỗi chat. | Khó khả thi lúc cao điểm, hay quên tag. | Không |
| **Rule** | Keyword matching (vd: có chữ "tiền" -> tag Billing). | Khi khách hàng dùng chính xác từ khóa định sẵn. | Dễ bắt trượt ý định, phân loại sai nếu khách dùng từ lóng, viết sai chính tả. | Không |
| **Workflow** | Setup luồng: nhận CSV -> LLM đọc hiểu ý định, phân loại & trích xuất -> điền nháp Docs -> Human review. | Khi cần tổng hợp tự động và nối chuỗi các công cụ (Intercom, Docs, Slack). | LLM hallucination tự chế ra phân loại sai. | Có |
| **Agent** | Agent tự login vào Intercom định kỳ, tự lọc, tự gửi cho PM nếu thấy rủi ro cao. | Khi CS không cần kiểm soát bản nháp báo cáo. | Gửi báo cáo sai sự thật làm PM ra quyết định hỏng; vượt thẩm quyền phân quyền dữ liệu. | Không |

**Mức chọn:** Workflow

**Vì sao không chọn mức đơn giản hơn:** Rule based không xử lý được ngôn ngữ tự nhiên đa dạng của khách hàng.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
| --- | --- |
| **Prediction** — AI dự đoán / tạo ra gì? | Dự đoán (phân loại) intent của hội thoại vào tag tương ứng; Sinh ra đoạn tóm tắt văn bản. |
| **Judgment** — con người cân nhắc, quyết định gì? | CS Executive quyết định xem bản tóm tắt có phản ánh đúng cục diện tuần qua không trước khi chốt. |
| **Action** — hành động cuối cùng là gì, ai làm? | Sinh tài liệu Báo cáo VoC hoàn chỉnh và trigger gửi đi (Automation). |
| **Outcome** — đo kết quả bằng gì? | PM nắm được bức tranh tổng thể kèm bối cảnh thực tế; CS giảm 90 phút manual/tuần. |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | File CSV log chat xuất từ Intercom (chứa Text hội thoại, User_ID, Timestamp). Có sẵn. |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Những tag bị CS sửa lại trong bản draft sẽ được thu thập để tối ưu (few-shot) prompt tuần sau. |

### 6.4. Hai câu hỏi của Google PAIR

*   Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: Muốn được hỗ trợ (Augment) ở khâu lao động chân tay (đọc, đếm, lọc), nhưng con người (CS) vẫn phải giữ thẩm quyền chốt báo cáo cuối cùng trước PM (Judgment).
*   AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: Bỏ sót nguy hiểm hơn. Nếu bỏ sót ticket khiếu nại nghiêm trọng, PM sẽ đánh giá sai ưu tiên sửa lỗi của Product. Thiết kế HITL (con người rà soát draft) giúp CS đối chiếu chéo nhanh chóng số lượng dòng của bản nháp so với CSV gốc.

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
| --- | --- |
| **Actor** | CS Executive và PM tại EdTech Startup |
| **Quy trình** | Từ lúc kết thúc tuần giao dịch đến khi gửi báo cáo VoC cho PM. |
| **Bottleneck** | CS mất 60-80 phút rà đọc và phân loại dữ liệu phi cấu trúc (ticket text) bằng mắt thường, 20 phút lọc ngược để trích xuất ngữ cảnh. |
| **Impact** | Tốn thời gian manual của CS; PM thiếu ngữ cảnh để ra quyết định cải tiến sản phẩm. |
| **Success Metric** (baseline → target, cách đo) | - Thời gian làm báo cáo: 120 phút → dưới 30 phút. - Số lần PM nhắn hỏi thêm context: 4 lần/tháng → 0 lần. |
| **Boundary** | AI chỉ sinh bản nháp báo cáo (Draft). Con người (CS Executive) BẮT BUỘC (HITL) phải đọc duyệt, chỉnh sửa trước khi cấp quyền gửi sang kênh của PM. |
| **AI intervention point** | Khâu đọc hiểu text ticket phi cấu trúc, phân loại intent vào các bucket (tag) có sẵn, và trích xuất câu trích dẫn tiêu biểu. |
| **Mức chọn** | Workflow |
| **Rủi ro & người kiểm tra** | Rủi ro AI bịa tag mới (Hallucination). CS Executive chịu trách nhiệm kiểm duyệt bản nháp. |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
| --- | --- | --- | --- |
| Success metric | Giảm thời gian | Thêm tiêu chí chất lượng context | Báo cáo nhanh nhưng không có ngữ cảnh sẽ vô dụng. |
| Bottleneck | Đọc lướt | Chia rõ rà đọc (80p) và lọc ngược context (20p) | Để xác định rõ task cho AI. |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| \# | Tiêu chí | Đạt khi | Không đạt khi |
| ---: | --- | --- | --- |
| 1 | Độ chính xác tag | 100% tag được gán nằm trong bộ Taxonomy quy định sẵn. | AI tự chế ra tên tag mới hoặc không gán được tag. |
| 2 | Trích xuất ngữ cảnh (Context) | Báo cáo đưa ra được trích dẫn (quote) tiêu biểu của người dùng cho Top 3 tính năng lỗi. | Chỉ đếm số lượng lỗi mà không có dẫn chứng văn bản đi kèm. |
| 3 | Tính nhất quán format | Trả về đúng định dạng Markdown/Cấu trúc Docs thống nhất hàng tuần. | Vỡ layout, tuần này trả bảng, tuần sau trả gạch đầu dòng. |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
| --- | --- | --- | --- |
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Thấp | Thời gian giảm từ 120p xuống 30p; PM nhận được context sâu hơn là lợi ích ngay lập tức. |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Thấp | Đầu ra là văn bản nháp (Docs) quen thuộc, CS dễ dàng gõ lại/sửa tay trước khi chốt. |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | Công nghệ Text Classification & Summarization của LLM hiện tại giải quyết cực tốt. Dữ liệu CSV luôn có sẵn. |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Thấp | Chi phí API rất rẻ so với lương nhân sự CS. Đảm bảo loại bỏ PII (thông tin định danh khách) trước khi đẩy API. |

### 8.2. Kết luận

**Quyết định:** Go

**Lý do:** Bài toán giải quyết trúng Pain Point tốn kém thời gian của một quy trình định kỳ có tính lặp lại cao. Scope công nghệ hoàn toàn nằm trong điểm rơi năng lực của LLM hiện tại. Rủi ro về quy trình và trải nghiệm được đóng khung an toàn bởi bước kiểm duyệt HITL.

**Nếu Go — pilot nhỏ nhất:** Chạy thử nghiệm mù (Shadow testing): CS xuất file CSV của tuần trước ném vào prompt LLM (đã custom taxonomy), đối chiếu xem Top 3 do AI đếm ra có khớp với kết quả thủ công đã làm không. Đánh giá thời gian và chất lượng sinh context.

**Nếu Not Yet — cần kiểm chứng gì trước:** (Không áp dụng)

**Nếu No-Go — nên làm gì thay AI:** (Không áp dụng)

**Ngưỡng dừng** (nếu sau … mà … thì quay về …): Nếu sau 2 tuần pilot mà tỷ lệ hallucination (bịa tag) lớn hơn 10%, quay về rule-based hoặc báo cáo thủ công.

---

## 9. Hạn chế và hướng tiếp theo

*   Cần kiểm tra kỹ khả năng xử lý file CSV dung lượng lớn (nếu số lượng ticket vượt quá context window của LLM).
*   Xây dựng một danh sách taxonomy tag chuẩn và cập nhật liên tục.

## 10. Tài liệu tham khảo

*   Các báo cáo cá nhân của thành viên Nhóm 1.