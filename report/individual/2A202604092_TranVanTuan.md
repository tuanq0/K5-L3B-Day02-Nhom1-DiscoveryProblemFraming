# Báo cáo cá nhân — 2A202604092_TranVanTuan

> Đổi tên file theo quy tắc `MSSV_HoTen.md`, ví dụ `20241234_NguyenVanAn.md` (MSSV trước, dấu `_`, họ tên viết liền không dấu). Sửa cả dòng tiêu đề phía trên cho khớp.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên:Trần Văn Tuấn
- MSSV:2A202604092
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm:Nhóm 1
- Link repo nhóm:https://github.com/tuanq0/K5-L3B-Day02-Nhom1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Tốn thời gian | Khi chờ bến xe bus, tôi muốn biết bao giờ xe đến để biết có nên đứng tiếp hay làm việc riêng | Người đi xe bus | ở những bến vắng xe đôi khi phải đứng chờ đến 30 phút mới có xe đến |
| 2 | Cần đọc, tổng hợp nhiều thông tin | Khi kiểm tra sự kiện khuyến mãi, tôi muốn biết những đồ cần thiết có không | người mua, người bán | app shoppe có nhiều khuyến mãi nhưng không tìm kiếm khuyến mãi được |
| 3 | Tốn thời gian | Khi ôn thi 1 môn thì muốn tổng hợp nội dung để không phải giở sách từng chương có trong đề để học | người học | thi tnthpt không phải dạng bài nào trong sách giáo khoa cũng có trong đề |
| 4 | Cần đọc, tổng hợp nhiều thông tin | Khi muốn xem một bộ phim, tôi muốn được đưa ra các phương án có thể chọn | người xem, rạp chiếu phim | các rạp chiếu phim sẽ có những bộ phim khác nhau tùy sắp xếp của rạp |
| 5 | Pain từ người khác | Khi con học tiểu học/THCS, phụ huynh muốn biết con đang học gì, bài tập nào chưa nộp để khỏi phải hỏi con hoặc đợi cô nhắn | Phụ huynh bận đi làm, giáo viên chủ nhiệm | Thông tin rải rác ở nhóm Zalo lớp, sổ liên lạc, lời con kể. Phỏng vấn 3-5 phụ huynh và 1-2 giáo viên |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- gợi ý phụ huynh muốn biết con đang học gì thì giữ lại vì thấy nhiều phụ huynh hay gọi con khi ở trường để hỏi tình hình.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 |  Khi chờ bến xe bus, tôi muốn biết bao giờ xe đến để biết có nên đứng tiếp hay làm việc riêng | Vì chờ xe bus mệt mỏi nhưng nếu đi ra chỗ khác có thể bị lỡ chuyến | cách tính toán thời gian sao cho hợp lí |
| 2 | Khi ôn thi 1 môn thì muốn tổng hợp nội dung để không phải giở sách từng chương có trong đề để học | Vì để tận dụng thêm thời gian chuẩn bị cho bài thi tốt hơn | đảm bảo tính nguyên vẹn và liền mạch của kiến thức |
| 3 | Khi con học tiểu học/THCS, phụ huynh muốn biết con đang học gì, bài tập nào chưa nộp để khỏi phải hỏi con hoặc đợi cô nhắn | để bố mẹ bớt lo lắng và đỡ gọi cho con cái nhiều hơn | con cái sẽ không chịu bị kiểm soát như thế |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story |  Khi chờ bến xe bus, tôi muốn biết bao giờ xe đến để biết có nên đứng tiếp hay làm việc riêng |
| Actor | Người chờ xe bus |
| Thời điểm / bối cảnh | người chờ không biết xe tiếp theo bao giờ đến để có thể sắp xếp làm việc riêng nếu có |
| Quy trình hiện tại (3–7 bước) | đến bến xe bus -> chờ xe bus 1 lúc lâu hoặc nhanh -> lên xe |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước chờ xe bus, để đảm bảo lên được xe thì có thể phải chờ lâu |
| Impact (nếu không giải thì sao) | trải nghiệm đi xe bus tệ hơn, có thể ảnh hưởng đến ngày đó |
| Success metric (baseline → target) | khách chờ dưới 10 phút, không lo lắng về việc trễ xe |
| Phương án không dùng AI | tăng thêm số xe bus đi tuyến, thuật toán tính thời gian xe tiếp đến |
| Giả thuyết về AI (nếu có) | |
| Cảm nhận nhanh | No AI |

Quy trình nháp hiện tại:

```text
[1. Đến bến và xác định tuyến xe cần đi]
                 ↓
[2. Chờ xe tại bến, chưa biết chính xác giờ xe đến]
          ← BOTTLENECK — có lúc chờ đến 30 phút ở bến vắng
                 ↓
[3. Quan sát xe đến và lên đúng chuyến]
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi ôn thi 1 môn thì muốn tổng hợp nội dung để không phải giở sách từng chương có trong đề để học |
| Actor | Học sinh đang ôn thi một môn, đặc biệt là học sinh chuẩn bị thi tốt nghiệp THPT. |
| Thời điểm / bối cảnh | Trước kỳ thi, khi cần xác định phần kiến thức có trong phạm vi ôn tập và học từ nhiều chương trong sách giáo khoa. |
| Quy trình hiện tại (3–7 bước) | 1. Xác định môn và phạm vi ôn tập từ đề cương/thông tin của giáo viên. 2. Dò các chương, bài trong sách có liên quan. 3. Đọc và ghi lại kiến thức cần học. 4. Gom nội dung thành đề cương theo chủ đề. 5. Đối chiếu lại với phạm vi ôn tập và luyện dạng bài liên quan. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–3: dò sách và xác định phần liên quan; chưa có số phút thực tế, cần bấm giờ ở lần ôn tiếp theo. |
| Impact (nếu không giải thì sao) | Mất thời gian dò từng chương, có thể học lan man hoặc bỏ sót phần cần ôn, làm giảm thời gian luyện tập. |
| Success metric (baseline → target) | Baseline thời gian chưa đo: bấm giờ ít nhất 2 lần ôn một môn; mục tiêu thử nghiệm giảm ít nhất 25% thời gian tìm và tổng hợp nội dung, đồng thời đối chiếu đủ các mục trong phạm vi ôn tập với sách/đề cương. |
| Phương án không dùng AI | Dùng đề cương của giáo viên, mục lục sách và checklist theo chương; đánh dấu từng mục đã đọc và tự đối chiếu trước khi luyện đề. |
| Giả thuyết về AI (nếu có) | Nếu cung cấp đề cương và tài liệu nguồn, AI có thể lập danh sách chủ đề cần học, tóm tắt theo chủ đề và dẫn lại chương/mục để học sinh kiểm tra. Không nên dựa vào bản tóm tắt nếu không đối chiếu được với nguồn. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[1. Xác định môn và phạm vi ôn tập]
                 ↓
[2. Dò chương/bài liên quan trong sách]
          ← BOTTLENECK — chưa bấm giờ
                 ↓
[3. Đọc và ghi lại kiến thức cần học]
                 ↓
[4. Gom thành đề cương theo chủ đề]
                 ↓
[5. Đối chiếu đề cương với sách và luyện tập]
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi con học tiểu học/THCS, phụ huynh muốn biết con đang học gì, bài tập nào chưa nộp để khỏi phải hỏi con hoặc đợi cô nhắn |
| Actor | Phụ huynh bận đi làm và con đang học tiểu học/THCS; giáo viên chủ nhiệm là người có thể cập nhật thông tin lớp. |
| Thời điểm / bối cảnh | Khi phụ huynh muốn nắm nội dung học và bài tập cần hoàn thành trong ngày/tuần nhưng thông tin có thể nằm ở nhóm Zalo, sổ liên lạc hoặc lời kể của con. |
| Quy trình hiện tại (3–7 bước) | 1. Kiểm tra nhóm Zalo hoặc sổ liên lạc. 2. Tìm thông báo về bài học và bài tập. 3. Hỏi con nội dung đã học/đã làm. 4. Đối chiếu các thông tin còn thiếu. 5. Nhắc con hoàn thành bài hoặc chờ giáo viên cập nhật. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 1–4: thông tin phân tán và phải hỏi nhiều nơi; chưa đo thời gian hay tần suất, cần ghi nhận trong một tuần. |
| Impact (nếu không giải thì sao) | Phụ huynh có thể không biết bài cần nộp hoặc nhắc muộn; việc hỏi lặp lại cũng có thể làm con cảm thấy bị kiểm soát và ảnh hưởng sự chủ động. |
| Success metric (baseline → target) | Baseline số lần phụ huynh phải hỏi/tìm thông tin chưa đo: ghi nhận trong 1 tuần|
| Phương án không dùng AI | Thống nhất một kênh cập nhật chính thức, dùng checklist hoặc lịch chung theo tuần; để con tự đánh dấu bài đã hoàn thành và phụ huynh cùng xem. |
| Giả thuyết về AI (nếu có) | AI có thể tóm tắt thông báo học tập và trích xuất hạn nộp từ nội dung do phụ huynh/giáo viên cung cấp, nhưng cần kiểm tra lại với nguồn. Chỉ chia sẻ thông tin phù hợp, có sự đồng thuận của con và không theo dõi tin nhắn riêng tư. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
[1. Kiểm tra nhóm Zalo/sổ liên lạc]
                 ↓
[2. Tìm thông tin bài học và bài tập]
                 ↓
[3. Hỏi con phần chưa rõ]
          ← BOTTLENECK — nhiều nguồn, chưa đo
                 ↓
[4. Đối chiếu và xác định bài cần làm/nộp]
                 ↓
[5. Nhắc con hoặc chờ giáo viên cập nhật]
```

### Card muốn pitch nhất

- Card số: 2
- Vì sao: Đây là vấn đề học sinh có thể gặp khi ôn thi nhiều chương; quy trình dò sách rồi tổng hợp nội dung đã được mô tả cụ thể. Có thể kiểm tra hiệu quả bằng cách đo thời gian trước/sau, đồng thời đối chiếu đề cương với sách để tránh bỏ sót kiến thức.
- Câu hỏi muốn nhóm phản biện: Làm thế nào xác định đúng phạm vi kiến thức cần ôn và kiểm tra bản tổng hợp không bỏ sót hoặc làm sai lệch nội dung trong sách/đề cương?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Chưa xác định rõ người học dựa vào nguồn nào để biết chương/bài nào nằm trong phạm vi thi; thời gian tìm và tổng hợp cũng chưa có baseline. | Đồng ý | Nêu đề cương/thông tin của giáo viên làm căn cứ; ghi rõ thời gian chưa đo và đề xuất bấm giờ ít nhất 2 lần ôn. |
| Nếu chỉ tóm tắt tự động, có thể bỏ sót hoặc làm sai kiến thức; metric chỉ giảm thời gian sẽ chưa đảm bảo chất lượng. | Đồng ý | Bổ sung bước đối chiếu đề cương với sách và yêu cầu kiểm tra đủ các mục trong phạm vi ôn tập. |

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
| CP1 Scan | Gợi ý thêm vấn đề từ góc nhìn phụ huynh. | Gợi ra ý phụ huynh muốn biết con đang học gì; tôi giữ lại vì thấy phụ huynh thường gọi con khi con ở trường để hỏi tình hình. | Gợi ý chưa có bằng chứng về tần suất, mức độ ảnh hưởng hay nhu cầu thực tế. | Chỉ giữ ý như một candidate cần kiểm chứng, không xem gợi ý là bằng chứng. |
| CP2 Problem Card | Hỗ trợ diễn đạt quy trình và phản biện Card #2. | Giúp chia việc ôn tập thành các bước và nhận ra cần có tiêu chí kiểm tra độ đầy đủ, chính xác. | Thời gian baseline và mức giảm chưa có dữ liệu thực tế; giải pháp AI không tự đảm bảo nội dung chính xác. | Ghi rõ baseline chưa đo, đề xuất bấm giờ và thêm bước đối chiếu với đề cương/sách. |

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
