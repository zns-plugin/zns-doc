---
id: co-che-tinh-gia-cua-mau-tin-zns
title: Cơ chế tính giá của mẫu tin ZNS
slug: /co-che-tinh-gia-cua-mau-tin-zns
---

# <p align="center">Cơ chế tính giá của mẫu tin ZNS</p>

Với mục đích cam kết chất lượng gửi tin, dịch vụ ZNS sẽ không tính phí nếu thời gian gửi tin vượt quá một mốc thời gian nhất định. Vui lòng tham khảo thêm trong bài viết dưới đây.

## 1. Bảng giá dịch vụ ZNS:

Thông tin chi tiết về bảng giá dịch vụ ZNS, Quý khách vui lòng tham khảo bảng giá ZNS tại [**ĐÂY**](https://zalo.cloud/zns/pricing).

## 2. Cơ chế tính giá dựa trên timeout API:

Với mục đích cam kết chất lượng gửi tin, dịch vụ ZNS sẽ chỉ được tính phí nếu thời gian gửi tin nằm trong khoảng thời gian timeout. Timeout của các loại tin ZNS như sau:

<div class="table" align="center">
    <table style=";"><tbody><tr><td style="background-color:#D1D1D1;border:1.0pt solid black;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:225.4pt;"><span style="color:#081C36;"><strong>Loại ZNS</strong></span></td><td style="background-color:#D1D1D1;border-bottom-style:solid;border-color:black;border-left-style:none;border-right-style:solid;border-top-style:solid;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:225.4pt;"><span style="color:#081C36;"><strong>Timeout (unit: giây/s)</strong></span></td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:225.4pt;"><span style="color:#081C36;">ZNS Xác thực</span></td><td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:225.4pt;"><span style="color:#081C36;">15</span></td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:225.4pt;"><span style="color:#081C36;">Các loại ZNS còn lại&nbsp;</span></td><td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:225.4pt;"><span style="color:#081C36;">7200</span></td></tr></tbody></table>
</div>

- _**Cách xác định thời gian gửi tin ZNS:**_

  - Khi gửi ZNS qua server Zalo thành công, nội dung response API sẽ bao gồm **sent_time.** (Xem hướng dẫn [gửi ZNS qua API](https://developers.zalo.me/docs/zalo-notification-service/gui-tin-zns/gui-zns))
  - Khi tin được gửi đến máy user, Zalo bắn event về webhook bao gồm **delivery_time**.   
    (Xem cách [truy xuất trạng thái ZNS qua API](https://developers.zalo.me/docs/zalo-notification-service/truy-xuat-thong-tin/lay-thong-tin-trang-thai-zns))
  - **Thời gian gửi tin ZNS** \= **delivery_time** – **sent time**
  - Nếu **Thời gian gửi tin ZNS >** **Timeout của loại ZNS**, tin ZNS sẽ không bị tính phí. Còn lại, nếu gửi thành công trong thời gian timeout quy định, tin ZNS sẽ được tính phí như thường lệ.

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ Chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
