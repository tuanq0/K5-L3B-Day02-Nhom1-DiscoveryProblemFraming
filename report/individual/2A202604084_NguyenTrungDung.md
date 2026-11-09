# Báo cáo cá nhân — 2A202604084_NguyenTrungDung

## 1. Thông tin học viên

- **Họ tên:** Nguyễn Trung Dũng
- **MSSV:** 2A202604084
- **Tên nhóm:** Nhóm 1
- **Link repo nhóm:** https://github.com/tuanq0/K5-L3B-Day02-Nhom1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Mình bắt đầu từ những việc đã gặp khi làm dự án, sinh hoạt và học nhóm. Có việc lặp lại khá nhiều, có việc không mất quá nhiều phút nhưng dễ làm sai hoặc khiến người khác phải chờ. Mình giữ cả những vấn đề nhỏ ở bước này, chưa vội nghĩ đến công cụ để giải quyết.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thực tế |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi review Pull Request (PR) của đồng đội, tôi muốn hiểu phần logic được thay đổi và chỗ nào đang đụng tới code của người khác, để biết cần sửa gì trước khi merge mà không làm hỏng chức năng cũ. | Người review PR và các developer cùng làm dự án. | Khoảng 10 PR/tuần. PR đơn giản thường xem trong khoảng 1 phút; PR có phần code chồng lấn có thể mất 10–15 phút. Đây là thời gian mình ước lượng từ lúc làm việc, chưa có log bấm giờ; repo riêng nên không đưa nội dung PR lên công khai. |
| 2 | Lặp lại | Khi tổng kết chi tiêu cuối tháng, tôi muốn đối chiếu các khoản đã dùng qua tài khoản ngân hàng, ví điện tử và tiền mặt, để biết mình thực sự đã chi bao nhiêu và có bị lệch số dư không. | Bản thân mình, người tự theo dõi chi tiêu cá nhân. | Khoảng 150 giao dịch/tháng. Mình thường dành chừng 5 phút để xem nhanh số liệu, nhưng vẫn có tháng chênh vài trăm nghìn đồng vì bỏ sót khoản nhỏ. 5 phút ở đây không phải thời gian rà lại từng giao dịch. |
| 3 | Tốn thời gian | Khi đi mua thực phẩm hoặc đồ dùng cá nhân, tôi muốn nhớ được món nào đang thiếu và nên mua ở đâu, để không phải đứng nghĩ lại tại cửa hàng hay đi về rồi mới phát hiện quên đồ. | Bản thân mình, hiện sống một mình. | Mình đi mua đồ khoảng 3 lần/tuần. Có lần phải cân nhắc khá lâu hoặc không mua được món định mua vì hết hàng. Chưa ghi lại chính xác số phút mất thêm. |
| 4 | Tốn thời gian | Khi cần làm căn cước công dân trực tiếp, tôi muốn nắm rõ giấy tờ và các bước phải làm trước khi đến nơi, để hạn chế việc đi lại hoặc phải xin nghỉ thêm. | Người đi làm thủ tục hành chính, nhất là người khó sắp xếp thời gian nghỉ. | Theo trải nghiệm đã ghi lại, mình từng chờ khoảng 1 tháng để nhận thẻ gửi về; địa điểm làm thủ tục xa và đông người, trong khi mình chỉ có 1 ngày nghỉ/tháng. Chưa có số liệu về số lần phải quay lại do thiếu giấy tờ. |
| 5 | Pain từ người khác | Khi nhóm học tập cần gặp trực tiếp, tôi muốn tìm được một khung giờ mà mọi người đều xác nhận tham gia, để không phải đổi lịch liên tục hoặc đến sát giờ mới biết có người bận. | Nhóm học tập gồm 6 thành viên. | Nhóm hiện gặp trực tiếp khoảng 1 buổi/2 tuần. Khi trao đổi qua Messenger/Discord, các bạn thường phản hồi vào những thời điểm khác nhau, có lúc trùng lịch hoặc báo bận khá sát giờ. Có thể kiểm tra lại mốc tin nhắn để đo thời gian chốt lịch. |

### Ghi chú sau khi scan

- Năm vấn đề trên là những chuyện mình đã gặp hoặc trực tiếp tham gia, không phải những ý tưởng về sản phẩm muốn làm.
- Khi tham khảo thêm gợi ý từ AI, mình có sửa ví dụ “mua sắm gia đình” thành “mua sắm cá nhân”, vì mình sống một mình. Những gợi ý về tổng hợp tài liệu học tập, du lịch hay chuẩn bị đi khám bệnh không được đưa vào bảng vì mình chưa có trải nghiệm đủ cụ thể để làm căn cứ.
- Các con số ở bảng là mức mình nhớ và ước lượng, chưa phải dữ liệu được đo đạc đầy đủ. Đặc biệt, chuyện làm căn cước và mua sắm cần thêm bằng chứng nếu nhóm muốn chọn để nghiên cứu sâu.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

Mình chọn ba vấn đề **#1, #2 và #5** trong bảng CP1. Cả ba đều có người gặp vấn đề cụ thể, có thể vẽ được cách họ đang làm và có đầu ra để theo dõi. Mình ưu tiên chuyện review PR vì đây là việc diễn ra thường xuyên và mình biết rõ bước nào làm mình mất thời gian.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Review PR có phần code chồng lấn (CP1 #1) | Gặp tương đối thường xuyên; bước đọc và đối chiếu logic khá rõ; có thể đo thời gian trên các PR tiếp theo. | Chưa biết bao nhiêu PR thực sự có code chồng lấn; nguyên nhân do thay đổi logic hay do cách chia việc trong nhóm. |
| 2 | Đối chiếu chi tiêu cá nhân (CP1 #2) | Có khoảng 150 giao dịch/tháng và từng gặp tình trạng lệch số dư; có thể đối chiếu lại bằng lịch sử giao dịch. | Chưa biết các khoản thiếu chủ yếu do quên ghi tiền mặt, chuyển tiền giữa các ví hay lỗi phân loại. |
| 3 | Sắp xếp lịch họp nhóm (CP1 #5) | Có 6 người cùng tham gia; có thể kiểm tra tin nhắn và lịch họp để xác định điểm nghẽn. | Chưa đo thời gian chờ phản hồi; chưa tách được việc khó thống nhất lịch với việc một số người không cam kết tham gia. |

**Lưu ý về thời gian trong quy trình:** Các phút ghi ở phần dưới là **ước tính để phác thảo**, không phải kết quả bấm giờ. Với PR và chi tiêu, mình chia khoảng thời gian đã nêu ở CP1 thành các bước để xem bước nào có thể nghẽn. Với lịch họp, thời gian chờ chỉ là một kịch bản giả định, phải kiểm tra lại từ lịch sử chat trước khi dùng làm baseline.

### Problem Card #1 — Review Pull Request

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi review PR của đồng đội, tôi muốn hiểu logic mới và phần code đang bị chồng lấn, để quyết định cần sửa gì trước khi merge mà không ảnh hưởng chức năng hiện có. |
| **Actor** | Người review PR trong nhóm phát triển phần mềm; thường phải đọc cả thay đổi của người khác lẫn phần code mình đang làm. |
| **Thời điểm / bối cảnh** | Khi có PR mới chạm vào module hoặc logic đang được nhiều người sửa. Đây có thể là xung đột logic, không nhất thiết là Git báo merge conflict. |
| **Quy trình hiện tại (5 bước)** | Nhận PR → xem diff → đối chiếu logic với code hiện tại → quyết định giữ/sửa phần chồng lấn → merge và kiểm tra nhanh. |
| **Bottleneck** | **Bước 3: đối chiếu logic**, dự kiến khoảng 5 phút trong trường hợp PR có phần code chồng lấn. Vì phải đọc thêm phần code liên quan nên việc xem một PR không còn đơn giản là nhìn diff. |
| **Impact** | PR bị giữ lâu hơn, làm chậm việc ghép code; nếu vội xử lý có thể sửa sai logic hoặc phát sinh lỗi sau merge. |
| **Success metric (baseline → target)** | **Baseline:** khoảng 10–15 phút/PR có code chồng lấn (ước lượng từ CP1). **Target thử nghiệm:** không quá 7 phút/PR cùng loại. **Cách đo:** ghi thời điểm bắt đầu và kết thúc review 10 PR có code chồng lấn tiếp theo; so sánh trung vị thời gian, không tính thời gian chờ CI chạy. |
| **Phương án không dùng AI** | Chia PR nhỏ hơn, thống nhất người phụ trách từng module, ghi rõ phần thay đổi logic trong mô tả PR và dùng checklist review. |
| **Giả thuyết về AI (nếu có)** | Có thể thử hỗ trợ tóm tắt thay đổi và chỉ ra phần logic cần xem kỹ. Reviewer vẫn phải đọc code và quyết định, không để công cụ tự merge. |
| **Cảm nhận nhanh** | Nghiêng về **Workflow**, nhưng nên thử cách cải thiện quy trình trước. |

**Quy trình hiện tại (ước tính cho một PR có code chồng lấn):**

```text
[1. Nhận PR, đọc mô tả: 0,5 phút]
    ↓
[2. Xem các file thay đổi và diff: 2 phút]
    ↓
[3. Đối chiếu logic với code hiện tại: 5 phút]  ← NGHẼN
    ↓
[4. Chọn cách xử lý phần chồng lấn: 3 phút]
    ↓
[5. Merge và kiểm tra nhanh: 2 phút]

Tổng thao tác ước tính: 12,5 phút/PR.
Chưa tính thời gian chờ người khác trả lời hoặc CI chạy.
```

Lý do mình đánh dấu bước 3: nếu PR chỉ sửa một phần độc lập thì việc đọc diff khá nhanh. Khi hai người cùng thay đổi luồng xử lý, mình phải mở thêm code liên quan mới biết phần nào có thể giữ lại. Bước 4 cũng mất thời gian, nhưng bước 3 là chỗ cần hiểu đúng trước khi quyết định.

### Problem Card #2 — Đối chiếu chi tiêu cá nhân

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi tổng kết chi tiêu cuối tháng, tôi muốn đối chiếu các khoản dùng qua ngân hàng, ví điện tử và tiền mặt, để biết số tiền thực sự đã chi và phát hiện khoản mình bỏ sót. |
| **Actor** | Bản thân mình, người tự quản lý chi tiêu và sử dụng nhiều nguồn tiền. |
| **Thời điểm / bối cảnh** | Cuối tháng, khi muốn xem tổng chi và kiểm tra số dư còn lại. |
| **Quy trình hiện tại (5 bước)** | Mở lịch sử ngân hàng → xem giao dịch ví điện tử → nhớ lại các khoản tiền mặt → so các nguồn và tìm khoản thiếu → tính tổng chi. |
| **Bottleneck** | **Bước 3: nhớ lại các khoản tiền mặt**, dự kiến khoảng 1,5 phút khi chỉ tổng kết nhanh. Vấn đề chính không hẳn là mất vài phút, mà là có khoản không còn nhớ để đưa vào bảng chi tiêu. |
| **Impact** | Có tháng tổng chi bị lệch vài trăm nghìn đồng; từ đó khó biết mình tiêu quá tay ở khoản nào. |
| **Success metric (baseline → target)** | **Baseline:** đôi khi chênh vài trăm nghìn đồng/tháng (chưa có thống kê đầy đủ). **Target thử nghiệm:** chênh không quá 50.000 đồng/tháng. **Cách đo:** ghi lại giao dịch trong tháng, đối chiếu số dư đầu/cuối kỳ của từng nguồn và số tiền mặt thực có; không tính chuyển tiền giữa các tài khoản là chi tiêu. |
| **Phương án không dùng AI** | Ghi khoản chi ngay sau khi thanh toán, dùng một bảng tính chung và đối soát mỗi tuần thay vì dồn đến cuối tháng. |
| **Giả thuyết về AI (nếu có)** | Nếu sau này có dữ liệu giao dịch đủ tốt, công cụ có thể hỗ trợ phân loại hoặc nhắc kiểm tra khoản chưa rõ. Nhưng AI cũng không thể tự biết giao dịch tiền mặt chưa từng được ghi lại. |
| **Cảm nhận nhanh** | **No AI / Rule** là đủ để thử trước. |

**Quy trình hiện tại (ước tính cho một lần tổng kết nhanh):**

```text
[1. Mở lịch sử giao dịch ngân hàng: 1 phút]
    ↓
[2. Xem giao dịch ví điện tử: 0,5 phút]
    ↓
[3. Nhớ lại các khoản chi tiền mặt: 1,5 phút]  ← NGHẼN
    ↓
[4. Đối chiếu nguồn tiền, tìm khoản thiếu: 1,5 phút]
    ↓
[5. Ước tính tổng chi và số dư: 0,5 phút]

Tổng thao tác ước tính: 5 phút/tháng.
Đây chỉ là bước xem nhanh, chưa đủ để kiểm hết ~150 giao dịch.
```

Ở vấn đề này, mình không nghĩ rút từ 5 phút xuống 2 phút là thành công. Nếu tổng kết nhanh hơn nhưng vẫn thiếu giao dịch thì số liệu vẫn sai. Vì vậy mình chọn độ lệch khi đối soát làm chỉ số chính, còn thời gian là chỉ số phụ.

### Problem Card #3 — Sắp xếp lịch họp nhóm

| Trường | Nội dung |
|---|---|
| **Job Story** | Khi nhóm học tập cần gặp trực tiếp, tôi muốn tìm được khung giờ mà cả nhóm xác nhận tham gia, để hạn chế đổi lịch và báo vắng ngay trước buổi họp. |
| **Actor** | Nhóm học tập 6 người, đặc biệt là người đứng ra chốt lịch. |
| **Thời điểm / bối cảnh** | Khi nhóm lên lịch gặp mặt, mọi người trao đổi qua Messenger hoặc Discord và có lịch cá nhân khác nhau. |
| **Quy trình hiện tại (6 bước)** | Đề xuất buổi họp → hỏi giờ rảnh → chờ các thành viên trả lời → so lịch để chọn giờ → chốt và yêu cầu xác nhận → xử lý thay đổi nếu có người bận. |
| **Bottleneck** | **Bước 3: chờ đủ phản hồi**. Đây là thời gian chờ theo đồng hồ chứ không phải thời gian người chốt lịch phải ngồi làm. Chưa có số liệu thật về số phút chờ; cần xem lại thời điểm gửi tin nhắn và thời điểm người cuối cùng trả lời. |
| **Impact** | Khó sắp xếp gặp mặt đều đặn; hiện nhóm chỉ gặp khoảng 1 buổi/2 tuần, việc trao đổi trực tiếp dễ bị ngắt quãng. |
| **Success metric (baseline → target)** | **Baseline:** khoảng 1 buổi họp trực tiếp/2 tuần. **Target thử nghiệm:** duy trì 1 buổi/tuần trong 4 tuần liên tiếp. **Cách đo:** ghi ngày lên lịch, ngày họp thật, số người tham gia và số lần phải đổi lịch. |
| **Phương án không dùng AI** | Tạo poll chọn giờ, yêu cầu phản hồi trước một hạn cụ thể, dùng lịch chung và quy ước báo vắng sớm. |
| **Giả thuyết về AI (nếu có)** | Có thể tổng hợp các khung giờ từ tin nhắn, nhưng nếu thành viên không phản hồi hoặc không giữ cam kết thì công cụ khó giải quyết được. |
| **Cảm nhận nhanh** | **No AI / Rule**; ưu tiên thay đổi cách chốt lịch. |

**Quy trình hiện tại (ước tính, tách thời gian thao tác và thời gian chờ):**

```text
[1. Đề xuất buổi họp trong nhóm: 2 phút]
    ↓
[2. Hỏi lịch của 6 thành viên: 4 phút]
    ↓
[3. Chờ đủ phản hồi: giả định 120–1.440 phút]  ← NGHẼN
    ↓
[4. So các khung giờ, chọn giờ phù hợp: 5 phút]
    ↓
[5. Chốt lịch và nhắc mọi người xác nhận: 3 phút]
    ↓
[6. Xử lý tin báo bận, đổi lịch (nếu có): 5 phút]

Thao tác chủ động ước tính: 19 phút/lần chốt lịch.
Khoảng chờ 120–1.440 phút chỉ dùng để minh họa,
KHÔNG phải số liệu đã quan sát. Cần đo lại từ lịch sử chat.
```

Mình tách riêng phần chờ vì nếu cộng tất cả lại thành “thời gian làm việc” sẽ dễ hiểu sai. Một người có thể mất vài phút để gửi poll, nhưng cả nhóm vẫn phải đợi đến hôm sau mới thống nhất được. Ở đây, thay đổi quy định phản hồi có lẽ đáng thử hơn việc xây một hệ thống mới.

### Card muốn pitch nhất

- **Card số:** 1 — Review Pull Request.
- **Vì sao:** Đây là vấn đề mình gặp trong công việc dev, có tình huống cụ thể để đem ra trao đổi và có thể kiểm tra lại thời gian trên các PR tiếp theo.
- **Câu hỏi muốn nhóm phản biện:** Thứ làm chậm việc review là thiếu thông tin về logic trong PR, hay do nhóm đang chia việc khiến nhiều người sửa cùng một phần code? Nếu là vế thứ hai thì sửa quy trình có thể hiệu quả hơn thêm công cụ.

### AI đã phản biện card thế nào

| Điểm yếu được chỉ ra | Mình có đồng ý không? | Mình chỉnh lại thế nào? |
|---|---|---|
| Không phải PR nào cũng có phần code chồng lấn. Lấy 10–15 phút nhân với tất cả PR trong tuần sẽ làm số liệu sai. | Có. | Chỉ dùng thời gian 10–15 phút cho PR có code chồng lấn; nếu muốn tính tổng thời gian mất mỗi tuần thì phải đếm tỷ lệ PR thuộc loại này. |
| Việc lệch chi tiêu có thể do quên ghi tiền mặt, không phải do khâu tính toán kém. | Có. | Đổi trọng tâm từ “tổng kết nhanh hơn” sang “ghi đủ và đối soát ít lệch hơn”; ưu tiên thử cách không dùng AI. |
| Vấn đề chốt lịch còn liên quan đến thói quen trả lời và cam kết tham gia, không chỉ thiếu công cụ. | Có. | Thêm thời hạn phản hồi, poll và quy tắc báo vắng vào phương án đơn giản; chưa vội chọn công cụ tự động. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | | |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt: | |
| Nhận phản biện | Câu hỏi tôi nhận được: | Tôi đã sửa gì: |
| Gom cluster / cây OST | | |
| Chọn candidate problem | | |
| Kiểm chứng / research | | |
| Quy trình nhóm | | |
| Problem Statement | | |
| Mức can thiệp AI | | |
| Quyết định | | |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Tham khảo cách viết Job Story và gợi ý thêm các vấn đề để tự chọn lọc. | Giúp mình nhìn lại vấn đề theo actor và bối cảnh. | Có gợi ý về mua sắm cho gia đình, không khớp việc mình sống một mình; vài gợi ý khác chưa có trải nghiệm để chứng minh. | Giữ những chuyện mình đã gặp, sửa lại thành mua sắm cá nhân và ghi rõ số liệu nào mới chỉ là ước tính. |
| CP2 Problem Card | Nhờ phản biện ba card, nhất là phần bottleneck, metric và khả năng giải quyết không cần AI. | Nhắc mình không suy rộng thời gian của PR có conflict sang mọi PR, và không coi việc làm nhanh hơn là đủ nếu số liệu chi tiêu vẫn lệch. | Không có dữ liệu để xác nhận thời gian từng bước; các target mới là đề xuất. | Tách rõ quan sát với giả định, chọn metric phù hợp từng vấn đề và ưu tiên thử phương án đơn giản trước. |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

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

- [README](../../README.md), [CHECKPOINTS](../../CHECKPOINTS.md), [RULES](../../RULES.md) và [Worksheet](../../docs/01-worksheet.md) trong repo bài học.
