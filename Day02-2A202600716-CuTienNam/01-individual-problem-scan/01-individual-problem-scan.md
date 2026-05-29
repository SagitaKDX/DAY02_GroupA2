# BÀI NỘP CÁ NHÂN (Phase 0, 1, 2)
**Học viên:** Cù Tiến Nam - 2A202600716

---

## Phase 0 — Worked Example

**Self-check:**
- [x] Tôi hiểu nhóm chỉ chọn **candidate problem**, không chọn ngay Problem Statement.
- [x] Tôi hiểu deep-dive gồm validation, research, workflow, metric, PS và AI decision.

---

## Phase 1 — Individual Scan (Scan 5+ problems)

Danh sách 5 vấn đề từ trải nghiệm thực tế (quản lý đội bóng phong trào, thể thao):

| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại, Tốn thời gian | Đối soát quỹ đội bóng sau trận tốn nhiều thời gian lội tin nhắn Zalo và app ngân hàng. | Đội trưởng / Bầu show | Mất 30-45 phút đếm người, cộng sổ, dễ sai sót thất thoát quỹ. |
| 2 | Tốn thời gian, Pain từ người khác | Việc đặt lịch tập phục hồi chấn thương mất thời gian nhắn tin qua lại, người tập dễ bỏ dở bài tập ở nhà. | Cầu thủ phong trào | Chờ phản hồi chốt lịch vài tiếng, tỷ lệ duy trì tập ở nhà chỉ đạt 30-40%. |
| 3 | Tốn thời gian | Dán mắt xem lại video 90 phút để dò tìm và cắt highlight/tình huống chiến thuật. | HLV / Nhân viên Media | Mất 2-3 tiếng xử lý cho mỗi video trận đấu, cực kỳ mỏi mắt và lặp lại. |
| 4 | Pain từ người khác | Theo dõi tình trạng trang thiết bị (bóng, áo bib, nước) mỗi trận hay bị thiếu sót, quên đồ. | Hậu cần / Đội trưởng | Hay bị mất áo bib, quên bóng do không ai nhớ người cầm cuối cùng. |
| 5 | Lặp lại | Thống kê phong độ, số kiến tạo, bàn thắng của cầu thủ sau mỗi giải đấu bằng tay. | Quản lý đội | Ghi chép ra Excel thủ công, dễ quên nếu không cập nhật ngay sau trận. |

---

## Phase 2 — Top 3 Problem Cards + Draft Workflow

### Chọn Top 3
| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Cắt highlight và tổng hợp chiến thuật (Video) | Pain point cực kỳ rõ, bottleneck tiêu tốn hàng giờ đồng hồ mỗi tuần. | Công nghệ AI Vision (nhận diện bóng đá) có dễ tích hợp và độ chính xác ra sao. |
| 2 | Quản lý và đối soát quỹ đội bóng | Workflow đối chiếu rõ ràng, có metric thời gian cụ thể, ảnh hưởng trực tiếp đến tài chính. | Đội trưởng thao tác upload ảnh/CSV có dễ hơn việc tự nhìn màn hình ghi sổ không. |
| 3 | Đặt lịch & theo dõi tập phục hồi | Giúp tăng hiệu quả rõ rệt cho người bệnh, metric tỷ lệ duy trì có thể đo lường tốt. | Agent tự động book lịch Zalo có thể gây khó chịu nếu không hiểu ngữ cảnh phức tạp. |

---

### Problem Card #1: Cắt highlight và tổng hợp tình huống chiến thuật sau trận

**Problem 1 câu:** Nhân viên media/HLV mất hàng giờ đồng hồ dán mắt xem lại toàn bộ video 90 phút của trận đấu để dò tìm timestamp và cắt thủ công các tình huống highlight/chiến thuật.

**Actor:** Huấn luyện viên hoặc nhân viên Media của đội bóng phong trào/bán chuyên.

**Thời điểm / bối cảnh:** Sau mỗi trận đấu cuối tuần.

**Current workflow:**
1. Đặt máy quay toàn bộ trận đấu.
2. Chép file video 90 phút vào máy tính.
3. Dán mắt xem lại video từ đầu đến cuối (hoặc tua nhanh).
4. Ghi chú timestamp các tình huống đáng chú ý. (Bottleneck - 90 phút)
5. Cắt clip thủ công và ghép thành video highlight. (Bottleneck - 60 phút)
6. Xuất file và đăng tải.

**Bottleneck:** Bước dán mắt xem lại toàn bộ video 90 phút để dò tìm timestamp và thao tác cắt clip thủ công tốn quá nhiều sức lực và độ lặp lại cao.

**Impact:** Mất 2-3 tiếng để ra được 1 video highlight. Việc này khiến media bị nản và video thường bị trả chậm sau 1-2 ngày.

**Success metric:** Giảm tổng thời gian xử lý và cắt video từ 2-3 tiếng/bản xuống dưới 30 phút/bản. Không bỏ sót các tình huống quan trọng (bàn thắng, kiến tạo, thẻ phạt).

**Non-AI alternative:** Phân công 1 người đứng ngoài sân cầm điện thoại bấm giờ (note lại phút thứ mấy có bàn thắng) để về nhà chỉ việc xem đúng đoạn đó.

**AI hypothesis:** Dùng mô hình AI Computer Vision (nhận diện bóng đá) phân tích file video đầu vào, tự động nhận diện các sự kiện (bàn thắng, sút, phạm lỗi) và xuất ra danh sách timestamp cùng đoạn clip đã cắt sẵn. HLV chỉ việc review và ghép lại.

**Quick gut:** [x] Workflow

#### Draft Current Workflow
```text
CURRENT STATE — 150 phút

[1 Quay video & Chép file: 10'] 
→ [2 Dán mắt xem lại & dò timestamp: 90']  <-- bottleneck
→ [3 Thao tác cắt & ghép clip: 40']  <-- bottleneck
→ [4 Export & Đăng tải: 10']
```

#### Draft Future Workflow
```text
FUTURE STATE — 25 phút

[1 Chép file & Upload lên hệ thống AI: 5'] 
→ [2 AI xử lý video và xuất danh sách Clip/Timestamp: 5' (chờ máy chạy)] 
→ [3 Người dùng review lại danh sách Clip và chọn đoạn ưng ý: 10'] <-- human boundary
→ [4 AI tự động ghép clip đã chọn & Export: 5']

Fallback: AI nhận diện trượt bàn thắng → Người dùng tự tua lại xem và cắt thủ công đoạn bị thiếu.
```

---

### Problem Card #2: Quản lý nhân sự và đối soát quỹ đội bóng hằng tuần

**Problem 1 câu:** Người quản lý đội bóng tốn nhiều thời gian đối soát quỹ thủ công vì dữ liệu phân mảnh giữa ảnh chụp/file CSV ngân hàng và danh sách điểm danh Zalo, dẫn đến dễ nhầm lẫn tên và số tiền khi có các giao dịch bất thường (chuyển thiếu, chuyển hộ).

**Actor:** Đội trưởng / "Bầu show" của đội bóng phong trào.

**Thời điểm / bối cảnh:** Sau khi trận đấu kết thúc, cần tổng kết thu chi dựa trên dữ liệu giao dịch ngân hàng.

**Current workflow:**
1. Tạo bình chọn điểm danh trên Zalo trước trận.
2. Tổ chức thi đấu.
3. Chụp ảnh màn hình lịch sử giao dịch (hoặc xuất file CSV) từ app ngân hàng.
4. Mở 2 màn hình song song để đối chiếu chéo tên trên Zalo và nội dung chuyển khoản. (Bottleneck - 15 phút)
5. Ghi sổ thủ công chốt ai đã đóng tiền, ai nợ. (Bottleneck - 15 phút)
6. Thông báo lại lên nhóm.

**Bottleneck:** Bước đối soát tài chính sau trận. Nội dung chuyển khoản lộn xộn, tên Zalo và tên ngân hàng không khớp, thường xuyên có trường hợp 1 người đóng hộ nhiều người.

**Impact:** Mất 30-45 phút mỗi trận chỉ để đếm người và cộng sổ. Sai sót dẫn đến thất thoát quỹ hoặc gây hiểu lầm với anh em trong đội.

**Success metric:** Giảm thời gian đếm người và cộng sổ từ 30-45 phút/trận xuống dưới 10 phút/trận. Tỷ lệ sai sót và thất thoát quỹ đội giảm về 0%.

**Non-AI alternative:** Dùng quỹ đóng "chết" hàng tháng (đóng họ) không thu lẻ tẻ theo trận, hoặc dùng ứng dụng Splitwise để tự ai nấy nhập (nhưng khó đồng bộ).

**AI hypothesis:** Đội trưởng upload ảnh màn hình giao dịch (hoặc CSV) và copy danh sách Zalo vào tool. AI (tích hợp OCR và LLM) sẽ đọc ảnh, trích xuất dữ liệu, tự động suy luận để map với danh sách Zalo (xử lý cả tên lóng và đóng hộ). AI trả ra bảng đối chiếu dự kiến, Đội trưởng phải tự duyệt lại trước khi chốt sổ.

**Quick gut:** [x] Workflow

#### Draft Current Workflow
```text
CURRENT STATE — 35 phút

[1 Điểm danh qua Zalo: 5'] 
→ [2 Chụp ảnh màn hình/Xuất CSV ngân hàng: 5'] 
→ [3 Đối chiếu chéo Zalo & Ngân hàng thủ công: 15'] <-- bottleneck
→ [4 Ghi sổ Excel/Giấy thủ công: 5'] <-- bottleneck
→ [5 Đòi nợ & Báo cáo: 5']
```

#### Draft Future Workflow
```text
FUTURE STATE — 10 phút

[1 Upload ảnh bill/CSV & copy text Zalo vào hệ thống: 2'] 
→ [2 AI (OCR) trích xuất Tên, Số tiền, Nội dung: 1'] 
→ [3 AI tự suy luận, map tên người gửi với tên lóng Zalo & nhận diện ca đóng hộ: 2'] 
→ [4 Đội trưởng duyệt bảng đề xuất của AI, tự sửa thủ công các ca AI đánh dấu "không chắc chắn": 3'] <-- human boundary / HITL
→ [5 Bấm nút xuất báo cáo / nhắc nợ: 2']

Fallback: AI nhận diện nhầm số tiền hoặc không hiểu nội dung (ví dụ: chuyển thiếu) → AI highlight đỏ dòng đó để Đội trưởng tự đối chiếu và sửa tay.
```

---

### Problem Card #3: Tự động hóa theo dõi tuân thủ điều trị (Compliance Tracking) tại nhà cho bệnh nhân chấn thương

**Problem 1 câu:** Việc thiếu hệ thống theo dõi và phân tích quá trình tự tập phục hồi tại nhà khiến người bệnh dễ nản chí, tập sai tư thế, dẫn đến hỏng phác đồ điều trị và làm giảm uy tín của phòng khám.

**Actor:** Chuyên viên vật lý trị liệu (người cần theo dõi tiến độ) và Cầu thủ phong trào (người tập).

**Thời điểm / bối cảnh:** Quá trình phục hồi kéo dài hàng tháng tại nhà giữa các buổi khám trực tiếp.

**Current workflow:**
1. Khách đến phòng khám nhận phác đồ điều trị.
2. Chuyên viên dặn dò tự tập ở nhà qua lời nói hoặc tờ giấy in.
3. Khách tự về nhà tập (thường lười biếng hoặc tập sai tư thế). (Bottleneck - thiếu kỷ luật)
4. Lễ tân thỉnh thoảng nhắn tin Zalo hỏi thăm thủ công.
5. Cuối tháng khách lên tái khám, bác sĩ mới phát hiện tập sai hoặc bỏ tập.

**Bottleneck:** Không có cơ chế giám sát và feedback (phản hồi) tự động hằng ngày. Việc phòng khám nhắn tin hỏi thăm/hối thúc thủ công tốn quá nhiều nguồn lực của lễ tân và kém hiệu quả.

**Impact:** Tỷ lệ duy trì liệu trình tại nhà giảm mạnh (chỉ còn 30-40%). Kết quả điều trị kém khiến khách hàng không quay lại hoặc không giới thiệu người mới, phòng khám mất doanh thu dài hạn.

**Success metric:** Tăng tỷ lệ duy trì bài tập (Compliance rate) sau 4 tuần lên trên 80%. Giảm thời gian lễ tân nhắn tin hỏi thăm thủ công xuống 0 phút.

**Non-AI alternative:** Thiết lập hệ thống Zalo OA nhắn tin nhắc nhở tự động (chỉ nhắc chứ không kiểm tra được chất lượng tập). Phát sổ tay checklist bắt bệnh nhân tự đánh dấu mỗi ngày.

**AI hypothesis:** Hệ thống AI Workflow tự động nhắn tin Zalo nhắc lịch mỗi ngày. Khi bệnh nhân gửi video quay cảnh tập ở nhà, AI (Computer Vision) sẽ phân tích form (góc gập gối, tư thế) và LLM phân tích text mô tả mức độ đau để phản hồi tự động. Nếu phát hiện cờ đỏ (Red flag: tập sai góc nguy hiểm, kêu đau bất thường), AI sẽ đẩy thông báo khẩn cấp cho bác sĩ can thiệp.

**Quick gut:** [x] Workflow (Kết hợp Rule nhắc nhở + AI phân tích video)

#### Draft Current Workflow
```text
CURRENT STATE — Tỷ lệ drop cao, hỏng phác đồ

[1 Chuyên viên dặn dò tự tập ở nhà: 2'] 
→ [2 Khách tự nhớ để tập: Dễ bỏ quên/tập sai] <-- bottleneck
→ [3 Lễ tân thỉnh thoảng nhắn Zalo nhắc tay: 10'] <-- bottleneck
→ [4 Tái khám cuối tháng phát hiện cơ không phục hồi]
```

#### Draft Future Workflow
```text
FUTURE STATE — Theo dõi 24/7, tỷ lệ duy trì cao

[1 Khách tập và quay video gửi Zalo Bot: 5'] 
→ [2 AI Vision phân tích tư thế & LLM phân tích text mô tả cảm giác đau: 2'] 
→ [3 Nếu đúng form: AI tự gửi lời khen & tick hoàn thành bài tập: 0']
→ [4 Nếu sai form/Kêu đau: AI gắn cờ đỏ, đẩy thẳng notification cho chuyên viên vào chat trực tiếp: 1'] <-- human boundary

Fallback: AI không đọc được video do mờ tối hoặc khách không chịu quay video → Chuyển luồng về nhắc nhở cơ bản (Rule) và nhắc Lễ tân gọi điện.
```

---

### Card muốn pitch nhất

**Card tôi muốn pitch nhất:** Đặt lịch và theo dõi tiến độ tập phục hồi chấn thương (Card #3).

**Vì sao (Đánh giá dưới góc nhìn AI Product):** 
- **Business Impact cực lớn:** Tỷ lệ bỏ dở bài tập ở nhà (churn rate) trong phục hồi chức năng là nỗi đau cốt lõi của các phòng khám và gây hậu quả trực tiếp đến người bệnh.
- **Không gian tranh luận lý tưởng (Trade-off):** Bài toán này mở ra cơ hội tranh luận rất hay cho phần làm nhóm: "Liệu chúng ta có thực sự cần một AI Agent để chat đặt lịch không, hay chỉ cần dùng link Calendly (Rule) là đủ?".
- **Mở rộng được luồng giá trị (Value chain):** Không chỉ giải quyết khâu "Đặt lịch" (Front-desk), AI còn can thiệp vào khâu "Theo dõi" (Workflow nhắc nhở) và "Kiểm tra" (AI Vision phân tích form tập qua video người dùng gửi). 

**Câu hỏi tôi muốn nhóm challenge:** 
1. Việc dùng AI Agent để chat đặt lịch có bị "overkill" (làm quá vấn đề) so với việc dùng tool truyền thống như Calendly không? 
2. Nếu người bệnh gửi video nhưng tập sai tư thế, AI có đủ khả năng và thẩm quyền y khoa để phát hiện không, hay bắt buộc phải đẩy (fallback) cho bác sĩ xem lại bằng mắt thường? (Điểm này rất quan trọng để xác định Human Boundary).
