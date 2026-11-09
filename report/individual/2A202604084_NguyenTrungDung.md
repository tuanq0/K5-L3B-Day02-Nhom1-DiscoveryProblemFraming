# Báo cáo cá nhân — 2A202604084_NguyenTrungDung

## 1. Thông tin học viên

- Họ tên: Nguyễn Trung Dũng
- MSSV: 2A202604084
- Email trường (không bắt buộc):
- Tên nhóm: Nhóm 1
- Link repo nhóm: https://github.com/tuanq0/K5-L3B-Day02-Nhom1-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi review PR của đồng đội, tôi muốn hiểu logic mới và phần code đang bị chồng lấn, để quyết định giữ cách triển khai nào mà không làm hỏng chức năng. | Developer và reviewer trong nhóm | Khoảng 10 PR/tuần; PR đơn giản ~1 phút, PR conflict ~10–15 phút tùy mức overlap. Repo private nên không đính kèm log công khai; số liệu tự ước lượng. |
| 2 | Lặp lại | Khi tổng kết chi tiêu, tôi muốn đối chiếu giao dịch giữa tài khoản chi tiêu, ví điện tử và tiền mặt, để biết số dư và mức chi thực tế. | Người tự quản lý tài chính | Khoảng 150 giao dịch/tháng; tổng kết ~5 phút/tháng, đôi khi chênh lệch hàng trăm nghìn đồng vì quên giao dịch nhỏ. |
| 3 | Tốn thời gian | Khi chuẩn bị mua thực phẩm và đồ dùng cá nhân, tôi muốn xác định trước những món cần mua và tình trạng sẵn có, để tránh phân vân, quên món hoặc đi mua mà hết hàng. | Người sống một mình | Mua sắm khoảng 3 lần/tuần; thường mất thời gian suy nghĩ, đôi lúc quên món hoặc gặp hết hàng. Chưa đo số phút/số lần cụ thể. |
| 4 | Pain từ người khác | Khi làm CCCD trực tiếp, tôi muốn biết đầy đủ giấy tờ và quy trình trước khi đi, để tránh phải quay lại nhiều lần và ảnh hưởng công việc. | Người làm thủ tục hành chính | Từng chờ khoảng 1 tháng để nhận thẻ chuyển về; địa điểm xa, đông người; chỉ được nghỉ 1 ngày/tháng. Chưa xác định số lần thực tế phải bổ sung hồ sơ. |
| 5 | Pain từ người khác | Khi cần họp nhóm học tập, tôi muốn thống nhất lịch phù hợp với các thành viên, để mọi người tham gia đầy đủ và không bị hủy sát giờ. | Nhóm học tập 6 người | Gặp mặt khoảng 1 buổi/2 tuần; thường trùng lịch, phản hồi chậm, đổi lịch hoặc báo vắng sát giờ; trao đổi chủ yếu qua Messenger/Discord. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Giữ 5 vấn đề trên vì gắn với trải nghiệm cá nhân; đã chỉnh vấn đề mua sắm gia đình thành mua sắm cá nhân cho đúng bối cảnh sống một mình.
- Bỏ các gợi ý về tổng hợp tài liệu học tập, lập kế hoạch du lịch và chuẩn bị khám bệnh vì hiện chưa có trải nghiệm/số liệu cụ thể để mô tả chắc chắn.
- Không đưa số liệu giả làm bằng chứng; các khoảng thời gian chưa được đo được ghi rõ là ước lượng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

> **Top 3 tạm đề xuất:** #1, #3, #8 theo số thứ tự vấn đề trong trao đổi ban đầu (tương ứng dòng 1, 2, 5 ở CP1). Cần xác nhận trước khi nộp. Các phút theo bước chưa được đo là giả định cần kiểm chứng.

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Review Pull Request (CP1 #1) | Actor rõ; conflict code gây nghẽn 10–15 phút/PR; dễ phác quy trình và đo thời gian. | Tỷ lệ PR conflict, chất lượng sau merge, khả năng dùng dữ liệu repo private. |
| 2 | Quản lý chi tiêu cá nhân (CP1 #2) | Có ~150 giao dịch/tháng và tình trạng lệch số dư; quy trình đối soát rõ. | Mức lệch chính xác, nguyên nhân chính, tỷ lệ giao dịch bị quên. |
| 3 | Sắp xếp lịch họp nhóm (CP1 #5) | 6 thành viên, khó gặp trực tiếp; ảnh hưởng phối hợp học tập. | Thời gian chốt lịch, tỷ lệ hủy và nguyên nhân không tham gia. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi review PR của đồng đội, tôi muốn hiểu logic mới và phần code đang bị chồng lấn, để quyết định giữ cách triển khai nào mà không làm hỏng chức năng. |
| Actor | Developer/reviewer trong nhóm phát triển phần mềm. |
| Thời điểm / bối cảnh | Khi nhận PR cần merge vào nhánh đang phát triển chức năng. |
| Quy trình hiện tại (3–7 bước) | (1) Nhận PR → (2) Xem diff → (3) Đối chiếu logic với code đang làm → (4) Quyết định cách xử lý conflict → (5) Merge/apply và kiểm tra chạy. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4 khi code overlap; tổng PR conflict khoảng 10–15 phút (chưa đo riêng từng bước). |
| Impact (nếu không giải thì sao) | Chậm merge; có thể giữ logic kém phù hợp hoặc gây regression. |
| Success metric (baseline → target) | Thời gian xử lý PR conflict: 10–15 phút → mục tiêu thử nghiệm ≤7 phút/PR; đo trên 10 PR conflict tiếp theo. |
| Phương án không dùng AI | Quy ước ownership module, PR nhỏ, checklist review và test tự động. |
| Giả thuyết về AI (nếu có) | Tóm tắt thay đổi logic và điểm xung đột để reviewer tự quyết định. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
Nhận PR (chưa đo)
  → Xem diff (chưa đo)
  → [NGHẼN] Đọc và so sánh logic + xử lý overlap
       (tổng PR conflict: 10–15 phút, chưa tách bước)
  → Quyết định giữ/sửa logic (chưa đo)
  → Merge/apply, kiểm tra chạy (chưa đo)
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi tổng kết chi tiêu, tôi muốn đối chiếu giao dịch giữa các nguồn tiền, để biết số dư và mức chi thực tế. |
| Actor | Cá nhân tự quản lý tài chính. |
| Thời điểm / bối cảnh | Cuối tháng hoặc khi cần kiểm tra ngân sách. |
| Quy trình hiện tại (3–7 bước) | (1) Mở tài khoản chi tiêu → (2) Kiểm tra ví điện tử → (3) Nhớ/ghi lại khoản tiền mặt → (4) Đối chiếu các khoản → (5) Ước tính tổng chi. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3–4: khó nhớ giao dịch nhỏ; tổng quá trình khoảng 5 phút/tháng, chưa đo riêng từng bước. |
| Impact (nếu không giải thì sao) | Số liệu tổng kết có thể lệch hàng trăm nghìn đồng, khó đánh giá chi tiêu. |
| Success metric (baseline → target) | Chênh lệch đối soát: đôi khi hàng trăm nghìn đồng → mục tiêu ≤50.000đ/tháng; đo bằng so sánh số dư đầu/cuối kỳ và giao dịch đã ghi. |
| Phương án không dùng AI | Ghi chi tiêu ngay sau giao dịch vào bảng tính, tách tài khoản theo mục đích, đối soát hằng tuần. |
| Giả thuyết về AI (nếu có) | Gợi ý phân loại giao dịch và đánh dấu khoản bất thường để người dùng xác nhận. |
| Cảm nhận nhanh | Rule / Workflow |

Quy trình nháp hiện tại:

```text
Mở lịch sử tài khoản chi tiêu (chưa đo)
  → Kiểm tra ví điện tử (chưa đo)
  → [NGHẼN] Nhớ giao dịch tiền mặt/nhỏ lẻ (chưa đo)
  → Đối chiếu các nguồn (chưa đo)
  → Ước tính tổng chi
     (toàn quy trình ~5 phút/tháng; đôi khi lệch hàng trăm nghìn)
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi cần họp nhóm học tập, tôi muốn thống nhất lịch phù hợp với các thành viên, để mọi người tham gia đầy đủ và không bị hủy sát giờ. |
| Actor | 6 thành viên nhóm học tập. |
| Thời điểm / bối cảnh | Khi chuẩn bị buổi họp trực tiếp, trao đổi qua Messenger/Discord. |
| Quy trình hiện tại (3–7 bước) | (1) Đề xuất buổi họp → (2) Hỏi lịch từng người → (3) Chờ phản hồi → (4) Chọn giờ chung → (5) Xác nhận lại → (6) Xử lý thay đổi/hủy sát giờ. |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2–4: phản hồi chậm và lịch trùng; chưa đo số phút, cần lấy mốc thời gian từ lịch sử chat. |
| Impact (nếu không giải thì sao) | Khó họp trực tiếp; hiện khoảng 2 tuần mới gặp được một buổi, ảnh hưởng phối hợp. |
| Success metric (baseline → target) | Tần suất gặp mặt: khoảng 1 buổi/2 tuần → mục tiêu 1 buổi/tuần; theo dõi lịch họp 4 tuần. |
| Phương án không dùng AI | Bình chọn lịch cố định, deadline xác nhận, lịch dùng chung và quy định báo vắng sớm. |
| Giả thuyết về AI (nếu có) | Tổng hợp các khung giờ từ tin nhắn và đề xuất lịch để nhóm xác nhận. |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
Đề xuất họp trên Messenger/Discord (chưa đo)
  → Hỏi lịch 6 thành viên (chưa đo)
  → [NGHẼN] Chờ phản hồi, xử lý trùng lịch (chưa đo)
  → Chốt giờ (chưa đo)
  → Xác nhận tham gia (chưa đo)
  → Có thể đổi/hủy sát giờ
     (kết quả hiện tại: ~1 buổi gặp mặt/2 tuần)
```

### Card muốn pitch nhất

- Card số: **1 — Review Pull Request** (đề xuất, cần bạn xác nhận).
- Vì sao: Pain rõ trong công việc dev; có baseline thời gian xử lý PR conflict và quy trình tương đối dễ đo.
- Câu hỏi muốn nhóm phản biện: Vấn đề nằm ở việc thiếu thông tin về logic hay ở cách chia module và phối hợp code giữa các developer?

### AI đã phản biện card thế nào

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| PR conflict không phải PR nào cũng gặp; chưa biết tỷ lệ conflict nên chưa thể suy ra tổng thời gian lãng phí mỗi tuần. | Có | Giới hạn metric vào PR có conflict; đề xuất theo dõi tỷ lệ conflict ở các PR tiếp theo. |
| Lệch số dư có thể do thiếu thói quen ghi giao dịch, không nhất thiết cần AI. | Có | Thêm phương án ghi chép/đối soát thủ công trước khi cân nhắc AI. |
| Khó chốt lịch họp có thể do cam kết tham gia, không chỉ do thiếu công cụ. | Có | Bổ sung deadline xác nhận và quy định báo vắng như giải pháp không dùng AI. |

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
| CP1 Scan | Gợi ý cách viết Job Story và hệ thống hóa 5 vấn đề. | Chuẩn hóa cách mô tả actor và dấu hiệu. | Gợi ý mua sắm gia đình không khớp việc sống một mình. | Đổi thành mua sắm cá nhân và cung cấp dữ liệu trải nghiệm. |
| CP2 Problem Card | Phác thảo card, quy trình, metric và phản biện giả định. | Chỉ ra các giả định cần đo và giải pháp không dùng AI. | Chưa có số phút từng bước; target mới là đề xuất. | Cần xác nhận Top 3, kiểm chứng metric trước khi nộp. |
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

- Template và CHECKPOINTS trong repo bài học (đã đối chiếu cấu trúc).
