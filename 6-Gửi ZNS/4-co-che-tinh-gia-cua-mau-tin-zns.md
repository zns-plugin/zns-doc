---
id: co-che-tinh-gia-cua-mau-tin-zns
title: Cơ chế tính giá của mẫu tin ZNS
slug: /co-che-tinh-gia-cua-mau-tin-zns
---

# <p align="center">Cơ chế tính giá của mẫu tin ZNS</p>


Với mục đích cam kết chất lượng gửi tin, dịch vụ ZNS sẽ không tính phí nếu thời gian gửi tin vượt quá một mốc thời gian nhất định. Vui lòng tham khảo thêm trong bài viết dưới đây.   
 

## 1. Bảng giá dịch vụ ZNS:


Thông tin chi tiết về bảng giá dịch vụ ZNS, Quý khách vui lòng tham khảo bảng giá ZNS tại [**ĐÂY**](https://zalo.cloud/zns/pricing ).


## 2. Cơ chế tính giá dựa trên timeout API:


Với mục đích cam kết chất lượng gửi tin, dịch vụ ZNS sẽ chỉ được tính phí nếu thời gian gửi tin nằm trong khoảng thời gian timeout. Timeout của các loại tin ZNS như sau:

<div class="table" align="center">
    <table>
<table class="ck-table-resized"><colgroup><col style="width:41.06%;"><col style="width:58.94%;"></colgroup><tbody><tr><td style="background-color:hsl(0, 0%, 60%);text-align:center;"><strong>Loại ZNS</strong></td><td style="background-color:hsl(0, 0%, 60%);text-align:center;"><strong>Timeout (unit: giây/s)</strong></td></tr><tr><td style="text-align:center;">ZNS Xác thực</td><td style="text-align:center;">15</td></tr><tr><td style="text-align:center;">Các ZNS còn lại</td><td style="text-align:center;">7200</td></tr></tbody></table>
</div>

*   _**Cách xác định thời gian gửi tin ZNS:**_

1.  Khi gửi ZNS qua server Zalo thành công, nội dung response API sẽ bao gồm **sent\_time.** (Xem hướng dẫn [gửi ZNS qua API](https://developers.zalo.me/docs/zalo-notification-service/gui-tin-zns/gui-zns))
2.  Khi tin được gửi đến máy user, Zalo bắn event về webhook bao gồm **delivery\_time**.   
    (Xem cách [truy xuất trạng thái ZNS qua API](https://developers.zalo.me/docs/zalo-notification-service/truy-xuat-thong-tin/lay-thong-tin-trang-thai-zns))

_**<p align="center">Thời gian gửi tin ZNS \= delivery\_time – sent_time</p>**_   
 

Nếu **Thời gian gửi tin ZNS >** **Timeout của loại ZNS**, tin ZNS sẽ không bị tính phí. Còn lại, nếu gửi thành công trong thời gian timeout quy định, tin ZNS sẽ được tính phí như thường lệ.


_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ Chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
