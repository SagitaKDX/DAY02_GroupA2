# 03 — Individual Reflection (Phase 7)
**Học viên:** Cù Tiến Nam - 2A202600716

---

## 1. Tôi đã tham gia vào phần nào?

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng |
|---|---|---|
| Scan cá nhân | Đưa ra các insight để phản biện lại topic của nhóm. | Đóng góp góc nhìn đa chiều, giúp nhóm nhận ra điểm yếu của ý tưởng ban đầu. |
| Pitch Problem Card | Pitch bài toán y tế "Theo dõi tiến độ tập phục hồi chấn thương". | Giúp nhóm có không gian tranh luận về rủi ro đạo đức và ranh giới con người (Human Boundary) trong AI Y tế. |
| Chọn candidate problem | Đồng ý từ bỏ bài toán cá nhân của mình, vote cho bài "Phân tích đánh giá Shopee" của Minh. | Giúp nhóm nhanh chóng hội tụ (convergence) vào một bài toán có data rõ ràng (file CSV) và an toàn để thực hành lab. |
| Workflow | Đóng góp ý tưởng xây dựng. | Giúp hoàn thiện luồng quy trình tương lai (Future Workflow) thực tế hơn, chỉ rõ bước nào cần AI. |


## 2. Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Validation | Dùng AI (đóng vai Store Manager) để giả lập phỏng vấn và hỏi xem họ xử lý review 1 sao thế nào. | Cho ra các luồng vận hành cơ bản của một shop thương mại điện tử (các loại lỗi phổ biến). | AI trả lời chung chung, bảo là "có team đọc tay". Không chỉ ra được nỗi đau khi quá tải mùa Mega Sale. | Tự đúc kết insight thực tế: Mùa sale số lượng đơn x10, team đọc tay vỡ trận, cần AI phân tích aspect-based sentiment để cứu nguy. |
| Workflow & PS | Nhờ AI so sánh nhanh xem phân tích review bằng Rule (Regex) khác gì LLM. | Giải thích dễ hiểu: Rule bị lừa bởi câu mỉa mai (Sarcasm), còn LLM thì hiểu được. | AI gợi ý luôn việc "tự động nhắn tin đền bù khách hàng". | Gạt bỏ bước tự động nhắn tin đền bù (tránh rủi ro văng tục/hứa hão). Chỉ giữ AI ở mức sinh báo cáo. |

## 3. Reflection câu hỏi mở

**- Tôi học được gì khi nghe top 3 problems của các bạn khác?**
Tôi học được rằng một Problem "khủng" (như bài toán y tế của tôi) chưa chắc đã là một Problem tốt để làm sản phẩm ngay. Bài toán "Phân tích review Shopee" của Minh ghi điểm tuyệt đối vì nó cực kỳ khả thi: data rất dễ lấy (xuất file Excel là xong), metric đo lường bằng tiền/giờ rất rõ, và rủi ro khi AI sai là cực thấp so với ngành y tế.

**- Tôi có thay đổi ý kiến sau khi bị challenge không?**
Có. Lúc đầu tôi rất muốn bảo vệ bài toán "Phục hồi chấn thương" của mình. Nhưng khi nhóm challenge về việc "Làm sao lấy được data chuẩn để train/test?" và "Nếu AI đánh giá form tập sai dẫn đến hoại tử cơ thì ai chịu trách nhiệm?", tôi lập tức nhận ra *Fatal Error* quá lớn. Việc "Kill your darlings" (từ bỏ ý tưởng con cưng) để hướng tới mục tiêu chung của nhóm là một bài học đắt giá.

**- Nhóm có lúc nào bị solution-first không?**
Có một khoảng khắc ngắn khi bàn về bài Shopee, nhóm nảy ra ý định "Làm một con AI Agent tự động chui vào app Shopee để reply cãi nhau với khách/xin lỗi khách". Đây là tư duy solution-first và cực kỳ rủi ro cho danh tiếng nhãn hàng. Nhóm đã kịp lùi lại, quay về đúng mục tiêu giải quyết Bottleneck cho bộ phận QA: Chỉ đọc và phân tích, con người mới là người đưa ra hành động (Action).


---
*Hoàn thành Lab Day 02 - Phần Phản tư Cá nhân*
