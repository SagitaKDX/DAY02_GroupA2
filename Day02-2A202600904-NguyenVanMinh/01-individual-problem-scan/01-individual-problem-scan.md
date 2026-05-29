# 01 — Individual Problem Scan

## Scan rộng

> Bài toán giáo viên tổng hợp tình hình học tập và báo phụ huynh


| # | Lăng kính | Problem quan sát được | Ai đang đau? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Lặp lại | Viết nhận xét học tập cho từng học sinh theo cùng một khuôn | Giáo viên | Lặp lại theo tuần/kỳ |
| 2 | Tốn thời gian | Tổng hợp điểm, chuyên cần, bài tập từ nhiều nguồn | Giáo viên | Mất nhiều thời gian mỗi lần báo cáo |
| 3 | AI có thể tốt hơn | Tóm tắt dữ liệu rời rạc thành nhận xét dễ hiểu | Giáo viên | Cần viết lại thành văn bản tự nhiên |
| 4 | Pain từ người khác | Phụ huynh hỏi lại tiến độ, điểm mạnh/yếu của con | Giáo viên, phụ huynh | Câu hỏi lặp lại, cần phản hồi nhanh |
| 5 | Lặp lại | Tạo báo cáo định kỳ cho nhiều lớp/học sinh | Giáo viên chủ nhiệm | Workload tăng theo số học sinh |

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Giáo viên tổng hợp tình hình học tập và báo phụ huynh | Workflow rõ nhất, có metric rõ, phù hợp HITL | Cần chuẩn hóa baseline thời gian |
| 2 | Bài toán trong bệnh viện | Pain thật nhưng rủi ro và scope cao hơn | Cần dữ liệu y tế và tri thức chuyên môn |
| 3 | Theo dõi và nhắc tiến độ học tập | Có repeatability cao | Dễ trượt sang reminder tool, chưa chắc cần AI |

## Problem Card #1 — Giáo viên báo phụ huynh

**Problem 1 câu:**
Giáo viên mất nhiều thời gian để tổng hợp dữ liệu học tập thành nhận xét cá nhân hóa cho phụ huynh, đặc biệt ở bước viết narrative.

**Actor:**
Giáo viên chủ nhiệm hoặc giáo viên bộ môn.

**Thời điểm / bối cảnh:**
Cuối tuần, cuối tháng hoặc cuối kỳ khi cần gửi báo cáo tiến độ học tập.

**Current workflow:**

```text
1. Lấy điểm số, bài tập, chuyên cần
2. Xem ghi chú hành vi / thái độ học tập
3. Xác định học sinh cần chú ý
4. Viết nhận xét cá nhân hóa cho từng học sinh
5. Rà lại nội dung và format
6. Gửi cho phụ huynh qua sổ liên lạc / app / tin nhắn
```

**Bước nghẽn nhất:**
Bước 4, vì giáo viên phải tự biến dữ liệu rời rạc thành câu chữ phù hợp từng học sinh.

**Impact:**
Mỗi lần báo cáo tốn nhiều công sức, feedback dễ ngắn và thiếu cá nhân hóa, phụ huynh khó theo dõi tiến độ thật.

**Success metric:**
Giảm thời gian tạo báo cáo xuống dưới 20 phút/lớp; tăng tỷ lệ nhận xét cá nhân hóa; không tăng số lần phụ huynh phải hỏi lại.

**Non-AI alternative:**
Template + rubric + form nhập dữ liệu chuẩn.

**AI hypothesis:**
AI có thể draft nhận xét và tóm tắt xu hướng, giáo viên vẫn review trước khi gửi.

**Quick gut:**
Workflow.

### Draft current workflow

```text
CURRENT STATE — khoảng 60 phút / 1 lớp báo cáo

[1 Lấy dữ liệu học tập: 10']
→ [2 Xem chuyên cần + ghi chú: 10']
→ [3 Xác định học sinh cần chú ý: 10']
→ [4 Viết nhận xét cá nhân hóa: 20']  <-- bottleneck
→ [5 Rà lại format: 5']
→ [6 Gửi báo cáo: 5']
```

### Draft future workflow

```text
FUTURE STATE — khoảng 20 phút / 1 lớp báo cáo

[1 Gom dữ liệu vào form/template chuẩn: 3']  -- Rule/process
→ [2 AI tóm tắt điểm mạnh/yếu/xu hướng: 2']   -- Workflow
→ [3 AI draft nhận xét cá nhân hóa: 5']       -- Workflow
→ [4 Giáo viên review + edit: 8']             -- Human boundary
→ [5 Giáo viên gửi báo cáo: 2']

Fallback: draft không đạt thì bỏ và viết lại theo template.
```

## Problem Cards #2 và #3 — tóm tắt

| Card | Actor | Bottleneck | Metric | Quick gut | Vì sao chưa chọn làm #1 |
|---|---|---|---|---|---|
| Bệnh viện | Y tá | Hỏi thông tin lặp lại, gợi ý lịch khám | Giảm thời gian hỏi đáp | Workflow | Rủi ro và boundary cao hơn |
| Theo dõi tiến độ học tập | Giáo viên | Nhắc và cập nhật lặp lại | Giảm công thủ công | Rule / Workflow | Có thể giải bằng template trước |

---