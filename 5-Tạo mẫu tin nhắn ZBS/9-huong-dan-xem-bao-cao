---
id: huong-dan-tai-bao-cao-mapping-ket-qua-phan-hoi-template-rating-template-response_ykdwo79en4o1uyc81zp5aayj
title: Hướng dẫn tải báo cáo & mapping kết quả phản hồi - Template Rating & Template Response
---
_Áp dụng cho cả Template Rating (mẫu đánh giá dịch vụ) và Template Response (mẫu phản hồi nhanh)_

Sau khi gửi mẫu tin đánh giá dịch vụ (Rating) hay mẫu tin phản hồi nhanh (Response) cho khách hàng, chắc hẳn bạn sẽ muốn biết: có bao nhiêu người đã bấm vào, họ đánh giá/phản hồi thế nào, và cụ thể là ai (số điện thoại nào) đã tương tác. Quy trình để lấy những thông tin này ở cả 2 loại mẫu tin về cơ bản là giống nhau, vì vậy bài viết này sẽ trình bày chung để bạn có thể áp dụng cho cả hai.

1\. Xem báo cáo kết quả người dùng đã phản hồi
----------------------------------------------

Bạn có thể tải file báo cáo cho cả mẫu Rating và Response chỉ với vài bước trên trang Quản lý Template của ZBS Account:

*   **Bước 1:** Ở menu bên trái, chọn Quản lý Template.
    
*   **Bước 2:** Dùng bộ lọc **Lọc theo loại mẫu ZBS** ở cột bên phải — chọn **Mẫu đánh giá dịch vụ** nếu bạn muốn xem báo cáo Rating, hoặc **Mẫu phản hồi nhanh** nếu muốn xem báo cáo Response. Bạn có thể kết hợp thêm Lọc theo trạng thái = Đã duyệt để thu hẹp kết quả.
*   **Bước 3:** Tại dòng template cần xem, bấm vào biểu tượng \[...\] cạnh nút Xem chi tiết, rồi chọn Tải báo cáo.

![image.png](https://content.zalo.cloud/uploads/image_80983df741.png)

2. Nội dung file báo cáo và ý nghĩa từng cột
--------------------------------------------

File tải về sẽ có tên ReportRateTemplate (cho Rating) hoặc ReportResponseTemplate (cho Response). Vì cơ chế giống nhau nên phần lớn các cột cũng trùng tên hoặc trùng ý nghĩa — bảng dưới đây liệt kê đầy đủ để bạn dễ tra cứu, trong đó các cột dùng chung và các cột chỉ có ở một loại mẫu tin đều được ghi chú rõ:

| **Cột (Rating)** | **Cột (Response)** | **Ý nghĩa** | **Dùng cho** |
| --- | --- | --- | --- |
| STT | STT | Số thứ tự dòng trong file | Cả hai |
| SubmitDate | submit\_time | Thời điểm người dùng gửi đánh giá / gửi phản hồi | Cả hai |
| MsgID (messageId) | message\_id | Mã tin nhắn — chìa khoá để nối với số điện thoại (xem mục 3) | Cả hai |
| TrackingID | tracking\_id | Mã tracking do doanh nghiệp tự truyền vào lúc gửi tin (nếu có) | Cả hai |
| Rating | — | Mức đánh giá người dùng chọn (số sao) | Chỉ Rating |
| Detailed\_feedback | — | Nội dung phản hồi chi tiết mà người dùng gõ vào | Chỉ Rating |
| Các cột tiêu chí (VD: đóng gói hàng tốt hơn, chất lượng sản phẩm tốt hơn, …) | — | Là các tiêu chí đánh giá đã được cấu hình sẵn trong template — tên cột chính là tên tiêu chí, giá trị cho biết tiêu chí đó có được người dùng chọn hay không. Số cột nhiều hay ít tuỳ vào cấu hình từng template và từng mức sao. | Chỉ Rating |
| — | Response(Data) | Nội dung người dùng phản hồi (nút họ bấm hoặc tin nhắn họ gửi) | Chỉ Response |

_Lưu ý: file báo cáo chỉ ghi nhận những tin nhắn đã có phản hồi. Những tin đã gửi nhưng chưa có người tương tác sẽ không xuất hiện trong file._

3. Cách nối dữ liệu để xác định số điện thoại đã tương tác
----------------------------------------------------------

File báo cáo ở trên cho bạn biết nội dung phản hồi, nhưng lại không có sẵn số điện thoại. Nếu bạn cần biết cụ thể ai đã đánh giá/phản hồi - ví dụ để chăm sóc lại khách hàng hay xử lý yêu cầu họ gửi — thì chỉ cần thêm một bước nối dữ liệu đơn giản dựa trên mã tin nhắn.

**Bước 1 — Tải file CampaignDetail:** Vào Công cụ gửi tin theo SĐT → Gửi theo chiến dịch → chọn đúng chiến dịch đã gửi mẫu tin (Rating hoặc Response) → Tải báo cáo chi tiết. File tải về có tên `CampaignDetail_<CampaignId>.xlsx`, bạn chỉ cần quan tâm 2 cột: Phone và MsgId. Nếu mẫu tin được gửi qua nhiều chiến dịch, bạn tải toàn bộ rồi gộp lại thành một bảng tra cứu chung.

![image.png](https://content.zalo.cloud/uploads/image_0d9273a1a9.png)

**Bước 2 — Nối dữ liệu bằng messageId:** Lấy cột MsgID (với Rating) hoặc message\_id (với Response) trong file báo cáo, đối chiếu với cột MsgId trong file CampaignDetail. Hai giá trị trùng nhau nghĩa là cùng một tin nhắn, từ đó bạn xác định được chính xác số điện thoại tương ứng với dòng phản hồi/đánh giá đó.
