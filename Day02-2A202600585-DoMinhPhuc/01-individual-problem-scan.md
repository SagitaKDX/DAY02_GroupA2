## Scan rộng

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại | Theo dõi chi tiêu cá nhân lẻ tẻ hằng ngày (tiền cafe, gửi xe, ăn trưa) rất mất thời gian nên thường bị bỏ sót. | Dân văn phòng, người trẻ | Cuối tháng nhìn tài khoản thâm hụt nhưng không nhớ tiền đi đâu, lười mở app nhập tay. |
| 2 | Lặp lại | Mỗi chiều phải nghĩ "Tối nay ăn gì?" dựa trên những nguyên liệu còn sót lại lộn xộn trong tủ lạnh. | Người nấu ăn chính trong nhà | Mất 15-20 phút suy nghĩ mỗi ngày, đồ ăn trong tủ hay bị héo/hỏng do quên. |
| 3 | Tốn thời gian |  Đứng trước tủ quần áo chật cứng nhưng không biết mặc gì cho hợp thời tiết và lịch trình hôm nay. | Sinh viên, dân văn phòng | Mất 15 phút thử ra thử vào mỗi sáng, nhiều đồ mua về để xó không đụng tới. |
| 4 | Pain từ người khác | Lưu hàng chục link bài viết, video hay vào bookmark để "đọc sau" nhưng cuối cùng không bao giờ đụng đến. | Người thích học hỏi (nhưng hay trì hoãn) | Danh sách "Read later" dài hàng trăm link, mỗi lần mở ra thấy ngợp lại đóng vào. |
| 5 | Tốn thời gian | Lên lịch trình du lịch chi tiết cho nhóm bạn (ăn gì, chơi ở đâu, di chuyển thế nào) từ hàng loạt review trên mạng. | Trưởng nhóm du lịch | Tốn hàng buổi tối đọc review, cắm pin trên Google Maps và sắp xếp lộ trình. |
| 6 | AI có thể tốt hơn | So sánh giá và săn sale một món đồ công nghệ/gia dụng trên nhiều sàn TMĐT (Shopee, Lazada, Tiki) để mua được giá tốt nhất. | Người hay mua sắm online | Tốn thời gian mở nhiều app soi giá, canh mã giảm giá thủ công. |
| 7 | AI có thể tốt hơn | Tóm tắt nội dung hội thoại dài: Bị add vào một group chat dự án hoặc nhóm du lịch đang cãi nhau/bàn luận sôi nổi cả trăm tin nhắn chưa kịp đọc. | Người bị miss thông tin | Phải cuộn ngược lên đọc từng tin nhắn để hiểu context, mất 10 phút lướt. |
| 8 | Lặp lại | Sắp xếp lịch họp với bên ngoài: Tìm một khung giờ trống chung cho 3-4 người khác công ty (không chung Google Calendar). | Freelancer, PM, Engineer đi họp chéo | Tốn nhiều tin nhắn qua cho mỗi cuộc họp. |
| 9 | Pain từ người khác | Tìm file/tài liệu trôi nổi: Đồng nghiệp/bạn bè thường xuyên nhắn hỏi xin lại link một file doc, ảnh design, hay quyết định cũ đã từng gửi đâu đó. | Người làm việc nhóm | Mất 5-10 phút bới lại lịch sử chat Zalo/Slack |
| 10 | Pain từ người khác | Xử lý form điền lỗi: Người dùng hoặc khách hàng điền form thông tin (đăng ký, support) bị sai định dạng, thiếu chữ, sai lỗi chính tả. | Người tiếp nhận data | Phải chạy script thủ công hoặc sửa bằng tay từng dòng trên Google Sheets trước khi dùng được data. |

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Quản lý chi tiêu | Workflow rõ, metric tốt, kết hợp Rule và AI mượt mà | Đôi khi thanh toán bằng một số ứng dụng sẽ không có tin nhắn sms, user sẽ phải reply sau mỗi khi thanh toán |
| 2 | Gợi ý món ăn | Pain lặp lại hằng ngày, AI giải quyết tốt constraint | Công thức sinh ra có hợp khẩu vị và dễ nấu cho từng đối tượng hay không |
| 3 | Xử lý Bookmark | Nhiều người đau, AI giúp tóm tắt và push học chủ động | Tóm tắt có làm mất context tài liệu chuyên sâu hay không |

## Problem Card #1 — Quản lý chi tiêu

**Problem 1 câu:**  
Cá nhân lười mở app nhập form lắt nhắt cho từng khoản chi, thường để dồn đến cuối tuần rồi quên mất mục đích chi tiêu, dẫn đến mất kiểm soát dòng tiền.

**Actor:**  
Người trẻ, dân văn phòng muốn quản lý tài chính.

**Thời điểm / bối cảnh:**  
Hằng ngày ngay khi phát sinh giao dịch, và cuối tuần khi cần đối soát.

**Current workflow:**

```text
1. Quẹt thẻ / nhận SMS trừ tiền.
2. Tự nhủ "lát rảnh sẽ nhập".
3. Cuối tuần mở lịch sử app ngân hàng.
4. Cố nhớ lại khoản này là vì mục đích gì.
5. Mở app điền form (số tiền, ngày, danh mục, ghi chú) bằng tay.
```

**Bottleneck:**  
Bước 4 và 5 — vắt óc nhớ lại ngữ cảnh (context) của dòng tiền cũ và thao tác điền form thủ công làm đứt gãy sự kiên nhẫn.

**Impact:**  
Mất 25 phút mỗi tuần rà soát trong mệt mỏi; người dùng dễ bỏ cuộc giữa chừng, cuối tháng thâm hụt ngân sách mà không rõ nguyên nhân.

**Success metric:**  
Giảm thời gian ghi chép xuống dưới 10 giây/giao dịch; tỷ lệ phân loại đúng danh mục đạt trên 90%.

**Non-AI alternative:**  
Chỉ dùng tính năng báo cáo có sẵn của app ngân hàng (nhưng không hiển thị chi tiết mua món gì).

**AI hypothesis:**  
Rule tự động lấy số tiền từ thông báo, AI hỏi nhanh người dùng về ngữ cảnh, người dùng trả lời, AI tự động gán đúng danh mục và điền vào bảng tính.

**Quick gut:**  
Workflow.

### Draft current workflow

```text
CURRENT STATE — 25 phút/tuần

[1 Quẹt thẻ / Nhận SMS: 0']
→ [2 Quên nhập ngay lúc đó: 0']
→ [3 Mở lịch sử bank cuối tuần: 5']
→ [4 Cố nhớ lại context: 10']  <-- bottleneck
→ [5 Mở app điền tay: 10']
```

### Draft future workflow

```text
FUTURE STATE — Khoảng 5-10 giây/giao dịch

[1 Rule bắt SMS gửi số liệu về Bot: 0']
→ [2 Bot hỏi ngay mục đích: 0']
→ [3 User reply ngắn gọn: 5'']  <-- human boundary
→ [4 AI ghép data, gán category và đẩy vào Sheets: 1'']
→ [5 User xem báo cáo cuối tháng: 0']

Fallback: AI phân loại sai danh mục → User vào Google Sheets tự sửa lại ô đó.
```

## Problem Card #2 — Gợi ý món ăn

**Problem 1 câu:**  
Mỗi chiều đứng trước tủ lạnh lộn xộn, người nấu ăn vắt óc suy nghĩ không biết ghép các nguyên liệu thừa thành món gì, dẫn đến mất thời gian tra cứu và lãng phí thực phẩm.

**Actor:**  
Người nấu ăn chính trong gia đình hoặc cá nhân sống một mình tự nấu nướng.

**Thời điểm / bối cảnh:**  
Khoảng 5-6h chiều sau giờ làm, cơ thể mệt mỏi.

**Current workflow:**

```text
1. Mở tủ lạnh rà soát xem còn sót lại nguyên liệu gì.

2. Tự suy nghĩ xem ghép các nguyên liệu này thành món gì.

3. Lên mạng tìm kiếm công thức

4. Lọc qua các bài viết SEO dài dòng để lấy được cách làm.

5. Bắt đầu nấu.
```

**Bottleneck:**  
Bước 2 — Quá trình tư duy kết hợp nguyên liệu ngẫu nhiên (constraint-solving) vượt quá khả năng của não bộ sau một ngày dài làm việc.

**Impact:**  
Tốn khoảng 20 phút mệt mỏi mỗi ngày chỉ để chốt thực đơn; thường xuyên phải vứt bỏ rau củ/thịt hỏng vì quên không dùng, gây lãng phí.

**Success metric:**  
Rút ngắn thời gian chốt món ăn xuống dưới 3 phút; giảm 50% lượng thực phẩm quá hạn/hư hỏng phải vứt đi hằng tháng.

**Non-AI alternative:**  
Lên thực đơn cố định hàng tuần và đi chợ 1 lần (nhưng cách này quá cứng nhắc, khó xử lý linh hoạt phần nguyên liệu dùng dở dang).

**AI hypothesis:**  
AI thực hiện Constraint-based Generation: nhận input là danh sách nguyên liệu lộn xộn từ user, trả về 1-2 công thức tối ưu và ngắn gọn nhất.

**Quick gut:**  
Workflow.

### Draft current workflow

```text
CURRENT STATE — 20 phút

[1 Nhìn đồ thừa trong tủ lạnh: 2']
→ [2 Vắt óc nghĩ món để ghép: 10']  <-- bottleneck
→ [3 Search công thức trên mạng: 3']
→ [4 Đọc lướt bài SEO lấy cách làm: 5']
→ [5 Bắt đầu nấu]
```

### Draft future workflow

```text
FUTURE STATE — 3 phút

[1 Nhập nhanh nguyên liệu vào chat: 1']
→ [2 AI tính toán và xuất 2 lựa chọn món + công thức tóm tắt: 1']
→ [3 User đọc, chốt món và nấu: 1']  <-- human boundary

Fallback: AI gợi ý món ăn vô lý hoặc không hợp khẩu vị → User yêu cầu gợi ý lại hoặc tự nấu theo thói quen cũ.
```

## Problem Card #3 — Xử lý Bookmark

**Problem 1 câu:**  
Cá nhân lưu quá nhiều link bài viết dài vào Bookmark nhưng luôn trì hoãn không mở ra vì bị ngợp thông tin, dẫn đến lãng phí kiến thức đã cất công sưu tầm.

**Actor:**  
Dân công nghệ, sinh viên, người thích học hỏi nhưng có quỹ thời gian eo hẹp.

**Thời điểm / bối cảnh:**  
Khi lướt web thấy bài hay cần lưu lại, hoặc lúc rảnh rỗi (cuối tuần) định lôi sách báo ra đọc.

**Current workflow:**

```text
1. Thấy bài báo/tài liệu hay trên mạng.

2. Bấm lưu vào Notion / Bookmark của trình duyệt.

3. Cuối tuần rảnh rỗi mở danh sách ra xem.

4. Thấy có quá nhiều thứ cần đọc và không biết bắt đầu từ đâu.

5. Đóng tab bỏ cuộc, quay ra lướt mạng xã hội cho nhẹ đầu.
```

**Bottleneck:**  
Bước 4 — Rào cản tâm lý cực lớn khi phải đối mặt với một khối lượng văn bản khổng lồ mà chưa biết nội dung có xứng đáng để đầu tư thời gian hay không.

**Impact:**  
Lãng phí nguồn tri thức; tạo áp lực tâm lý ngầm (sự tội lỗi vì trì hoãn); các link cũ bị lãng quên mãi mãi.

**Success metric:**  
Tăng tỷ lệ xử lý backlog (đọc hết bản tóm tắt hoặc dọn dẹp xóa bỏ link) từ dưới 5% lên trên 30% mỗi tuần.

**Non-AI alternative:**  
Cài đặt lịch "Giờ đọc tài liệu" cố định mỗi tối.

**AI hypothesis:**  
AI làm nhiệm vụ Summarization & Push (Tóm tắt và Đẩy chủ động): Workflow tự động bốc 1 bài báo cũ, AI tóm tắt siêu ngắn gọn và gửi thẳng vào tin nhắn mỗi ngày.

**Quick gut:**  
Workflow.

### Draft current workflow

```text
[1 Lưu bài viết hay: 1']
→ [2 Dồn đống link trong list]
→ [3 Mở ra xem lúc rảnh: 2']
→ [4 Thấy ngợp chữ: 2']  <-- bottleneck
→ [5 Đóng tab bỏ cuộc: 0']
```

### Draft future workflow

```text
FUTURE STATE — Tiêu thụ chủ động

[1 Lưu bài vào list: 1']
→ [2 Script tự động kéo 1 vài link cũ nhất vào mỗi sáng: 0']
→ [3 AI đọc text và tóm tắt thành các bullet points: 0']
→ [4 Bot đẩy tin nhắn tóm tắt theo giờ cố định : 0']
→ [5 User đọc lướt 3 ý, chốt đọc bản full hoặc xóa link: 2']  <-- human boundary

Fallback: AI tóm tắt quá sơ sài hoặc sai ngữ cảnh → User vẫn có sẵn link gốc đính kèm trong tin nhắn để tự click vào đọc nếu chủ đề hấp dẫn.
```

---