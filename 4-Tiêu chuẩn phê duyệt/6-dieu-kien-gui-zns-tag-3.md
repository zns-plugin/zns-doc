---
id: dieu-kien-de-gui-thong-bao-zns-hau-mai-tag-3
title: Điều kiện để gửi thông báo ZNS Hậu mãi (Tag 3)
slug: /dieu-kien-de-gui-thong-bao-zns-hau-mai-tag-3
---

# <p align="center">Điều kiện để gửi thông báo ZNS Hậu mãi (Tag 3)</p>

Mẫu thông báo ZNS cấp độ Hậu mãi (_hay còn gọi **ZNS Tag 3 Hậu mãi** hay mẫu ZNS **Promotion** - đối với quý khách sử dụng API)_ dùng để **gửi thông báo hậu mãi đến khách hàng đã từng phát sinh giao dịch với Zalo Official Account (OA)**.

**Lưu ý:**

- Ngoài thiết lập đúng mục đích, cách dùng từ trong nội dung mẫu thông báo cần đảm bảo tính chuyên nghiệp, đồng bộ, cụ thể để diễn giải đúng và chính xác bối cảnh và mục đích của mẫu thông báo.
  - Zalo Cloud có quyền từ chối các mẫu thông báo có nội dung chưa phù hợp, thiếu thông tin thể hiện bối cảnh và mục đích mẫu tin.
  - Tham khảo [**Quy định chung khi kiểm duyệt mẫu ZNS**](https://zalo.cloud/news/quy-dinh-chung-khi-kiem-duyet-mau-tin-zns/baujzpyvjjrz7776m) để biết thêm chi tiết về quy định kiểm duyệt.
- Trong mẫu thông báo tag Hậu mãi, tùy chọn CTA dẫn về Hotline/ Số điện thoại (SĐT) doanh nghiệp: doanh nghiệp cần sử dụng SĐT có định dạng tổng đài với đầu số 1800 hoặc 1900 để đảm bảo tính chuyên nghiệp và trải nghiệm của người dùng.
  - Trường hợp doanh nghiệp sử dụng số bàn/ số điện thoại cá nhân hoặc đầu số khác: cần cũng cấp thông tin chứng minh là SĐT này là số hotline của doanh nghiệp.   
    (VD: SĐT này được đăng tải công khai là số hotline trên website hoặc trên các kênh chính thống của doanh nghiệp và đính kèm link tại mục **Ghi chú cho kiểm duyệt** khi tạo temp).

Xem thêm hướng dẫn [Thiết lập mục đích gửi khi tạo mẫu ZNS](https://zalo.cloud/blog/thiet-lap-muc-dich-gui-khi-tao-mau-zns/erug88djjgrd9r7zzj)

## 1. Để gửi mẫu thông báo ZNS cấp độ Hậu mãi, Quý khách sẽ thông qua quy trình như sau: 

### Bước 1: Kiểm tra tình trạng quyền gửi ZNS hiện tại của OA

Quý doanh nghiệp cần đảm bảo yêu cầu sau:

<div class="table">
<table><tbody><tr><td><p style="margin-left:0px;text-align:center;"><span style="background-color:hsl(180,75%,60%);"><strong><p align="center">Sau 0H ngày 12/03/2024</p></strong>&nbsp;</span></p></td></tr><tr><td><span style="color:rgb(18,19,23);">Zalo OA đang được cấp phép gửi ở Cấp độ 3 (Tra cứu tại trang </span><a target="_blank" rel="noopener noreferrer" href="https://account.zalo.cloud/RZUPB7MA6RKY9VGZ/tool/zns/report/quality"><span style="color:hsl(210,75%,60%);"><u>Chất lượng gửi ZNS</u></span><span style="color:rgb(18,19,23);"> trên ZCA</span></a><span style="color:rgb(18,19,23);"> hoặc sử dụng </span><a target="_blank" rel="noopener noreferrer" href="https://developers.zalo.me/docs/zalo-notification-service/truy-xuat-thong-tin/lay-thong-tin-loai-noi-dung-zns-duoc-phep-gui"><span style="color:hsl(210,75%,60%);"><u>API để lấy thông tin loại nội dung ZNS được phép gửi</u></span></a><span style="color:rgb(18,19,23);">)&nbsp;</span></td></tr></tbody></table>
</div>

_<p align="center">Xem thêm [Cơ chế đánh giá chất lượng và quyền lợi gửi ZNS](https://zalo.cloud/blog/co-che-danh-gia-chat-luong-va-quyen-loi-gui-zns/rzu6k97e8vkbnmereg).</p>_

### Bước 2: Đánh giá lại toàn diện 

Sau khi thỏa mãn 2 yêu cầu trên, **Quý khách vui lòng gửi email** đến bộ phận phụ trách khách hàng của Zalo Cloud tại địa chỉ [support@zalo.cloud](mailto:support@zalo.cloud) để chúng tôi tiến hành sang bước đánh giá lại toàn diện. Nội dung Email bao gồm 2 phần:

- Tiêu đề email Quý khách vui lòng ghi rõ: **Hỗ trợ gửi thông báo cấp độ 3 OA** \[điền OA ID\]
- Kèm theo nội dung trong email thể hiện:
  - Thông tin liên quan đến lĩnh vực doanh nghiệp đang hoạt động;
  - Thông tin tài khoản ZCA (Mã tài khoản ZCA);
  - Nội dung thông báo ZNS Tag 3 dự định triển khai;
  - Thông tin liên hệ của nhân sự chịu trách nhiệm làm việc với đội ngũ phát triển khách hàng của Zalo Cloud.

Sau khi nhận yêu cầu từ quý khách, đội ngũ phụ trách phát triển khách hàng và đối tác kinh doanh ZNS sẽ tiến hành xem xét lại toàn diện quá trình gửi ZNS của doanh nghiệp, đánh giá tiềm năng gửi trong tương lai và đưa ra quyết định OA đó có được gửi ZNS cấp độ 3 hay không. Chúng tôi sẽ phản hồi Quý khách trong vòng 2 – 3 ngày làm việc kế tiếp.

Đối với quý khách không sử dụng API, nếu Quý khách chưa biết được OA của doanh nghiệp đang được cấp phép gửi ở cấp độ nào, đội ngũ chăm sóc khách hàng của Zalo Cloud có thể hỗ trợ tra cứu giúp Quý khách.

Để yêu cầu hỗ trợ tra cứu, quý khách vui lòng gửi mail về địa chỉ [support@zalo.cloud](mailto:support@zalo.cloud) với tiêu đề là: **ZNS-Hỗ trợ kiểm tra cấp độ được phép gửi của OA\[điền OA ID\]**. Đội ngũ hỗ trợ khách hàng sẽ phản hồi lại yêu cầu trong vòng 1 –2 ngày làm việc kế tiếp.

## 2. Các cơ chế gửi và nhận ZNS template tag Hậu mãi:

Xem thêm **tại phần A.2** - [Cơ chế đánh giá chất lượng và quyền lợi gửi ZNS](https://zalo.cloud/blog/co-che-danh-gia-chat-luong-va-quyen-loi-gui-zns/rzu6k97e8vkbnmereg)

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của Zalo Cloud qua email: support@zalo.cloud. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
