## Reflection Cá Nhân: Vượt Ra Khỏi Dòng Code Để Nhìn Vào Bài Toán Thực Tế

**1. Góc nhìn mới về AI: Công cụ mạnh không bằng định hướng đúng**
Trước đây, khi làm việc với các dự án AI, sự tập trung thường dồn vào kiến trúc hệ thống—làm sao để xây dựng pipeline tối ưu, tinh chỉnh hệ thống RAG, hay làm mượt các luồng truy xuất dữ liệu. Nhưng trải qua lab này, góc nhìn của tôi đã thay đổi hoàn toàn. 

AI hiện tại có thể "nhúng" vào mọi nơi, từ y tế, giáo dục đến thương mại điện tử. Tuy nhiên, việc đề xuất một giải pháp (Propose Solution) bằng AI giờ đây là phần dễ nhất. Phần khó nhất và mang lại giá trị cao nhất chính là **Define Business Case**. Nhận ra được AI sinh ra để phục vụ ai, giải quyết "nỗi đau" gì, và mang lại bao nhiêu lợi ích thực tế mới là thứ phân biệt một sản phẩm AI có tính ứng dụng với một bản demo kỹ thuật vô thưởng vô phạt.

**2. Vai trò trong nhóm: Mỏ neo thực tế và kiểm soát rủi ro**
Trong quá trình làm việc nhóm, rất dễ để các thành viên bị cuốn theo sự hào nhoáng của công nghệ (như việc muốn build các Agent tự động hoàn toàn từ A-Z). Vai trò của tôi là kéo những ý tưởng đó về lại mặt đất. 

Khi bảo vệ và phát triển bài toán **Sentiment Analysis cho đánh giá đơn hàng**, tôi tập trung vào việc bóc tách Workflow: Input là gì (file Excel từ sàn), Output là gì (báo cáo nguyên nhân), và ranh giới nằm ở đâu. Thay vì để AI tự động rep comment khách hàng với rủi ro khủng hoảng truyền thông cực cao, tôi định hình lại luồng đi: AI đóng vai trò xử lý lô lớn (Batch processing), nhưng con người (QA/Store Manager) mới là chốt chặn cuối cùng ra quyết định. Việc nhìn ra rủi ro và biết "điểm dừng" của công nghệ là đóng góp cốt lõi của tôi để dự án có tính khả thi cao nhất.

**3. Bài học cốt lõi sau Lab: Problem-First Thinking**
* **Xác định vấn đề quan trọng hơn giải pháp:** Nếu không đo lường được thời gian lãng phí hiện tại (Bottleneck) hay xác định đúng Actor, mọi nỗ lực code hay viết prompt đều vô nghĩa. 
* **Hiểu những gì mình đang làm:** Nhảy sang dùng Agent quá sớm khi bài toán chỉ cần một LLM Workflow một chiều là một cái bẫy lớn. Việc hiểu rõ ranh giới giữa Rule-based, LLM Pipeline và Agent giúp tối ưu hóa chi phí vận hành và giảm thiểu rủi ro sinh ảo (Hallucination).
* **Quản lý và ứng dụng là then chốt:** Công nghệ có thể lỗi thời sau vài tháng, nhưng tư duy quản lý một hệ thống AI thì không. Việc biết cách tích hợp một công cụ AI vào quy trình làm việc hiện có của người dùng một cách mượt mà, không gây xáo trộn, và có chỉ số đánh giá (Metric) rõ ràng mới là yếu tố quyết định sự sống còn của một sản phẩm thực tế.
