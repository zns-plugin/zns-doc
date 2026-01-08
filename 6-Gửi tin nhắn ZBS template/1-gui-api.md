---
id: gui-api
title: Hướng dẫn gửi API
slug: /gui-api
---

# <p align ="center">Hướng dẫn gửi API</p>


## 1. Giới thiệu về các phương thức gửi Tin nhắn ZBS Template


Có 2 hình thức gửi tin: 

1.      **Qua API** 

2.      **Gửi theo chiến dịch** (Không qua API)

<div class="table" align="center">
    <table>
<table><tbody><tr><td style="text-align:center;"><strong>Qua API</strong></td><td style="text-align:center;"><strong>Theo chiến dịch (Không qua API)</strong></td></tr><tr><td><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi qua API</p><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Cần nhân lực có kiến thức về kỹ thuật&nbsp;</p><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi số lượng lớn&nbsp;</p><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Dữ liệu gửi API không được lưu trên ZCA</p></td><td><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi qua file Excel tải lên ZBS</p><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Cần chuẩn bị file Excel&nbsp;</p><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi số lượng có hạn mức</p><p>·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Dữ liệu gửi được lưu trên tài khoản ZBS</p></td></tr></tbody></table>
</div>


## 2. Hướng dẫn gửi API

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/046b14d8a00bee14b617f6dc541a2bd0.png" />
</p>


_<p align="center">Sequence diagram API giữa Đối tác gửi tin, Zalo server và người nhận tin</p>_


**Miêu tả chi tiết:**

### a. Gửi request API

Gửi request API theo hướng dẫn tại [**ĐÂY**](https://developers.zalo.me/docs/zalo-notification-service/gui-tin-zns/gui-zns) và [**lấy Access Token**](https://stc-developers.zdn.vn/docs/v2/official-account/bat-dau/xac-thuc-va-uy-quyen-cho-ung-dung-new) (Mã định danh để gửi tin) theo 1 trong 2 cách sau:


*   Công cụ [API explorer](https://developers.zalo.me/docs/api/official-account-api/xac-thuc-va-uy-quyen/cach-2-xac-thuc-voi-cong-cu-api-explorer/phuong-thuc-lay-oa-access-token-su-dung-cong-cu-api-explorer-post-5004): _Dành cho Admin của OA/Ứng dụng lấy mã xác thực gửi tin._
*   [Giao thức OAuth](https://developers.zalo.me/docs/api/official-account-api/xac-thuc-va-uy-quyen/cach-1-xac-thuc-voi-giao-thuc-oauth/yeu-cau-cap-moi-oa-access-token-post-4307): _Dành cho người có kiến thức về lập trình, hoặc khi Doanh nghiệp sử dụng Ứng dụng của bên thứ 3._


### b. Response sau khi gửi API


Sau khi yêu cầu được gửi đi, máy chủ Zalo sẽ phản hồi với các thông tin sau:

<div class="table" align="center">
    <table>
<table><tbody><tr><td style="text-align:center;"><strong>Tham số</strong></td><td style="text-align:center;"><strong>Mô tả</strong></td></tr><tr><td style="text-align:center;">error</td><td style="text-align:justify;">0 nếu request thành công<br>Ngược lại, xem Error Code chi tiết&nbsp;<a target="_blank" rel="noopener noreferrer" href="https://developers.zalo.me/docs/api/zalo-notification-service-api/phu-luc/bang-ma-loi-post-5233">tại đây</a></td></tr><tr><td style="text-align:center;"><i>message</i></td><td style="text-align:justify;">Mô tả của lỗi tương ứng</td></tr><tr><td style="text-align:center;"><i>msg_id</i></td><td style="text-align:justify;">ID của tin<br><i>Lưu ý: chỉ trả về nếu yêu cầu thành công</i></td></tr><tr><td style="text-align:center;"><i>sent_time</i></td><td style="text-align:justify;">Thời gian máy chủ Zalo bắt đầu gửi tin (Định dạng timestamp)</td></tr><tr><td style="text-align:center;"><i>quota</i></td><td style="text-align:justify;">Thông tin quota của OA<br><i>Lưu ý: chỉ trả về nếu yêu cầu thành công</i></td></tr></tbody></table>
</div>

**Example response**

```json
{
    "error": 0,
    "message": "Success",
    "data": {
        "msg_id": "a4d0243feee163bd3af2"
            "sent_time": "1626926349402",
            "quota": {
                "dailyQuota": "500",
                "remainingQuota": "499"
            }
    }
}
```

Xem chi tiết hơn về cấu trúc của request và response tại [**ĐÂY**](https://developers.zalo.me/docs/api/zalo-notification-service-api/gui-zns/gui-zns-post-5208).


### c. Sự kiện gửi tin [](https://zalo.solutions/zns/guidelines/zns-api#3-s%E1%BB%B1-ki%E1%BB%87n-g%E1%BB%ADi-zns)

Nếu request thành công, tin sẽ được gửi tới người dùng:

·       **sent\_time:** Thời điểm máy chủ Zalo bắt đầu gửi tin.

·       **delivery\_time:** Thời gian người dùng nhận được tin trên thiết bị.


### d. Sự kiện người dùng nhận được tin [](https://zalo.solutions/zns/guidelines/zns-api#4-s%E1%BB%B1-ki%E1%BB%87n-ng%C6%B0%E1%BB%9Di-d%C3%B9ng-nh%E1%BA%ADn-%C4%91%C6%B0%E1%BB%A3c-tin-zns)


Nếu tin được gửi thành công trên thiết bị của người dùng, thì một sự kiện sẽ được gửi tới URL webhook của Doanh nghiệp.

<div class="table" align="center">
    <table>
<table><tbody><tr><td style="text-align:center;"><strong>Tham số</strong></td><td style="text-align:center;"><strong>Mô tả</strong></td></tr><tr><td style="text-align:center;"><i>sender</i></td><td style="text-align:justify;">ID của Official Account gửi thông báo</td></tr><tr><td style="text-align:center;"><i>recipient</i></td><td style="text-align:justify;">Số điện thoại người dùng nhận thông báo</td></tr><tr><td style="text-align:center;"><i>event_name</i></td><td style="text-align:justify;">Tên sự kiện: user_received_message</td></tr><tr><td style="text-align:center;"><i>delivery_time</i></td><td style="text-align:justify;">Thời gian trên thiết bị người dùng nhận được ZNS</td></tr><tr><td style="text-align:center;"><i>msg_id</i></td><td style="text-align:justify;">ID của tin ZNS<br><i>Lưu ý: chỉ trả về nếu yêu cầu thành công</i></td></tr><tr><td style="text-align:center;"><i>tracking_id</i></td><td style="text-align:justify;">Mã số đánh dấu lần gọi API của đối tác, do đối tác định nghĩa ở <u>bước (1)</u></td></tr><tr><td style="text-align:center;"><i>app_id</i></td><td style="text-align:justify;">ID của ứng dụng gửi tin (ứng dụng mà OA đã cấp quyền)</td></tr><tr><td style="text-align:center;"><i>timestamp</i></td><td style="text-align:justify;">Thời điểm gửi sự kiện</td></tr></tbody></table>
</div>

_<p align="center">Xem thêm chi tiết sự kiện tại [**ĐÂY**](https://developers.zalo.me/docs/api/zalo-notification-service-api/webhook/su-kien-nguoi-dung-nhan-thong-bao-zns-post-5235).</p>_

_Nếu có bất kì yêu cầu hỗ trợ, Quý khách có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của chúng tôi qua **Biểu Mẫu: [Mẫu hỗ trợ Zalo Business Solutions](https://go.zalo.me/SupportZBS )**. Chúng tôi sẽ phản hồi Quý khách trong vòng 24h làm việc tiếp theo._

