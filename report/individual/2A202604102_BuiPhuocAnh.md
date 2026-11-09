# Báo cáo cá nhân — 2A202604102_BuiPhuocAnh


## 1. Thông tin học viên
- Họ tên: Bùi Phước Anh
- MSSV: 2A202604102
- Email trường (không bắt buộc, repo có thể để public): cuubui2004@gmail.com
- Tên nhóm: Nhóm 1
- Link repo nhóm:https://github.com/tuanq0/K5-L3B-Day02-Nhom1-DiscoveryProblemFraming/tree/main
---

## 2. Scan problem (CP1)

**Giả định:** Customer Success Executive (CS) ở một startup EdTech khoảng 80 nhân sự, dùng Intercom, Google Sheets và Slack. Mỗi chiều thứ Sáu, người đó phải đọc, phân loại phản hồi từ người dùng (ticket, đánh giá app) để tổng hợp thành báo cáo "Voice of Customer" (VoC) gửi cho Product Manager (PM) và Marketing Lead.

| # | Lăng kính | Job Story | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tới sáng thứ Hai, tôi muốn có số liệu sprint và tình hình team ở một chỗ, để gửi báo cáo tuần cho CEO trước 10h | PM, EM, CEO | Tự bấm giờ 2 tuần gần nhất: 85 và 95 phút |
| 2 | Lặp lại | Khi cập nhật slide cho buổi họp tháng, tôi muốn có sẵn velocity các sprint, để không phải copy tay từ Jira | PM | Mỗi tháng 1 lần, khoảng 20 phút |
| 3 | Tốn thời gian | Khi nhận một PRD 10–15 trang cần review, tôi muốn nắm nhanh các quyết định chính, để comment đúng chỗ trước hạn | PM reviewer, design lead | Khoảng 45 phút/bản, 2 bản/tuần |
| 4 | Tốn thời gian | Khi vừa xong một cuộc họp liên team, tôi muốn có danh sách việc cần làm và người phụ trách, để không ai bỏ sót | PM, team | 30 phút/buổi viết lại ghi chú |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi có quá nhiều task cùng hạn, tôi muốn biết nên làm việc nào trước, để không trễ việc quan trọng | PM, team | Tuần trước trễ 2 task vì ưu tiên sai |
| 6 | Cần đọc, tổng hợp nhiều thông tin | Khi cần biết vì sao team từng chọn phương án A, tôi muốn tìm lại được quyết định cũ, để không tranh luận lại từ đầu | Cả team | 10–15 phút mỗi lần tìm trong Slack, 3–4 lần/tuần |
| 7 | Pain từ người khác | Khi designer nhận spec từ tôi, họ muốn hiểu đúng yêu cầu ngay lần đầu, để không phải hỏi lại | Designer, PM | Designer hỏi lại 2–3 lần/spec (đếm từ thread Slack) |
| 8 | Pain từ người khác | Khi CEO cần chuẩn bị họp leadership sáng thứ Hai, CEO muốn có báo cáo trước giờ họp, để nắm tình hình | CEO, PM | 3/8 tuần gần nhất báo cáo gửi trễ |
| 9 | Tốn thời gian | Khi cuối tháng, tôi muốn có KPI từ nhiều dashboard trong một bảng, để báo cáo tháng | PM, manager | Mỗi tháng khoảng 2 tiếng |
| 10 | Lặp lại | Khi tới giờ standup, tôi muốn có sẵn update hôm qua, để không phải nhớ lại | PM | 5–10 phút/ngày |

**AI gợi ý thêm:** Sau khi tự scan được 7 ý đầu, dùng AI gợi ý và chọn thêm ý #8, #9, #10. Đã loại bỏ ý "Trợ lý AI tự động gọi điện thoại xoa dịu khách hàng giận dữ" vì rủi ro cao đối với trải nghiệm người dùng và vượt quá mức độ tự động hóa mà công ty cho phép hiện tại.


---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Báo cáo VoC tuần (#1, #3, #4) | Quy trình lặp lại hàng tuần rất rõ, tốn nhiều thời gian nhất (khoảng 2 tiếng), bottleneck nằm ở việc đọc và phân loại dữ liệu phi cấu trúc bằng mắt thường. | Khả năng AI phân loại tag (Bug, UX, Pricing...) có nhất quán và chính xác như người làm không? Báo cáo tự động có đủ bối cảnh để PM tin tưởng không? |
| 2 | Tóm tắt lịch sử VIP (#2) | Nỗi đau thật sự vì áp lực thời gian cao (khách đang đợi/giận), tác động trực tiếp đến CSAT (độ hài lòng). | Dữ liệu log chat thường chứa thông tin nhạy cảm (PII). AI tóm tắt có bị sót chi tiết "trọng yếu" dẫn đến việc CS xử lý sai không? |
| 3 | Cảnh báo lỗi cho Tech (#7) | Tác động liên phòng ban (Cross-functional), giải quyết được bài toán phản ứng nhanh, giảm thiểu rủi ro khủng hoảng (crisis). | Khó xác định trigger nào đủ ngưỡng để gọi là "bất thường" (anomaly) thay vì biến động nhỏ, dễ tạo ra cảnh báo rác (spam) làm phiền Tech team. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tới chiều thứ Sáu, tôi muốn có sẵn danh sách top 3 tính năng bị phàn nàn nhiều nhất tuần kèm bối cảnh, để đưa vào báo cáo VoC cho PM trước 16h. |
| Actor | CS Executive và PM. |
| Thời điểm / bối cảnh | Chiều thứ Sáu hàng tuần, lúc cần tổng hợp báo cáo. |
| Quy trình hiện tại (3–7 bước) | 1. Xuất CSV log chat từ Intercom.<br>2. Đọc lướt từng ticket để gắn tag (Bug, UX...).<br>3. Chạy Pivot table đếm tag lấy Top 3.<br>4. Lọc lại ticket của Top 3, copy trích dẫn khách hàng để làm context.<br>5. Viết docs và gửi Slack. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2: Đọc và gắn tag thủ công (mất 60-80 phút). Bước 4: Trích xuất context (20 phút). |
| Impact (nếu không giải thì sao) | CS tốn quá nhiều thời gian manual. PM thường xuyên thiếu bối cảnh để ra quyết định cải tiến sản phẩm. |
| Success metric (baseline → target) | - Thời gian làm báo cáo: 120 phút → dưới 30 phút.<br>- Số lần PM nhắn hỏi thêm context: 4 lần/tháng → 0 lần. |
| Phương án không dùng AI | Ép KPI bắt buộc các bạn CS khác phải gán tag chính xác ngay sau khi kết thúc phiên chat. (Khó khả thi vì lúc cao điểm CS hay quên). |
| Giả thuyết về AI (nếu có) | LLM có khả năng đọc nguyên file CSV hội thoại, phân tích intent và tự động gom nhóm thành Top 3 vấn đề kèm theo 1 đoạn tóm tắt bối cảnh ngắn gọn. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
(1) Export CSV Intercom -> (2) Đọc lướt & gán tag thủ công trên Google Sheets -> (3) Chạy Pivot Table lấy top 3 -> (4) Copy paste trích dẫn làm context -> (5) Điền Template Docs -> (6) Gửi Slack cho PM.
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi nhận một khiếu nại dài từ khách hàng VIP, tôi muốn tóm tắt nhanh lịch sử các lần hỗ trợ trước, để trả lời đúng bối cảnh mà không làm họ cáu thêm. |
| Actor | CS Executive hỗ trợ khách VIP. |
| Thời điểm / bối cảnh | Real-time, ngay khi nhận được tin nhắn từ khách VIP đang giận dữ. |
| Quy trình hiện tại (3–7 bước) | 1. Thấy thông báo ticket VIP nhảy lên.<br>2. Bấm vào profile khách, cuộn đọc lại các ticket cũ.<br>3. Note nháp các mốc thời gian khách từng khiếu nại.<br>4. Quay lại màn hình chat hiện tại và soạn câu trả lời. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2: Cuộn và đọc lướt lịch sử chat dài (mất 15-20 phút tùy lượng data). |
| Impact (nếu không giải thì sao) | Trễ SLA phản hồi (khách VIP ghét chờ đợi). Trả lời sai bối cảnh khiến khách phải lặp lại vấn đề, gây nguy cơ churn (bỏ app). |
| Success metric (baseline → target) | Thời gian nắm bắt bối cảnh trước khi gõ phím: 15 phút → dưới 2 phút. |
| Phương án không dùng AI | Yêu cầu viết "Handoff note" (ghi chú bàn giao) cực kỳ chi tiết sau mỗi lần chat với VIP. |
| Giả thuyết về AI (nếu có) | AI được tích hợp thẳng vào nền tảng chat, chỉ cần bấm nút là tóm tắt toàn bộ lịch sử tương tác thành 3 gạch đầu dòng. |
| Cảm nhận nhanh | Agent / Workflow (tích hợp thẳng tool) |

Quy trình nháp hiện tại:

```text
(1) Nhận chat VIP -> (2) Mở profile khách hàng -> (3) Cuộn đọc thủ công các ticket cũ -> (4) Tổng hợp thông tin ra giấy/note nháp -> (5) Soạn câu trả lời.
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi server có sự cố (user ồ ạt báo lỗi), tôi muốn Tech team nhận cảnh báo ngay kèm pattern lỗi, để ưu tiên xử lý kịp thời. |
| Actor | Tech Lead, CS Executive. |
| Thời điểm / bối cảnh | Bất ngờ, khi có khủng hoảng/lỗi hệ thống (incident). |
| Quy trình hiện tại (3–7 bước) | 1. User bắt đầu nhắn tin báo lỗi ồ ạt.<br>2. CS mải mê trả lời trấn an từng người.<br>3. CS nhận ra "có vẻ đang có lỗi diện rộng".<br>4. CS tạm dừng chat, qua Slack nhắn Tech check.<br>5. Tech vào check log và xác nhận sự cố. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2 & 3: CS nhận ra pattern và báo qua cho Tech (độ trễ khoảng 15-20 phút từ lúc bắt đầu bùng lỗi). |
| Impact (nếu không giải thì sao) | Thời gian downtime kéo dài, hàng trăm user bị ảnh hưởng, uy tín sản phẩm giảm mạnh. |
| Success metric (baseline → target) | Thời gian từ lúc user thứ 5 báo lỗi đến khi Tech nhận cảnh báo: 20 phút → dưới 5 phút. |
| Phương án không dùng AI | Thiết lập Rule: Nếu lượng tin nhắn đến vọt lên gấp 3 lần trung bình thì bắn alert. (Nhược điểm: Chỉ biết là có nhiều tin nhắn chứ không biết có phải lỗi không). |
| Giả thuyết về AI (nếu có) | AI stream data realtime, phân tích keyword tiêu cực ("sập", "lỗi", "không vào được"), tự động gom pattern và bắn Webhook sang Slack cho Tech. |
| Cảm nhận nhanh | Agent / Workflow |

Quy trình nháp hiện tại:

```text
(1) Lượng chat tăng đột biến -> (2) CS loay hoay xử lý -> (3) Nhận diện pattern thủ công (bằng cảm giác) -> (4) Nhắn tin Slack cho Tech -> (5) Tech đi tìm nguyên nhân.
```

### Card muốn pitch nhất

- **Card số:** #1 (Báo cáo VoC tuần)
- **Vì sao:** 
  - Bài toán này có quy trình AS-IS (hiện tại) cực kỳ rõ ràng, lặp lại với tần suất cố định (thứ Sáu hàng tuần).
  - Khởi phát (Trigger) và kết quả (Outcome) đã được định nghĩa chắc chắn (Đầu vào là CSV Intercom, đầu ra là Docs báo cáo). 
  - Nằm hoàn toàn trong vùng kiểm soát (Zone of Control) của CS Executive, dễ dàng tự làm thử nghiệm nghiệm thu (UAT) mà không cần can thiệp quy trình của team khác.
  - Mang lại lợi ích ngay lập tức: giải phóng 2 tiếng đồng hồ mệt mỏi nhất trong tuần của CS.
- **Câu hỏi muốn nhóm phản biện:** 
  - Việc tải CSV lên ChatGPT/Claude thì giải quyết được nhanh, nhưng làm sao để tạo thành một Workflow tự động hóa (ví dụ dùng Make.com) để thứ Sáu nó tự chạy mà CS Executive không cần upload file thủ công?
  - Làm thế nào để "dạy" AI hiểu đúng taxonomy (hệ thống phân loại tag) riêng của công ty mình mà không bịa ra tag mới?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Card #1: Success metric "giảm thời gian xuống 30 phút" hơi chủ quan. Cần định nghĩa rõ chất lượng báo cáo đầu ra. | Đồng ý. Thời gian nhanh nhưng báo cáo rác thì PM cũng không dùng. | Thêm tiêu chí "Báo cáo giữ nguyên hoặc tăng độ chi tiết (PM không phải Slack hỏi lại bối cảnh ở các top issues)". |
| Card #1: Bottleneck gán tag đang bị gom chung với bottleneck viết báo cáo. Thực ra đây là 2 bước tách biệt. | Đồng ý. Việc gán tag bù ở cuối tuần mới là nguyên nhân chính gây tốn thời gian. | Sửa lại quy trình nháp, tách rõ bước 3 (Rà soát và gán tag lại cho ticket) và bước 4 (Tổng hợp text đưa vào Docs). |
| Card #2: Mục tiêu "không làm khách hàng VIP cáu" rất khó đo lường bằng số. | Đồng ý một phần. CSAT đo được nhưng thường có độ trễ. | Đổi Success metric thành "Thời gian phản hồi lại khách hàng (Resolution Time/First Response Time) giảm từ 20 phút xuống dưới 5 phút". |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Trình bày 3 ý tưởng, trong đó nhấn mạnh nhất bài toán: "Tổng hợp, phân loại ticket thành báo cáo VoC tuần cho PM". Phân tích rõ đầu vào (CSV) và đầu ra (Docs). | Thuyết phục được nhóm chọn bài toán này làm Candidate cuối cùng vì có quy trình rõ ràng nhất và tính khả thi cao (Zone of control) để làm lab. |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt cho ý tưởng "Tìm đường tránh ngập" của Toàn: "Làm thế nào để cập nhật chính xác và real-time tình trạng ngập khi thời tiết thay đổi liên tục?" | Giúp nhóm nhận ra rào cản lớn về hạ tầng dữ liệu thời gian thực (real-time data), từ đó đồng thuận loại bỏ các ý tưởng vĩ mô vượt quá sức lab. |
| Nhận phản biện | Câu hỏi tôi nhận được: "Làm sao để 'dạy' AI hiểu đúng taxonomy (hệ thống tag) của công ty mà không bịa ra tag mới (Hallucination)?" | Tôi đã sửa gì: Đưa rủi ro này vào Problem Statement, thêm yêu cầu ép taxonomy cứng vào System Prompt và bắt buộc phải có bước con người kiểm duyệt (Human-in-the-loop) trước khi gửi. |
| Gom cluster / cây OST | Đề xuất gom các bài toán của tôi vào Cluster G (Phân tích tín hiệu khách hàng) và tham gia xây dựng Opportunity B (Rút ngắn thời gian đọc hiểu và chắt lọc thông tin dài/phức tạp). | Giúp nhóm không bị sa đà vào giải pháp (solution-first) mà nhìn nhận đúng bản chất nỗi đau là sự lãng phí thời gian xử lý dữ liệu phi cấu trúc. |
| Chọn candidate problem | Bảo vệ quan điểm chọn bài toán VoC dựa trên tiêu chí "Vừa sức lab" và "Khả năng so sánh các mức AI". | Nhóm thống nhất chấm điểm 35/35 cho bài toán VoC và loại bỏ các bài toán vướng bảo mật code (PR) hay dữ liệu GPS (Xe buýt). |
| Kiểm chứng / research | Tìm hiểu và so sánh công cụ Intercom AI Insights (Native) với phương án ghép nối Zapier/Make.com + OpenAI. Đóng vai thực hiện phỏng vấn giả định CS và PM. | Rút ra bài học: Dùng Workflow (Make + OpenAI) rẻ và dễ tùy biến format báo cáo hơn công cụ native. Nhận ra điểm nghẽn kép (đếm tag và trích xuất ngữ cảnh). |
| Quy trình nhóm | Vẽ quy trình AS-IS (6 bước) và TO-BE (4 bước), bóc tách rõ thời gian bottleneck ở khâu đọc và gán tag thủ công (60-80 phút). | Làm nổi bật được giá trị của AI khi chuyển vai trò của CS từ "người thực thi" (nhập liệu) sang "người kiểm duyệt" (reviewer). |
| Problem Statement | Định nghĩa lại mốc thời gian, impact, và success metric (Giảm thời gian từ 120p xuống 30p; số lần PM hỏi lại bối cảnh về 0). | Đóng khung chặt chẽ bài toán, thiết lập các tiêu chí đánh giá nghiệm thu (Acceptance Criteria) rõ ràng cho khâu test prompt. |
| Mức can thiệp AI | Đánh giá 4 mức độ can thiệp (No AI, Rule, Workflow, Agent) dựa trên ma trận độ phức tạp/mơ hồ và trả lời 2 câu hỏi PAIR. | Chốt phương án Workflow. Bác bỏ phương án Rule (do Text mơ hồ) và phương án Agent (do rủi ro tự động gửi báo cáo sai). |
| Quyết định | Tham gia phân tích 4 rủi ro (Value, Usability, Feasibility, Viability) và đề xuất phương án Shadow Testing (Kiểm thử mù) cho Pilot. | Chốt quyết định "GO" an toàn và có phương pháp luận rõ ràng để mang đi thực hành ở các lab tiếp theo. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Cung cấp 7 vấn đề ban đầu, yêu cầu AI đóng vai CS Manager gợi ý thêm các pain point liên quan đến xử lý ticket và training nhân sự. | Đã gợi ý rất đúng nỗi đau về việc tổng hợp Q&A cho Newbie (ý #9) và trả lời tin nhắn hàng loạt sau khi release app (ý #8). | AI gợi ý một số ý tưởng quá viển vông, ví dụ: "Dùng Voice AI tự động gọi điện xoa dịu khách hàng khi họ tức giận". | Tôi gạch bỏ các ý tưởng có rủi ro cao về trải nghiệm khách hàng (Customer Experience). Chỉ giữ lại những task liên quan đến xử lý text (văn bản) nội bộ. |
| CP2 Problem Card | Yêu cầu AI đóng vai Product Manager khó tính để "bắt lỗi" các Problem Card tôi vừa viết, đặc biệt chú ý vào tính khả thi và cách đo lường. | Chỉ ra được lỗ hổng trong việc gộp chung các bước quy trình (gán tag và viết báo cáo là 2 bottleneck khác nhau), giúp làm rõ bottleneck thực sự. | Khi phản biện Card #2, AI khuyên dùng chỉ số CSAT (Customer Satisfaction Score) để làm Success Metric cho việc tóm tắt log chat nhanh. | Nhận định của tôi là CSAT có độ trễ và phụ thuộc vào kết quả xử lý cuối cùng, không phản ánh ngay việc "đọc log chat nhanh". Tôi tự đổi thành FRT (First Response Time) - thời gian phản hồi đầu tiên. |
| CP4 Research | Yêu cầu AI đóng vai PM để phỏng vấn giả định (Mock Interview) về những gì họ thực sự muốn thấy trong báo cáo VoC; hỏi AI các công cụ tự động hóa Intercom hiện có. | Đã giúp tôi nhận ra PM quan tâm nhiều nhất đến "trích dẫn bối cảnh (context)" chứ không chỉ là con số lỗi đếm được. Gợi ý công cụ Make.com. | AI khuyên nên mua luôn gói Intercom AI Insights (Native Tool) thay vì tự build Workflow bên ngoài. | Tôi bác bỏ vì Intercom AI Insights là bản Enterprise đắt đỏ, không phù hợp với nguồn lực làm lab và khó tùy biến format báo cáo cho PM. Tôi chọn hướng ghép nối Make.com + OpenAI. |
| CP5 Quy trình | Cung cấp quy trình AS-IS (6 bước) và nhờ AI đề xuất cách rút gọn thành TO-BE bằng mô hình LLM. | AI đã gom rất khéo các bước "đọc lướt", "gán tag", "đếm Top 3" và "trích xuất trích dẫn" vào chung 1 node xử lý duy nhất của LLM. | AI đề xuất quy trình tự động hóa 100%: LLM sinh báo cáo xong tự động bắn thẳng qua Slack cho PM mà không cần CS xem lại. | Tôi nhận thấy rủi ro (AI có thể hallucinate bịa ra lỗi sai), nên đã thêm bước "Con người kiểm duyệt (HITL)" vào giữa. CS bắt buộc phải duyệt draft trước khi gửi. |
| CP5–6 Problem Statement | Nhờ AI review lại tiêu chí đánh giá (Acceptance Criteria) cho đầu ra của LLM. | Nhắc nhở tôi về việc AI có thể tự chế ra các thẻ tag không có thật (Ví dụ: tự bịa tag "Lỗi mạng" thay vì dùng tag chuẩn "Connectivity"). | AI viết Problem Statement bằng văn phong quá "marketing", tập trung ca ngợi giải pháp thay vì đóng khung vấn đề kỹ thuật. | Tôi tự viết lại hoàn toàn Problem Statement theo đúng template khắt khe của môn học: Actor rõ ràng, Impact đo lường được, và Boundary (Giới hạn can thiệp) được siết chặt. |
| CP6 Mức can thiệp / quyết định | Đưa thông tin bài toán và nhờ AI đánh giá 4 rủi ro (Value, Usability, Feasibility, Viability) để chốt quyết định Go/No-Go. | AI phân tích rất sắc sảo về rủi ro Viability: Nguy cơ rò rỉ dữ liệu cá nhân (PII) của khách hàng khi ném nguyên file CSV log chat lên OpenAI. | AI đánh giá rủi ro Feasibility (Khả thi) là "Trung bình/Cao" vì cho rằng prompt engineering để trích xuất dữ liệu rất phức tạp. | Tôi hạ mức rủi ro Feasibility xuống "Thấp (An toàn)" vì bài toán phân loại văn bản (Text Classification) hiện tại LLM làm cực kỳ tốt. Để xử lý rủi ro PII, tôi bổ sung phương án làm mờ dữ liệu định danh trước khi gọi API. |

---

## 6. Reflection (CP7)

## 6. Reflection (CP7)

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi nhận ra rằng một "vấn đề tốt" để đưa vào lab không chỉ nằm ở việc nó gây đau đớn (painful) hay có tác động lớn (impactful) đến đâu, mà quan trọng nhất là tính khả thi (feasibility) và vùng kiểm soát (zone of control). Các bài toán của Tuấn và Toàn (dự đoán xe buýt, tránh đường ngập) rất thiết thực nhưng đòi hỏi dữ liệu thời gian thực và phụ thuộc API bên thứ 3. Bài toán review code của Dũng thì vướng bảo mật repo công ty. Điều này dạy tôi rằng khi framing problem, phải đánh giá ngay nguồn lực mình đang có và khả năng xây dựng dataset để kiểm thử nhanh chóng. 

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**
Có, ngay khi tôi vừa pitch bài toán VoC, cả nhóm đã lao vào bàn luận "Hay là mình code một con AI Agent đọc thẳng Intercom rồi tự động nhắn tin qua Slack cho PM luôn, không cần CS nhúng tay vào". Chúng tôi bị cuốn vào sự "tiện lợi" của giải pháp Agent. Nhóm chỉ giật mình nhận ra khi làm bước phân tích Quy trình (AS-IS) và đánh giá rủi ro: nếu Agent tự động gửi sai báo cáo lỗi, hậu quả ai chịu? Từ đó nhóm quay ngược lại, tập trung vào điểm nghẽn cốt lõi (nỗi đau phải đọc thủ công) và hạ mức can thiệp xuống Workflow có con người kiểm duyệt (HITL).

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**
Có. Ban đầu tôi quá tin tưởng vào khả năng của LLM, cho rằng cứ ném file CSV vào là nó tự biết phân loại. Khi Dũng phản biện: *"Làm sao đảm bảo AI không tự bịa ra các tag mới (hallucinate) làm nát hệ thống taxonomy hiện tại của công ty?"*, tôi đã phải suy nghĩ lại. Tôi đổi ý, không để AI tự do phân loại nữa mà thiết lập Boundary cực kỳ chặt chẽ: AI bắt buộc phải map dữ liệu vào bộ tag cố định được nạp sẵn, và đầu ra phải là bản nháp (draft) để con người chốt cuối cùng.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**
Điều làm tôi bất ngờ nhất là insight từ "người tiêu thụ báo cáo" - Product Manager. Ban đầu, tôi định hướng AI chỉ cần đếm đúng số lượng ticket cho từng tag (ví dụ: 50 lỗi UI, 20 lỗi Payment) là đủ để đo lường. Nhưng qua đóng vai phỏng vấn, tôi nhận ra PM thực sự không quan tâm những con số vô hồn đó, họ cần "bối cảnh" (khách hàng phàn nàn nguyên văn như thế nào). Điều này buộc tôi phải thiết kế lại quy trình TO-BE, yêu cầu AI không chỉ đếm tag mà còn phải trích xuất được "Context / Quote", thay đổi hoàn toàn cách tôi định hình tiêu chí đánh giá đầu ra của AI.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**
Khó nhất là viết sao cho hoàn toàn "sạch" bóng dáng của giải pháp. Rất dễ để vô thức viết "Bottleneck là do CS không có công cụ AI để đọc lướt nhanh", hoặc định nghĩa Boundary là "AI dùng Make.com". Tôi đã phải gạch xóa nhiều lần để miêu tả thuần túy về nỗi đau nghiệp vụ (đọc chữ bằng mắt, đếm tay) và các con số baseline (thời gian 120 phút), đảm bảo người đọc Problem Statement xong chưa cần biết sẽ dùng công nghệ gì để giải.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**
Nếu làm lại, ở khâu gom nhóm (Cluster) và OST, tôi sẽ đẩy mạnh việc bóc tách nguyên nhân gốc rễ (root cause) của các problem khác. Ví dụ với bài toán "Điền template banner" của Thắng, tôi sẽ phản biện mạnh hơn để chỉ ra đây thuần túy là vấn đề thiếu kỹ năng dùng tools tự động hóa (No-code / Script), chứ không thực sự cần đến khả năng suy luận của AI, từ đó giúp nhóm tiết kiệm thời gian tranh luận ở vòng shortlist. Với bài của mình, tôi sẽ cố gắng quy đổi Success Metric từ "thời gian" sang "chi phí nhân sự tiết kiệm được" để thuyết phục hơn.

**6.7. Hiểu bài:** Bài toán của nhóm xuất phát từ việc nhân sự CS tốn quá nhiều thời gian đọc và gán tag thủ công hàng chục ticket để làm báo cáo VoC gửi PM mỗi tuần. Quy trình AS-IS bị nghẽn trực tiếp ở khâu đọc hiểu và trích xuất ngữ cảnh. Nhóm đặt metric thành công là giảm thời gian xử lý xuống dưới 30 phút, đồng thời PM không phải hỏi lại thông tin bối cảnh. Để kiểm soát rủi ro LLM bịa thông tin, nhóm thiết lập boundary cứng: AI chỉ làm nhiệm vụ sinh bản nháp báo cáo (draft), con người bắt buộc phải tham gia kiểm duyệt (HITL) trước khi gửi. Từ đó, mức can thiệp AI được chốt là Workflow tự động hóa thay vì dùng AI Agent. Dựa trên rào cản kỹ thuật thấp (xử lý text cơ bản) và rủi ro vận hành nằm trong tầm kiểm soát, nhóm ra quyết định "Go".

---

## 7. Tài liệu tham khảo

-
