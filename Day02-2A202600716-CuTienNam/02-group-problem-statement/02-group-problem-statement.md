# BÀI NỘP NHÓM (Phase 3-6)
**Nhóm:** (Điền tên nhóm / Tên các thành viên)

---

## Phase 3 — Group Convergence

**Nhóm 5 người, mỗi người share top 3. Tổng cộng 14 candidates.**

| Cluster | Candidate examples | Pattern chung |
|---|---|---|
| Báo cáo / Phân tích dữ liệu | Check đánh giá Shopee thành checklist (Minh), Tổng hợp tiến độ học sinh (Văn Minh), Tổng hợp bài viết (Phúc), Highlight trận đấu (Nam) | Đọc, gom nhóm, tóm tắt khối lượng lớn dữ liệu text/thông tin rời rạc thành báo cáo/insight. |
| Y tế / Sức khỏe | Tư vấn lịch khám (Văn Minh), Lịch phục hồi chấn thương (Nam), Gợi ý thuốc cho bác sĩ (Điệp), Nhắc lịch tiêm ngừa (Điệp) | Matching thông tin y tế, lên lịch và cảnh báo rủi ro (tương tác thuốc). |
| Trợ lý cá nhân / Đời sống | Sắp xếp lịch trình (Minh), Gợi ý nấu ăn/đi chợ (Phúc), Gợi ý phối đồ (Phúc), Quản lý quỹ đội bóng (Nam) | Tối ưu hóa thời gian và nguồn lực cá nhân dựa trên context hiện tại. |
| Tìm kiếm / Quản lý tri thức | Search bài DSA (Minh), Note tài liệu từ keyword ra file .md (Điệp) | Tìm kiếm ngữ nghĩa và tự động cấu trúc hóa kiến thức. |

### Shortlist và score

Nhóm chọn 3 bài toán tiềm năng nhất để chấm điểm.

| Candidate | Actor rõ | Workflow rõ | Pain có evidence | Impact đo được | Làm trong lab | So sánh R/W/A được | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| Phân tích review Shopee (Minh) | 5 | 5 | 5 | 5 | 5 | 5 | 4 | **34** |
| Gợi ý thuốc cho bác sĩ (Điệp) | 4 | 4 | 5 | 3 | 2 | 4 | 2 | **24** |
| Tổng hợp tiến độ học sinh (Văn Minh) | 4 | 4 | 4 | 4 | 4 | 4 | 5 | **29** |

**Nhóm chốt chọn:** **Phân tích đánh giá đơn hàng (Sentiment Analysis).**

**Vì sao chọn:**
- Có workflow và data rõ ràng (export được file Excel/CSV từ sàn).
- Impact đo được ngay bằng số giờ tiết kiệm được của nhân viên Quality Analytics (QA) và độ chính xác phân loại.
- Dễ dàng so sánh ranh giới giữa Rule-based (tìm keyword) và LLM Workflow (hiểu ngữ cảnh).
- Không vướng rủi ro lớn về đạo đức/pháp lý như bài toán Y tế (Gợi ý thuốc).

**Vì sao không chọn các bài khác:**
- *Gợi ý thuốc:* Domain quá chuyên sâu, rủi ro fatal error cao (chết người), không thể test an toàn trong lab.
- *Tổng hợp tiến độ học sinh:* Gom data từ nhiều nguồn (điểm số, thái độ, bài tập) khá phân mảnh, khó xin data thật của học sinh để làm lab.

---

## Phase 4 — Quick Validation + Research giải pháp

Nhóm hỏi nhanh 3 người đang kinh doanh online / Store Manager / QA.

| Nguồn | Số người | Tín hiệu xác nhận | Tín hiệu phản bác | Nhóm sửa problem thế nào |
|---|---:|---|---|---|
| Phỏng vấn chủ shop / QA | 3 | 2/3 shop tốn rất nhiều thời gian đọc review 1-3 sao để tìm lỗi vận chuyển hay lỗi sản phẩm. | 1 shop nhỏ bảo lượng đơn ít, tự đọc ngày 15p là xong, không cần AI. | **Thu hẹp problem:** Nhắm tới các Store Manager/QA quản lý gian hàng lớn (Mall) hoặc dùng trong đợt Mega Sale khi data bị quá tải. |
| Quan sát công cụ hiện tại | N/A | Các sàn chỉ có biểu đồ chung (tổng số sao), không có tóm tắt lý do. | Các công cụ social listening (như Buzzmetrics) thì quá đắt cho 1 shop bán lẻ. | **Xác định khoảng trống:** Cần một tool xử lý text giá rẻ, tập trung vào trích xuất lý do (aspect-based sentiment) thay vì chỉ đếm positive/negative. |

**Insight sau validation:**
Pain thật không nằm ở việc biết hôm nay có bao nhiêu review 1 sao. Pain nằm ở việc **"Tại sao khách cho 1 sao?"** (Giao chậm? Vỡ hộp? Thái độ shipper? Hàng lỗi?). Việc đọc thủ công hàng ngàn review mất quá nhiều thời gian, khiến Store Manager/QA không có **Actionable Insight** kịp thời để chấn chỉnh vận hành ngay trong ngày.

---

## Phase 5 & 6 — Workflow & AI Decision (Phần tiếp theo nhóm cần làm)

> *Dựa trên insight đắt giá phía trên, nhóm hãy tiếp tục thảo luận để:*
> 1. *Vẽ Workflow hiện tại (Khi Store Manager xuất file Excel review ra và đọc tay) và Workflow tương lai (Khi có AI hỗ trợ lọc/nhãn).*
> 2. *Viết Problem Statement v0 và v1.*
> 3. *Đánh giá xem bài toán này giải quyết bằng Rule, Workflow hay Agent là tốt nhất.*
