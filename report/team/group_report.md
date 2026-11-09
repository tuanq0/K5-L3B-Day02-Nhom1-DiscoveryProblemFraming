# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

* Tên nhóm: Nhóm 1

* Thành viên: Đào Hồng Thắng, Nguyễn Trung Dũng, Trần Văn Tuấn, Nguyễn Quốc Toàn, Bùi Phước Anh

* Candidate problem được chọn (1 câu): Tự động hóa quá trình phân loại, tổng hợp dữ liệu ticket từ Intercom thành báo cáo Voice of Customer (VoC) hàng tuần cho Product Manager (PM).

* Quyết định cuối: Go

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| \# | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) | 
| ----- | ----- | ----- | ----- | ----- | ----- | 
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
|---|---|---|
| A. Điền dữ liệu vào đầu ra có cấu trúc | #1 Điền dữ liệu Excel vào template banner | Chuyển dữ liệu có sẵn theo từng dòng vào một mẫu cố định; trọng tâm là giảm thao tác copy/paste và tạo đầu ra đồng nhất. |
| B. Ghi nhận và đối soát giao dịch cá nhân | #2 Theo dõi thu chi<br>#14 Đối chiếu giao dịch giữa các nguồn tiền | Ghi nhận, phân loại hoặc đối chiếu giao dịch từ nhiều nguồn để có bức tranh chi tiêu đầy đủ; rủi ro là quên giao dịch nhỏ hoặc lệch số dư. |
| C. So sánh chi phí để ra quyết định mua | #3 Mua sản phẩm giá trị lớn/trả góp | Tổng hợp giá, lãi suất, phí và điều kiện từ nhiều nguồn để so sánh nghĩa vụ thanh toán trước khi quyết định. |
| D. Tổng hợp kiến thức phục vụ ôn tập | #5 Tổng hợp nội dung ôn thi<br>#8 Tổng hợp kiến thức học phần | Lọc và hệ thống hóa kiến thức từ sách, giáo trình, slide hoặc ghi chép; cần đảm bảo nội dung trọng tâm không bị thiếu hoặc sai lệch. |
| E. Theo dõi trạng thái học tập của con | #6 Theo dõi nội dung học và bài tập chưa nộp | Gom thông tin học tập đang phân tán để phụ huynh nắm tiến độ mà không phải hỏi nhiều kênh; cần cân bằng khả năng theo dõi với sự riêng tư/tự chủ của trẻ. |
| F. Cập nhật tình trạng giao thông để chọn tuyến | #4 Tra cứu thời gian xe buýt đến<br>#7 Chọn tuyến ít ùn tắc<br>#9 Tìm tuyến tránh ngập | Dựa vào thông tin vị trí/tình trạng đường có tính thời điểm để quyết định chờ hay chọn tuyến; độ mới và độ tin cậy của dữ liệu ảnh hưởng trực tiếp đến quyết định. |
| G. Phân tích tín hiệu khách hàng cho CS/PM | #10 Tổng hợp báo cáo VoC tuần<br>#11 Tóm tắt lịch sử hỗ trợ khách VIP | Đọc dữ liệu hội thoại để rút ra vấn đề hoặc bối cảnh cần thiết cho nhân viên; cần giữ được chi tiết quan trọng và khả năng truy vết về nguồn. |
| H. Phát hiện sự cố và chuyển cảnh báo | #12 Phát hiện lỗi diện rộng, cảnh báo Tech | Phát hiện mẫu bất thường từ nhiều báo cáo theo thời gian gần thực và chuyển cảnh báo đúng lúc; cần hạn chế bỏ sót sự cố lẫn cảnh báo giả. |
| I. Hiểu thay đổi và xử lý xung đột trong cộng tác code | #13 Review PR có phần code chồng lấn | Reviewer cần hiểu logic thay đổi và vùng overlap để đưa ra quyết định an toàn; thời gian tăng khi PR có conflict. |
| J. Phối hợp lịch nhóm | #15 Thống nhất lịch họp học tập | Thu thập khả năng tham gia từ nhiều người, xử lý lịch trùng và chờ xác nhận; điểm nghẽn là phản hồi chậm và thay đổi sát giờ. |



### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: Giảm thiểu tối đa thời gian và công sức lãng phí khi phải thu thập, đối chiếu và xử lý thông tin phân tán để ra quyết định nhanh hơn.
├── Opportunity A: Cần loại bỏ các thao tác sao chép, đối soát và phân loại dữ liệu thủ công lặp đi lặp lại (Bao hàm Cluster A, B, G).
├── Opportunity B: Cần rút ngắn thời gian đọc hiểu và chắt lọc thông tin cốt lõi từ nhiều nguồn nội dung dài/phức tạp (Bao hàm Cluster C, D, I).
├── Opportunity C: Cần nắm bắt sự kiện, tình trạng biến động theo thời gian thực để phản ứng/ra quyết định kịp thời (Bao hàm Cluster F, H).
└── Opportunity D: Cần giảm độ trễ và sự phụ thuộc khi phải thu thập, thống nhất thông tin từ nhiều người khác (Bao hàm Cluster E, J).

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

* "Cần một công cụ tự động điền file Excel vào mẫu Canva" -> Đây là giải pháp (Workflow/Script). Nhu cầu thực sự là giải quyết nỗi đau mất thời gian copy-paste lặp lại.
* "Cần dùng AI để tóm tắt lịch sử chat VIP" -> Đây là giải pháp (LLM). Nhu cầu thực sự là cần nắm bắt nhanh bối cảnh mà không phải đọc thủ công tài liệu dài.
* "Cần hệ thống tự động bắn cảnh báo lỗi sang Slack cho Tech" -> Đây là tính năng (Alerting system). Nhu cầu thực sự là giảm độ trễ trong việc nhận diện điểm bất thường (pattern) khi có sự cố.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| 1. Điền template banner (Thắng) | 4 | 5 | 3 | 4 | 5 | 2 | 4 | **27** |
| 2. Review Pull Request (Dũng) | 5 | 3 | 3 | 4 | 2 | 4 | 5 | **26** |
| 3. Dự đoán giờ xe buýt (Tuấn) | 5 | 2 | 3 | 3 | 1 | 2 | 3 | **19** |
| 4. Tìm đường tránh ngập (Toàn) | 5 | 3 | 3 | 3 | 1 | 3 | 4 | **22** |
| **5. Báo cáo VoC tuần (Anh)** | **5** | **5** | **4** | **5** | **4** | **5** | **4** | **32** |

**Candidate được chọn:** Báo cáo VoC tuần (Phước Anh).

**Vì sao chọn:** Bài toán đại diện tốt nhất cho Opportunity 1. Nó có quy trình AS-IS rõ ràng, lặp lại cố định vào thứ Sáu; trigger và outcome được định nghĩa chắc chắn (Đầu vào: CSV Intercom, Đầu ra: Docs). Thời gian nghẽn đo lường được rõ ràng (bottleneck khoảng 60-80 phút). Quan trọng nhất, bài toán được đóng khung gọn trong tác vụ xử lý text, cực kỳ phù hợp với năng lực của LLM hiện tại và vừa sức để làm pilot nghiệm thu (UAT) ngay trong Lab.

**Vì sao loại các candidate còn lại:**
- **Dự đoán xe buýt & Tìm đường tránh ngập:** Đòi hỏi thu thập dữ liệu thời gian thực (real-time GPS, bản đồ kẹt xe, cảm biến ngập), phụ thuộc vào API bên thứ 3 và môi trường vật lý. Điều này vượt quá phạm vi khả thi và nguồn lực thời gian của một bài lab.
- **Review Pull Request:** Là một bài toán hay nhưng vướng mắc ở rào cản bảo mật (dữ liệu mã nguồn thuộc private repo của công ty). Rất khó để trích xuất đủ bộ dữ liệu thật (dataset) mang ra thử nghiệm nội bộ trong lab mà không vi phạm quy định.
- **Điền template banner:** Vấn đề này thiên về tự động hóa cấu trúc (Rule-based / Script / Mail merge) hơn là thực sự cần đến sự suy luận phức tạp của AI. Phương án Workflow truyền thống (không AI) đã có thể giải quyết được 80-90% nỗi đau, khiến việc so sánh các mức can thiệp AI bị gượng ép.


## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| \# | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? | 
| ----- | ----- | ----- | ----- | ----- | ----- | 
| 1 | LLM có khả năng đọc hiểu file CSV log chat thô và gán tag chính xác theo taxonomy (bộ thẻ) quy định sẵn của công ty mà không tự bịa tag mới (Hallucination). | Feasibility | 5 | 2 | Có |
| 2 | Trích xuất ngữ cảnh (quote của khách hàng) do AI sinh ra đủ độ sâu, chính xác và đúng trọng tâm để PM tin tưởng ra quyết định mà không cần hỏi lại CS. | Value | 5 | 2 | Có |
| 3 | Việc che giấu/lọc thông tin định danh cá nhân (PII) của khách hàng trước khi đẩy dữ liệu CSV qua API của LLM có thể thực hiện dễ dàng mà không làm mất ngữ cảnh lỗi. | Viability | 5 | 3 | Không |
| 4 | CS Executive có thể dễ dàng đọc duyệt, phát hiện lỗi sai và chỉnh sửa bản nháp báo cáo do AI sinh ra trong thời gian ngắn (<10 phút) thay vì tốn thời gian như tự làm. | Usability | 4 | 3 | Không |
| 5 | Có thể thiết lập một Workflow tự động (qua Make.com/Zapier) nhận file CSV và trả về template Docs mà không đòi hỏi kỹ năng code phức tạp từ team CS. | Feasibility | 4 | 3 | Không |

Giả định nhóm kiểm chứng trong buổi này: Nhóm sẽ ưu tiên kiểm chứng **Giả định #1 (Feasibility)** và **Giả định #2 (Value)**. 
- *Lý do:* Đây là 2 giả định mang rủi ro "sống còn" (leap-of-faith). Nếu AI không thể phân loại tag chính xác hoặc trích xuất bối cảnh (context) bị sai lệch/vô nghĩa, PM sẽ không dùng báo cáo này, dẫn đến toàn bộ giải pháp vô giá trị dù Workflow có mượt mà đến đâu. Nhóm sẽ test thử bằng cách đưa một đoạn CSV log chat (khoảng 20-30 dòng) vào prompt của LLM để đánh giá đầu ra.

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn giả lập Actor (PM & CS Executive) và thử nghiệm prompt nháp.

Interview snapshot:

| Trường | Nội dung | 
| ----- | ----- | 
| Người được hỏi (vai trò, không ghi tên thật) | CS Executive, Product Manager (PM) | 
| Câu nói đáng nhớ nhất (nguyên văn) | "Tôi rất ghét chiều thứ Sáu vì phải ngồi đọc lại cả trăm ticket để gán tag bù do trong tuần bận quá quên tag." | 
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | Tuần trước, CS gửi báo cáo trễ, PM hỏi lại bối cảnh của 2 lỗi nhưng CS không nhớ rõ, phải tra lại lịch sử rất lâu mới trả lời được. | 
| Hiện đang xử lý bằng cách nào (workaround)? | CS xuất file CSV ra Google Sheets, dùng hàm đếm hoặc Pivot table, sau đó lọc đọc lại bằng mắt rồi copy context. Đôi khi quản lý ép KPI gán tag ngay nhưng dễ sót lúc cao điểm. | 
| Mất bao lâu, bao lần? | Mất 120 phút mỗi chiều thứ Sáu. PM phải hỏi lại chi tiết ở 4/5 báo cáo gần nhất. | 
| Insight / opportunity rút ra | Không thể ép quy trình No AI (bắt CS không được quên gán tag) vì không khả thi thực tế. Việc gán tag và viết báo cáo là 2 bottleneck tách biệt nhưng AI có thể giải quyết đồng thời. PM đặc biệt quan tâm "bối cảnh khách nói gì", chứ không chỉ cần đếm số lượng lỗi. | 

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác | 
| ----- | ----- | ----- | ----- | 
| Phỏng vấn | 2 | Xác nhận nỗi đau mất thời gian rà soát tag và sự thiếu hụt bối cảnh trong báo cáo. | (Không có) | 

**Nhóm đã sửa problem thế nào sau kiểm chứng:** Tách rõ 2 yêu cầu bắt buộc đối với đầu ra của AI trong problem statement: (1) Đếm đúng Top 3 tag và (2) Phải trích xuất được nguyên văn bối cảnh (context) cho PM đọc, không chỉ trả về số lượng.

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| **Intercom AI Insights (Native Tool)** | [intercom.com/ai](https://www.intercom.com/ai) | Gán tag trực tiếp ngay khi kết thúc phiên chat (Bước 2). | Tích hợp sẵn (native) trong nền tảng, độ trễ bằng không, không cần trích xuất file. | Thường yêu cầu nâng cấp gói cước Enterprise rất đắt đỏ; khó tùy biến format báo cáo (template) theo ý thích riêng của PM. | Việc thiết kế một Workflow linh hoạt đẩy dữ liệu từ bên ngoài (thông qua CSV/Webhook) sẽ tối ưu chi phí và dễ tùy biến đầu ra hơn công cụ gốc. |
| **Upload CSV trực tiếp lên ChatGPT/Claude** | [chatgpt.com](https://chatgpt.com) | Đọc file, phân loại tag, đếm số lượng và sinh nội dung báo cáo (Bước 2, 3, 4, 5). | Rất dễ sử dụng, chi phí thấp, thao tác prompt linh hoạt để điều chỉnh nhanh bộ taxonomy. | Phải upload thủ công mỗi tuần. Có rủi ro cao về rò rỉ dữ liệu cá nhân (PII) của khách hàng nếu dùng bản web. Format đầu ra đôi khi không nhất quán giữa các lần chat. | Rất tốt để dùng làm môi trường kiểm thử prompt (few-shot prompting) trước. Cần có bước tiền xử lý (xóa cột tên, email, sđt) trước khi đưa dữ liệu cho AI đọc. |
| **Make.com (hoặc Zapier) + OpenAI API** | [make.com](https://www.make.com) | Tự động hóa khâu đọc CSV, gọi AI xử lý và điền vào template Google Docs (Gộp Bước 1 đến 5). | Tự động hóa hoàn toàn luồng chuyển dữ liệu giữa các app mà không cần code (No-code), kết nối trực tiếp được với Docs/Slack. | Dễ bị quá tải giới hạn token (Context Window) nếu file CSV log chat quá nặng, dẫn đến việc AI "quên" dữ liệu hoặc trích xuất context bị sai lệch. | Không nên gom tất cả yêu cầu vào 1 prompt duy nhất. Cần thiết kế workflow chia nhỏ: 1 node LLM chuyên đọc và gán tag, 1 node LLM chuyên trích xuất trích dẫn (quote). |

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ:

```
(1) Export CSV Intercom -> (2) Đọc lướt & gán tag thủ công trên Sheets -> (3) Chạy Pivot Table lấy top 3 -> (4) Copy paste trích dẫn làm context -> (5) Điền Template Docs -> (6) Gửi Slack cho PM.
```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú | 
| ----- | ----- | ----- | ----- | ----- | ----- | 
| 1 | CS | Intercom Log | File CSV | 2-3 phút (hàng tuần) | Khởi đầu quy trình. | 
| 2 | CS | File CSV | Bảng đã gán tag | **60-80 phút** | **Bottleneck 1:** Phải đọc lướt thủ công từng ticket để gán nhãn. | 
| 3 | CS | Bảng gán tag | Top 3 Issue | 5 phút | Pivot table đếm tag. | 
| 4 | CS | Ticket Top 3 | Trích dẫn context | **20 phút** | **Bottleneck 2:** Lọc ngược lại file tìm lý do/ngữ cảnh. | 
| 5 | CS | Data tổng hợp | File báo cáo Docs | 10 phút | Trình bày format. | 
| 6 | CS | File Docs | Tin nhắn Slack | 1 phút | Gửi PM. | 

**Bottleneck chính:** Bước 2 (Đọc lướt & gán tag thủ công trên Sheets mất 60-80 phút) và Bước 4 (Lọc tìm ngữ cảnh mất 20 phút).

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```
[Con người] Xuất CSV -> [AI Workflow] Đọc log, phân loại Tag, đếm Top 3, trích xuất Quote & Sinh nháp báo cáo Docs -> [Con người (HITL)] Đọc duyệt và sửa nội dung bản nháp -> [Rule] Đẩy báo cáo cuối cùng qua Slack cho PM.
```
* **Boundary:** AI không được tự động gửi thẳng báo cáo cho PM.
* **Phương án quay về:** Nếu AI sinh lỗi hoặc bịa tag quá nhiều, CS hủy bản nháp AI và chạy lại Pivot Table gán tag bằng tay trên Sheets như cũ.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú | 
| ----- | ----- | ----- | ----- | 
| Số bước | 6 bước | 4 bước | Gộp bước gán tag, lọc context và sinh template vào 1 workflow AI. | 
| Tổng thời gian | \~120 phút | < 30 phút | Tiết kiệm khoảng 90 phút mỗi tuần. | 
| Số bước thủ công | 5 bước | 2 bước | CS chỉ cần thao tác xuất dữ liệu và Review bản nháp cuối. | 
| Bottleneck chính | Đọc gán tag (80p) | Khâu Human Review (10p) | Trọng tâm công việc chuyển sang bước kiểm duyệt (Judgment) của CS. | 
| Rủi ro mới phát sinh | \- | AI gán sai tag hoặc bịa tag (Hallucination) | Cần định nghĩa taxonomy cực kỳ chặt chẽ trong system prompt. | 

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung | 
| ----- | ----- | 
| **Actor** | CS Executive và Product Manager (PM) tại một EdTech Startup. | 
| **Quy trình** | Từ lúc kết thúc tuần giao dịch đến khi hoàn thiện và gửi báo cáo VoC cho PM vào chiều thứ Sáu. | 
| **Bottleneck** | CS mất 60-80 phút rà đọc và phân loại dữ liệu phi cấu trúc (ticket text) bằng mắt thường, cộng thêm 20 phút lọc ngược để trích xuất ngữ cảnh. | 
| **Impact** | Gây lãng phí thời gian manual của CS; đồng thời PM thường xuyên thiếu ngữ cảnh thực tế (context) để ra quyết định cải tiến sản phẩm. | 
| **Success Metric** (baseline → target, cách đo) | \- Thời gian làm báo cáo: 120 phút → giảm xuống dưới 30 phút. <br> - Số lần PM nhắn hỏi thêm context: 4 lần/tháng → 0 lần. | 
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | AI chỉ được phép sinh bản nháp báo cáo (Draft). Con người (CS Executive) BẮT BUỘC (Human-in-the-loop) phải đọc duyệt, đối chiếu và chỉnh sửa trước khi cấp quyền gửi sang kênh của PM. | 

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

* **Phản biện từ AI:** Success metric "giảm thời gian xuống 30 phút" là chưa đủ. Báo cáo làm nhanh nhưng chất lượng kém (phân loại sai, ngữ cảnh rác) thì PM cũng sẽ không dùng.
* **Nhóm đồng ý:** Đã bổ sung thêm tiêu chí đánh giá chất lượng (không bịa tag, có trích dẫn thật) vào phiên bản v1 bên dưới.

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô: **Độ phức tạp thấp - Độ mơ hồ cao**.

Vì sao: Quy trình đầu vào/đầu ra cực kỳ rõ ràng, tĩnh (lặp lại cố định vào thứ Sáu hàng tuần nên độ phức tạp quy trình thấp). Tuy nhiên, dữ liệu cần xử lý là ngôn ngữ tự nhiên (log chat của khách hàng), vốn mơ hồ, chứa nhiều ngữ cảnh ẩn, từ lóng và không có quy tắc if-else cố định để lập trình theo kiểu rule-based.

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? | 
| ----- | ----- | ----- | ----- | ----- | 
| **No AI** (sửa quy trình) | Ép KPI bắt buộc CS gán tag chính xác ngay sau khi kết thúc phiên chat. | Khi lượng ticket ít, CS có dư dả thời gian rảnh sau mỗi chat. | Khó khả thi lúc cao điểm, nhân sự hay quên hoặc gán bừa để đạt KPI. | Không | 
| **Rule** | Keyword matching (vd: có chữ "tiền" -> gán tag Billing). | Khi khách hàng dùng chính xác từ khóa định sẵn. | Dễ bắt trượt ý định, phân loại sai nếu khách dùng từ lóng, viết sai chính tả hoặc nói bóng gió. | Không | 
| **Workflow** | Setup luồng: nhận CSV -> LLM đọc hiểu ý định, phân loại & trích xuất quote -> điền nháp Docs -> Human review. | Khi cần tổng hợp tự động văn bản phi cấu trúc và nối chuỗi các công cụ (Intercom, Docs, Slack). | LLM hallucination tự chế ra phân loại tag sai. | **Có** | 
| **Agent** | Agent tự login vào Intercom định kỳ, tự lọc, tự viết và tự gửi cho PM nếu thấy rủi ro cao. | Khi CS không cần kiểm soát bản nháp báo cáo và tin tưởng 100% vào AI. | AI gửi báo cáo sai sự thật làm PM ra quyết định hỏng; vượt thẩm quyền phân quyền dữ liệu. | Không | 

**Mức chọn:** Workflow

**Vì sao không chọn mức đơn giản hơn:** Các giải pháp Rule-based không thể xử lý được ngôn ngữ tự nhiên đa dạng và mơ hồ của khách hàng. No-AI thì không giải quyết triệt để vấn đề mà chỉ đẩy áp lực sang khâu khác trong vận hành.

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung | 
| ----- | ----- | 
| **Prediction** — AI dự đoán / tạo ra gì? | Phân tích và dự đoán intent của đoạn hội thoại để gom vào tag tương ứng; Sinh ra đoạn tóm tắt văn bản và trích xuất câu quote. | 
| **Judgment** — con người cân nhắc, quyết định gì? | CS Executive quyết định xem bản nháp báo cáo có phản ánh đúng cục diện thực tế của tuần qua không trước khi "Duyệt". | 
| **Action** — hành động cuối cùng là gì, ai làm? | Sinh ra tài liệu Báo cáo VoC hoàn chỉnh và kích hoạt trigger gửi đi qua Slack (Workflow Automation thực hiện). | 
| **Outcome** — đo kết quả bằng gì? | PM nắm được bức tranh tổng thể kèm bối cảnh sâu sát; CS tiết kiệm được 90 phút manual mỗi tuần. | 
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | File CSV log chat xuất từ nền tảng Intercom (chứa Text hội thoại, User_ID, Timestamp). Data này luôn có sẵn mỗi tuần. | 
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | Những thẻ tag hoặc đoạn context bị CS sửa lại/xóa bỏ trong bản draft sẽ được thu thập để làm ví dụ few-shot nhằm tối ưu prompt cho tuần sau. | 

### 6.4. Hai câu hỏi của Google PAIR

* Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng: Người dùng muốn được **hỗ trợ (Augment)** ở khâu lao động chân tay (đọc hàng trăm dòng text, đếm, lọc dữ liệu), nhưng con người (CS) vẫn muốn giữ thẩm quyền kiểm soát và chốt báo cáo cuối cùng trước mặt PM (Judgment).
* AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào: **Bỏ sót** nguy hiểm hơn. Nếu AI bỏ sót các ticket khiếu nại về một lỗi nghiêm trọng, PM sẽ đánh giá sai ưu tiên sửa lỗi, ảnh hưởng đến trải nghiệm người dùng diện rộng. Thiết kế HITL (con người rà soát draft) giúp CS có thể đối chiếu chéo nhanh chóng số lượng dòng tag của bản nháp so với cảm nhận thực tế khi chat trong tuần.

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung | 
| ----- | ----- | 
| **Actor** | CS Executive và Product Manager (PM) tại EdTech Startup. | 
| **Quy trình** | Từ lúc kết thúc tuần giao dịch đến khi hoàn thiện báo cáo VoC gửi cho PM. | 
| **Bottleneck** | CS mất 60-80 phút rà đọc, phân loại dữ liệu phi cấu trúc bằng mắt thường và 20 phút lọc ngược để trích xuất ngữ cảnh. | 
| **Impact** | Lãng phí nguồn lực manual của CS; PM thiếu context để ra quyết định cải tiến sản phẩm chính xác. | 
| **Success Metric** (baseline → target, cách đo) | \- Thời gian làm báo cáo giảm từ 120 phút → dưới 30 phút. <br> - Số lần PM nhắn hỏi thêm context giảm từ 4 lần/tháng → 0 lần. | 
| **Boundary** | AI chỉ được sinh bản nháp báo cáo (Draft). Con người (CS) BẮT BUỘC (HITL) phải đọc duyệt trước khi cấp quyền gửi. | 
| **AI intervention point** | Khâu đọc hiểu text ticket, phân loại intent vào các bucket (tag) có sẵn, đếm số lượng và trích xuất câu quote tiêu biểu. | 
| **Mức chọn** | Workflow | 
| **Rủi ro & người kiểm tra** | Rủi ro lớn nhất là AI bịa tag mới (Hallucination) hoặc lấy sai ngữ cảnh. CS Executive là người chịu trách nhiệm kiểm duyệt trực tiếp bản nháp. | 

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi | 
| ----- | ----- | ----- | ----- | 
| Bottleneck | Mô tả chung chung việc đọc lướt | Chia rõ rà đọc (mất 80p) và lọc ngược tìm context (mất 20p) | Để xác định rõ ràng hai nhiệm vụ riêng biệt mà AI cần xử lý trong prompt. | 
| AI intervention point | (Chưa có) | Thêm rõ "trích xuất câu quote tiêu biểu" | Xác nhận lại insight từ phỏng vấn PM: bối cảnh (quote thật) quan trọng ngang với số đếm. | 

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| \# | Tiêu chí | Đạt khi | Không đạt khi | 
| ----- | ----- | ----- | ----- | 
| 1 | Độ chính xác taxonomy (tag) | 100% tag được AI gán nằm trong bộ Taxonomy quy định sẵn của công ty. | AI tự chế ra tên tag mới không có trong danh sách hoặc để trống tag. | 
| 2 | Khả năng trích xuất ngữ cảnh (Context) | Báo cáo đưa ra được ít nhất 1-2 trích dẫn (quote) tiêu biểu nguyên văn của người dùng cho Top 3 tính năng lỗi. | Báo cáo chỉ đếm số lượng lỗi thuần túy mà không có dẫn chứng văn bản đi kèm. | 
| 3 | Tính nhất quán format (Cấu trúc) | Trả về đúng định dạng Markdown/Cấu trúc Docs thống nhất (VD: Tiêu đề -> Số liệu -> Trích dẫn) hàng tuần. | Vỡ layout, tuần này trả kết quả dạng bảng, tuần sau lại trả dạng gạch đầu dòng lộn xộn. | 

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng | 
| ----- | ----- | ----- | ----- | 
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | Thấp | Thời gian xử lý giảm mạnh từ 120p xuống 30p; PM nhận được context sâu hơn. Đây là lợi ích có thể thấy ngay lập tức. | 
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | Thấp | Đầu ra là một văn bản nháp (Docs) rất quen thuộc. CS hoàn toàn có thể dễ dàng gõ lại/sửa tay/xóa đoạn nếu AI viết sai trước khi chốt duyệt. | 
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | Thấp | Công nghệ Text Classification & Summarization của các LLM hiện nay giải quyết bài toán này cực kỳ tốt. Dữ liệu CSV luôn có sẵn. | 
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | Thấp | Chi phí gọi API LLM xử lý text hàng tuần rất rẻ so với giá trị sức lao động của nhân sự CS. Quy trình cần đảm bảo loại bỏ PII (thông tin định danh khách hàng) ở file CSV trước khi đẩy lên API để tuân thủ bảo mật. | 

### 8.2. Kết luận

**Quyết định:** Go

**Lý do:** Bài toán giải quyết trúng Pain Point tốn kém thời gian của một quy trình định kỳ có tính lặp lại cao. Phạm vi công nghệ yêu cầu hoàn toàn nằm trong điểm rơi năng lực mạnh nhất của LLM hiện tại (xử lý văn bản phi cấu trúc). Hơn nữa, rủi ro về mặt quy trình và trải nghiệm được đóng khung an toàn bởi bước kiểm duyệt HITL (Human-in-the-loop).

**Nếu Go — pilot nhỏ nhất:** Chạy thử nghiệm mù (Shadow testing): CS xuất file CSV log chat của tuần trước, xóa thông tin PII, rồi ném vào prompt LLM (đã custom sẵn taxonomy của công ty). Đối chiếu xem Top 3 lỗi do AI đếm ra có khớp với kết quả thủ công CS đã làm tuần trước không, đồng thời đánh giá chất lượng các câu quote được trích xuất.

**Nếu Not Yet — cần kiểm chứng gì trước:** (Không áp dụng)

**Nếu No-Go — nên làm gì thay AI:** (Không áp dụng)

**Ngưỡng dừng** (nếu sau … mà … thì quay về …): Nếu sau 2 tuần chạy pilot mà tỷ lệ hallucination (AI liên tục bịa ra tag mới không có trong taxonomy) lớn hơn 10%, hoặc trích xuất sai ý khách hàng, dự án sẽ dừng lại và quay về báo cáo bằng rule-based Pivot Table như cũ.

## 9. Hạn chế và hướng tiếp theo

* Cần kiểm tra kỹ khả năng xử lý file CSV dung lượng lớn, đề phòng trường hợp số lượng ticket một tuần quá nhiều vượt qua giới hạn context window của API.
* Cần xây dựng và duy trì một danh sách taxonomy (hệ thống tag) chuẩn nội bộ và cập nhật system prompt liên tục khi có tag mới được thống nhất.

## 10. Tài liệu tham khảo

* Báo cáo cá nhân của 5 thành viên Nhóm 1.