 # Báo cáo cá nhân — 2A202604076_DaoHongThang

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Đào Hồng Thắng
- MSSV: 2A202604092
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: nhóm 1
- Link repo nhóm: https://github.com/tuanq0/K5-L3B-Day02-Nhom1-DiscoveryProblemFraming.git

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Lặp lại | Khi tôi làm banner quảng cáo, tôi muốn những chỗ placeholder trong template mẫu được điền nội dung trong file Excel, để không phải copy thủ công từ Excel vào template Canva/PowerPoint. | Bản thân, người thuê | 1 tiếng cho 100 dòng trong sheet. |
| 2 | Lặp lại | Khi được yêu cầu làm một chức năng trong tài liệu, tôi muốn tự động hóa các bước phân tích, đề xuất giải pháp, implement, test và tạo tài liệu test, để tôi chỉ cần review kết quả. | Bản thân, PM, QA | Quy trình gồm nhiều bước từ phân tích đến kiểm thử và lập tài liệu; chưa có số đo thời gian/tần suất. |
| 3 | Tốn thời gian | Khi làm tài liệu test theo mẫu và cần chụp evidence, tôi muốn phần giải thích được tự tạo trong tài liệu, để tôi chỉ cần chụp evidence. | Bản thân, PM | 2 tiếng cho một lần làm tài liệu. |
| 4 | Lặp lại | Khi phát sinh các khoản chi tiêu trong ngày, tôi muốn theo dõi đầy đủ và phân loại các khoản thu chi, để biết chính xác tiền đã được sử dụng vào mục đích nào. | Bản thân | Phát sinh hàng ngày; chưa đo số giao dịch hoặc thời gian ghi chép. |
| 5 | Cần đọc, tổng hợp nhiều thông tin | Khi cân nhắc mua sản phẩm giá trị lớn hoặc trả góp, tôi muốn hiểu tổng chi phí và nghĩa vụ thanh toán của từng lựa chọn, để đánh giá khả năng chi trả trước khi quyết định. | Bản thân, bên bán, tổ chức tài chính | Cần đọc và so sánh giá, lãi suất, phí và điều kiện thanh toán; chưa đo tần suất. |
| 6 | Lặp lại | Khi học kiến thức mới, tôi muốn xác định mức độ ghi nhớ của từng chủ đề sau một khoảng thời gian, để biết phần nào đã hiểu, phần nào còn yếu và duy trì ghi nhớ lâu dài. | Bản thân | Cần ôn lại kiến thức sau một khoảng thời gian; chưa đo tần suất hoặc mức độ quên. |
| 7 | Pain từ người khác | Khi gửi Pull Request để review, tôi muốn người review hiểu nhanh mục đích thay đổi và khu vực bị ảnh hưởng, để quá trình review diễn ra thuận lợi hơn. | Người review, người gửi PR | Người review phải tự tìm hiểu mục đích và phạm vi thay đổi; chưa có số đo thời gian hoặc số người. |
| 8 | — | — | — | — |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Không có thông tin về ý tưởng được AI gợi ý trong phần nội dung cung cấp.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Điền nội dung Excel vào template banner quảng cáo | Quy trình lặp lại, thao tác thủ công rõ ràng, có baseline ước tính (1 giờ/100 dòng), đầu vào và đầu ra cụ thể. | Tần suất thực hiện đã đủ cao chưa? |
| 2 | Quản lý tài chính | Nhu cầu phát sinh hàng ngày, thao tác lặp lại, có thể đo lường lượng giao dịch. | Có sẵn sàng ghi chép thường xuyên không? |
| 3 | Mua sản phẩm có giá trị lớn | Phải đọc và so sánh nhiều nguồn thông tin để ra quyết định. | Có mua thường xuyên không? |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi tôi làm banner quảng cáo, tôi muốn những chỗ placeholder trong template mẫu được điền nội dung trong file Excel, để không phải copy thủ công từ Excel vào template Canva/PowerPoint. |
| Actor | Người thuê |
| Thời điểm / bối cảnh | Mỗi tối |
| Quy trình hiện tại (3–7 bước) | 1. Lấy nội dung từng row trong sheet. 2. Tìm ảnh theo mô tả trong nội dung. 3. Điền nội dung và ảnh vào đúng vị trí trong template Canva. 4. Xuất file PDF. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Tìm ảnh mất thời gian và thao tác điền lặp lại; tổng cộng khoảng 1 tiếng/ngày cho 100 row. Chưa có số đo riêng cho từng bước. |
| Impact (nếu không giải thì sao) | Tốn khoảng 1 tiếng mỗi ngày cho thao tác thủ công; có thể giảm thời gian dành cho công việc khác. |
| Success metric (baseline → target) | Tổng thời gian xử lý 100 row: baseline 1 giờ → dưới 30 phút. |
| Phương án không dùng AI | Dùng template cố định, script và workflow để điền nội dung vào template. |
| Giả thuyết về AI (nếu có) | AI tự động tạo ảnh phù hợp với mô tả. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
Lấy các row trong sheet → tìm ảnh theo mô tả → điền nội dung và ảnh vào template → xuất PDF
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi phát sinh các khoản chi tiêu trong ngày, tôi muốn theo dõi đầy đủ các khoản thu chi, để biết chính xác tiền đã được sử dụng vào những mục đích nào. |
| Actor | Bản thân |
| Thời điểm / bối cảnh | Hàng ngày |
| Quy trình hiện tại (3–7 bước) | 1. Mua sản phẩm hoặc phát sinh khoản thu/chi. 2. Ghi chép nhanh lại. 3. Tổng hợp các khoản vào sheet. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Có thể quên ghi hoặc ghi không đầy đủ; mỗi lần ghi chép tốn thêm vài phút. |
| Impact (nếu không giải thì sao) | Dữ liệu thu chi không đầy đủ, khó biết chính xác tiền đã được dùng vào mục đích nào. |
| Success metric (baseline → target) | Baseline chưa được đo; mục tiêu mong muốn là không phải ghi chép thủ công và theo dõi đầy đủ các khoản thu chi. |
| Phương án không dùng AI | Ghi chép thủ công rồi tổng hợp vào sheet. |
| Giả thuyết về AI (nếu có) | AI điều phối workflow theo dõi và tổng hợp thu chi. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
Phát sinh khoản thu/chi → ghi chép nhanh → tổng hợp vào sheet
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi cân nhắc mua một sản phẩm có giá trị lớn hoặc lựa chọn hình thức trả góp, tôi muốn hiểu tổng chi phí và nghĩa vụ thanh toán của từng lựa chọn, để đánh giá khả năng chi trả trước khi quyết định. |
| Actor | Bản thân |
| Thời điểm / bối cảnh | Khi cân nhắc mua sản phẩm giá trị lớn hoặc trả góp; tần suất chưa xác định. |
| Quy trình hiện tại (3–7 bước) | 1. Tìm thông tin về giá sản phẩm. 2. Đọc lãi suất, phí và điều kiện thanh toán từ các nguồn. 3. So sánh tổng chi phí và nghĩa vụ thanh toán giữa các lựa chọn. 4. Đánh giá khả năng chi trả và quyết định. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Phải đọc và tổng hợp nhiều thông tin về giá, lãi suất, phí và điều kiện; thời gian thực tế chưa được đo. |
| Impact (nếu không giải thì sao) | Khó nắm được tổng chi phí và nghĩa vụ thanh toán, từ đó khó đánh giá khả năng chi trả trước khi quyết định. |
| Success metric (baseline → target) | Baseline chưa được đo; mục tiêu là có thể so sánh tổng chi phí và nghĩa vụ thanh toán của các lựa chọn trước khi quyết định. |
| Phương án không dùng AI | Tự đọc thông tin từ các nguồn và so sánh bằng bảng tính hoặc máy tính. |
| Giả thuyết về AI (nếu có) | AI có thể trích xuất và tổng hợp giá, lãi suất, phí, điều kiện thanh toán từ thông tin người dùng cung cấp; kết quả cần được kiểm tra trước khi ra quyết định. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
Tìm thông tin → đọc giá, lãi suất, phí và điều kiện → so sánh tổng chi phí/nghĩa vụ thanh toán → đánh giá khả năng chi trả → quyết định
```

### Card muốn pitch nhất

- Card số: #3 - Mua sản phẩm giá trị lớn hoặc trả góp.
- Vì sao: Người mua phải tự đọc và tổng hợp giá, lãi suất, phí và điều kiện thanh toán từ nhiều nguồn để hiểu tổng chi phí. Nếu không làm rõ được các khoản này, họ khó đánh giá khả năng chi trả trước khi quyết định. Tuy vậy, tần suất gặp vấn đề và thời gian thực tế hiện chưa được đo.
- Câu hỏi muốn nhóm phản biện: Vấn đề này có đủ thường xuyên và tốn công để ưu tiên không? Nhóm nghĩ nên kiểm chứng bằng cách nào, và nên dùng chỉ số nào để đo mức độ cải thiện?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa có dữ liệu về tần suất gặp vấn đề và thời gian thực tế để đọc, tổng hợp thông tin, nên chưa đủ cơ sở đánh giá mức độ ưu tiên. | Đồng ý. | Ghi rõ tần suất và thời gian chưa được đo; cần kiểm chứng với người mua sản phẩm giá trị lớn trước khi kết luận đây là vấn đề ưu tiên. |
| Thông tin tài chính có thể thiếu hoặc sai nếu nguồn cung cấp không đầy đủ; người dùng không nên dựa hoàn toàn vào phần tổng hợp của AI để quyết định. | Đồng ý. | Giới hạn giả thuyết AI ở việc trích xuất, tổng hợp thông tin người dùng cung cấp và nêu rõ kết quả cần được kiểm tra trước khi ra quyết định. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Tôi đưa ra ba candidate: tự động điền dữ liệu Excel vào banner, theo dõi thu chi và so sánh chi phí khi mua sản phẩm giá trị lớn/trả góp. Trong đó, tôi muốn pitch Card #3 nhất. | Dù Card #3 là lựa chọn tôi muốn pitch, nhóm không chọn card này làm đề tài cuối. Nhóm chọn **Báo cáo VoC (Anh)**: phân loại và tổng hợp ticket Intercom thành báo cáo Voice of Customer hằng tuần cho PM. |
| Phản biện bài của bạn khác |   |  |
| Nhận phản biện | Với Card #1 về banner, nhóm đặt câu hỏi vì sao cần AI thay vì dùng script/rule để điền template cố định. | Câu hỏi giúp làm rõ cần cân nhắc giải pháp đơn giản hơn AI;  |
| Gom cluster / cây OST | Tôi tham gia gom các candidate theo pattern chung và xây cây OST với outcome tối ưu hiệu suất xử lý thông tin. | Nhóm xác định cơ hội giảm thao tác đọc, phân loại và trích xuất dữ liệu văn bản định kỳ; Báo cáo VoC (Anh) phù hợp với cơ hội này. |
| Chọn candidate problem | Tôi tham gia xem xét shortlist và tiêu chí chấm điểm. | Báo cáo nhóm ghi nhận Báo cáo VoC (Anh) đạt 35/35 và được chọn: tự động hóa việc phân loại, tổng hợp ticket Intercom thành báo cáo VoC tuần cho PM.  |
| Kiểm chứng / research | Tôi tham gia xem xét kết quả phỏng vấn CS Executive và PM, cùng research các hướng như Zapier/Make.com tích hợp OpenAI và Intercom Fin AI/AI Insights. | Bằng chứng cho thấy quy trình báo cáo mất khoảng 120 phút mỗi thứ Sáu và PM hỏi thêm context ở 4/5 báo cáo gần nhất; nhóm bổ sung yêu cầu đếm đúng Top 3 tag và trích xuất context. |
| Quy trình nhóm | Tôi tham gia phân tích quy trình Báo cáo| Nhóm xác định hai bottleneck: đọc/gán tag thủ công 60–80 phút và lọc context 20 phút; mục tiêu là giảm tổng thời gian từ khoảng 120 xuống dưới 30 phút. |
| Problem Statement | Tôi tham gia xây dựng Problem Statement cho Báo cáo VoC, xác định actor là CS Executive và PM tại EdTech Startup, bottleneck, impact và metric. | Mục tiêu là giảm thời gian làm báo cáo từ 120 xuống dưới 30 phút và giảm số lần PM hỏi thêm context từ 4 lần/tháng xuống 0; CS phải duyệt bản nháp trước khi gửi. |
| Mức can thiệp AI | Tôi tham gia so sánh No AI, Rule, Workflow và Agent cho Báo cáo VoC. | Nhóm chọn Workflow để AI phân loại intent theo taxonomy có sẵn, đếm Top 3 và tạo nháp báo cáo; CS kiểm tra, chỉnh sửa trước khi gửi. |
| Quyết định | Tôi tham gia thống nhất quyết định Go cho Báo cáo VoC (Anh). | Nhóm đề xuất pilot trên CSV của tuần trước, đối chiếu Top 3 với kết quả thủ công và đánh giá thời gian cũng như chất lượng context; nếu hallucination tag vượt 10% sau 2 tuần thì quay về phương án khác. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tôi dùng AI để tìm thêm những vấn đề gặp phải trong context của chính tôi | AI giúp tôi tìm ra thêm vấn đề cần giải quyết | Chưa có thông tin. | Tôi sửa lại cho phù hợp với bản thân mình và vấn đề mà mình nhận thấy |
| CP2 Problem Card | Dùng AI để rà soát Card #3 về mua sản phẩm giá trị lớn/trả góp. | Giúp nhận ra còn thiếu dữ liệu về tần suất, thời gian xử lý và cần kiểm chứng trước khi đánh giá mức độ ưu tiên. | Nhận xét chỉ dựa trên nội dung card, không thay thế phản hồi của người mua hoặc bằng chứng thực tế. | Ghi rõ tần suất và thời gian chưa được đo; giới hạn giả thuyết AI ở việc tổng hợp thông tin người dùng cung cấp và yêu cầu kiểm tra kết quả. |
| CP4 Research | Chưa ghi nhận việc dùng AI ở checkpoint này; báo cáo nhóm ghi phỏng vấn và research giải pháp. | Chưa có thông tin về đóng góp riêng của AI. | Chưa có thông tin. | Chưa có thông tin. |
| CP5 Quy trình | Chưa ghi nhận việc dùng AI ở checkpoint này; báo cáo nhóm mô tả quy trình VoC trước và sau. | Chưa có thông tin về đóng góp riêng của AI. | Chưa có thông tin. | Chưa có thông tin. |
| CP5–6 Problem Statement | Chưa ghi nhận việc dùng AI để viết Problem Statement của nhóm. | Chưa có thông tin về đóng góp riêng của AI. | Chưa có thông tin. | Chưa có thông tin. |
| CP6 Mức can thiệp / quyết định | Chưa ghi nhận việc dùng AI để so sánh mức can thiệp hoặc đưa ra quyết định của nhóm. | Chưa có thông tin về đóng góp riêng của AI. | Chưa có thông tin. | Chưa có thông tin. |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

---

## 7. Tài liệu tham khảo

-
