# 03 — Individual Reflection Example

## Đóng góp của Minh Phúc trong nhóm

| Hoạt động | Minh Phúc đã làm gì? | Kết quả |
|---|---|---|
| Scan cá nhân | Đưa ra 3 problems | Nhóm có nhiều candidate về reporting/workflow |
| Pitch | Pitch Xử lý Bookmark | Không được chọn nhưng có nhiều góc nhìn hơn về vấn đề này |
| Challenge | Debate các vấn đề của các thành viên khác đưa ra để tìm ra vấn đề phù hợp nhất | Nhóm loại bớt scope quá rộng |
| Workflow | Đóng góp ý tưởng giúp hoàn thiện workflow cho vấn đề được chọn | Nhóm hoàn thiện workflow bản cuối |


## Bảng dùng AI trong reflection

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| Scan | Gợi ý thêm problems trong cuộc sống thường nhật | Giúp chỉ ra nhiều vấn đề mà bản thân chưa nghĩ tới | Vài gợi ý quá chung chung, hay quá vĩ mô ở tầm doanh nghiệp | Bỏ các ý bản thân thấy chưa thật sự nhìn được workflow rõ ràng |
| Workflow | Nhờ AI phác thảo luồng công việc (before/after) cho bài toán gợi ý thực đơn. | Chia bước rất nhanh và mạch lạc | AI có xu hướng tự cho AI quyền quyết định thay người dùng. | Chỉnh lại ranh giới (Human Boundary). Ép AI chỉ dừng ở bước sinh ra gợi ý, quyền chốt món phải thuộc về con người. |
| Research | Nhờ AI tìm các tool/ứng dụng đã có trên thị trường giải quyết bài toán nhập liệu chi tiêu bằng tin nhắn tự do hoặc tự động đọc SMS. | Liệt kê rất nhanh các pattern phổ biến (như dùng Telegram Bot kết nối LLM API) và nhắc đến tính năng scan hóa đơn của một số app như Spendee, MoneyLover. | Đề xuất các giải pháp đòi hỏi tích hợp thẳng API ngân hàng. | Gạt bỏ ngay các hướng đi đòi hỏi API ngân hàng nội địa. |


## Bài học của Minh Phúc

- Problem tốt bắt nguồn từ workflow thực tế, không phải từ quy mô: Ban đầu AI thường vẽ ra các vấn đề vĩ mô hoặc quá chung chung. Tuy nhiên, một bài toán chỉ thực sự giải quyết được bằng AI khi ta nhìn thấy rõ từng bước trong workflow hiện tại.
- Luôn phải thiết lập Human Boundary: Trách nhiệm của người thiết kế là phải giữ quyền chốt hạ quan trọng thuộc về con người.
- Cẩn trọng với ảo giác kiến trúc của AI khi research: LLM có thể đề xuất các giải pháp công nghệ nghe rất logic và phổ biến trên thế giới, nhưng lại hoàn toàn phi thực tế và vi phạm rào cản bảo mật.

Nếu làm lại:

```text
Tôi sẽ thiết lập các rào cản kỹ thuật (như bảo mật dữ liệu, giới hạn API nội địa) ngay từ bước Individual Scan, thay vì đợi đến lúc Research mới bắt đầu gạt bỏ các ý tưởng viển vông. Việc xác định rõ giới hạn công nghệ ngay từ đầu sẽ giúp nhóm không bị cuốn vào những bài toán nghe rất hay ho nhưng lại bất khả thi khi triển khai thực tế.
```

---