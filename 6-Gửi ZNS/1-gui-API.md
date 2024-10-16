---
id: gui-api
title: Hướng dẫn gửi API
---

# <p align ="center">Hướng dẫn gửi API</p>

## A. Giới thiệu về các phương thức gửi thông báo ZNS

Có 2 hình thức gửi thông báo ZNS:

1.      **Qua API**

2.      **Gửi theo chiến dịch** (Không qua API)

<div class="table" align="center">
    <table>
  <tbody>
    <tr>
      <td style="border:1.0pt solid black;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:225.75pt;">
        <p style="text-align:center;">
          <span style="color:#323130;">
            <strong>Qua API</strong>
          </span>
        </p>
      </td>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:none;border-right-style:solid;border-top-style:solid;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:231.1pt;">
        <p style="text-align:center;">
          <span style="color:#323130;">
            <strong>Theo chiến dịch&nbsp;</strong>(Không qua API)
          </span>
        </p>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:136.5pt;padding:0in 5.4pt;vertical-align:top;width:225.75pt;">
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi qua API
          </span>
        </p>
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Cần nhân lực có kiến
            thức về kỹ thuật&nbsp;
          </span>
        </p>
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi số lượng lớn&nbsp;
          </span>
        </p>
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Dữ liệu gửi API không
            được lưu trên ZCA
          </span>
        </p>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:136.5pt;padding:0in 5.4pt;vertical-align:top;width:231.1pt;">
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi qua file Excel tải
            lên ZCA
          </span>
        </p>
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Cần chuẩn bị file
            Excel&nbsp;
          </span>
        </p>
        <p style="margin-left:.5in;">
          <span style="color:#323130;">&nbsp;</span>
        </p>
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Gửi số lượng có hạn mức
          </span>
        </p>
        <p>
          <span style="color:#323130;">
            ·&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;Dữ liệu gửi được lưu
            trên tài khoản ZCA
          </span>
        </p>
      </td>
    </tr>
  </tbody>
</table>
</div>

## B. Hướng dẫn gửi API

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/046b14d8a00bee14b617f6dc541a2bd0.png" />
</p>

_<p align="center">Sequence diagram API giữa Đối tác gửi tin, Zalo server và người nhận ZNS</p>_

**Miêu tả chi tiết:**

### **(1) Gửi request API** theo hướng dẫn tại [**đây**](https://developers.zalo.me/docs/zalo-notification-service/gui-tin-zns/gui-zns) và [**lấy Access Token**](https://stc-developers.zdn.vn/docs/v2/official-account/bat-dau/xac-thuc-va-uy-quyen-cho-ung-dung-new) (Mã định danh để gửi ZNS) theo 1 trong 2 cách sau:

- Công cụ [API explorer](https://developers.zalo.me/docs/api/official-account-api/xac-thuc-va-uy-quyen/cach-2-xac-thuc-voi-cong-cu-api-explorer/phuong-thuc-lay-oa-access-token-su-dung-cong-cu-api-explorer-post-5004): _Dành cho Admin của OA/Ứng dụng lấy mã xác thực gửi tin._
- [Giao thức OAuth](https://developers.zalo.me/docs/api/official-account-api/xac-thuc-va-uy-quyen/cach-1-xac-thuc-voi-giao-thuc-oauth/yeu-cau-cap-moi-oa-access-token-post-4307): _Dành cho người có kiến thức về lập trình, hoặc khi Doanh nghiệp sử dụng Ứng dụng của bên thứ 3._

### **(2) Response** sau khi gửi API

Sau khi yêu cầu được gửi đi, máy chủ Zalo sẽ phản hồi với các thông tin sau:

<div class="table" align="center">
    <table>
  <tbody>
    <tr>
      <td style="border:1.0pt solid black;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:103.5pt;">
        <span style="color:#262626;">
          <strong>Tham số</strong>
        </span>
      </td>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:none;border-right-style:solid;border-top-style:solid;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:328.0pt;">
        <span style="color:#262626;">
          <strong>Mô tả</strong>
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:103.5pt;">
        <span style="color:#262626;">
          <i>error</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:328.0pt;">
        <span style="color:#262626;">0 nếu request thành công</span>
        <br />
        <span style="color:#262626;">
          ngược lại, xem Error Code chi tiết&nbsp;
        </span>
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://developers.zalo.me/docs/api/zalo-notification-service-api/phu-luc/bang-ma-loi-post-5233"
        >
          <span style="color:#262626;">tại đây</span>
        </a>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:103.5pt;">
        <span style="color:#262626;">
          <i>message</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:328.0pt;">
        <span style="color:#262626;">Mô tả của lỗi tương ứng</span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:103.5pt;">
        <span style="color:#262626;">
          <i>msg_id</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:328.0pt;">
        <span style="color:#262626;">ID của tin ZNS</span>
        <br />
        <span style="color:#262626;">
          <i>Lưu ý: chỉ trả về nếu yêu cầu thành công</i>
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:103.5pt;">
        <span style="color:#262626;">
          <i>sent_time</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:328.0pt;">
        <span style="color:#262626;">
          Thời gian máy chủ Zalo bắt đầu gửi ZNS (Định dạng timestamp)
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:103.5pt;">
        <span style="color:#262626;">
          <i>quota</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:328.0pt;">
        <span style="color:#262626;">Thông tin quota của OA</span>
        <br />
        <span style="color:#262626;">
          <i>Lưu ý: chỉ trả về nếu yêu cầu thành công</i>
        </span>
      </td>
    </tr>
  </tbody>
</table>
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

_Xem chi tiết hơn về cấu trúc của request và response tại [**ĐÂY**](https://developers.zalo.me/docs/api/zalo-notification-service-api/gui-zns/gui-zns-post-5208)_

### **(3) Sự kiện gửi ZNS** [](https://zalo.cloud/zns/guidelines/zns-api#3-s%E1%BB%B1-ki%E1%BB%87n-g%E1%BB%ADi-zns)

Nếu request thành công, tin ZNS sẽ được gửi tới người dùng:

·       **sent_time:** Thời điểm máy chủ Zalo bắt đầu gửi ZNS.

·       **delivery_time:** Thời gian người dùng nhận được ZNS trên thiết bị.

### **(4) Sự kiện người dùng nhận được tin ZNS** [](https://zalo.cloud/zns/guidelines/zns-api#4-s%E1%BB%B1-ki%E1%BB%87n-ng%C6%B0%E1%BB%9Di-d%C3%B9ng-nh%E1%BA%ADn-%C4%91%C6%B0%E1%BB%A3c-tin-zns)

Nếu ZNS được gửi thành công trên thiết bị của người dùng, thì một sự kiện sẽ được gửi tới URL webhook của Doanh nghiệp.

<div class="table" align="center">
    <table>
  <tbody>
    <tr>
      <td style="border:1.0pt solid black;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <strong>Tham số</strong>
        </span>
      </td>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:none;border-right-style:solid;border-top-style:solid;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">
          <strong>Mô tả</strong>
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>sender</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">
          ID của Official Account gửi thông báo
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>recipient</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">
          Số điện thoại người dùng nhận thông báo
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>event_name</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">Tên sự kiện: user_received_message</span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>delivery_time</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">
          Thời gian trên thiết bị người dùng nhận được ZNS
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>msg_id</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">ID của tin ZNS</span>
        <br />
        <span style="color:#262626;">
          <i>Lưu ý: chỉ trả về nếu yêu cầu thành công</i>
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>tracking_id</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">
          Mã số đánh dấu lần gọi API của đối tác, do đối tác định nghĩa ở{" "}
          <u>bước (1)</u>
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>app_id</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">
          ID của ứng dụng gửi tin (ứng dụng mà OA đã cấp quyền)
        </span>
      </td>
    </tr>
    <tr>
      <td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:72.8pt;">
        <span style="color:#262626;">
          <i>timestamp</i>
        </span>
      </td>
      <td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:377.95pt;">
        <span style="color:#262626;">Thời điểm gửi sự kiện</span>
      </td>
    </tr>
  </tbody>
</table>
</div>

Xem thêm chi tiết sự kiện tại [**ĐÂY**](https://developers.zalo.me/docs/api/zalo-notification-service-api/webhook/su-kien-nguoi-dung-nhan-thong-bao-zns-post-5235).

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
