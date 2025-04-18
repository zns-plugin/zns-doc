---
id: phan-biet-thong-bao-zns-va-tin-uid
title: Phân biệt Thông báo ZNS và Tin UID
slug: /phan-biet-thong-bao-zns-va-tin-uid
---

# <p align="center">Phân biệt mẫu thông báo ZNS và tin UID</p>

## I. Định nghĩa cơ bản

**Thông báo Zalo Notification Service (ZNS) là thông báo Chăm sóc khách hàng** được gửi từ Zalo Official Account Doanh nghiệp đến khách hàng của Doanh nghiệp **bằng Số điện thoại có sử dụng Zalo**.

_Xem thêm_ [_Zalo Notification Service - Giải pháp Chăm sóc Khách hàng Tiết kiệm & Hiệu quả trên Zalo_](https://zalo.cloud/zns)

Mặt khác, **Tin nhắn UID là tin nhắn gửi từ Official Account Doanh nghiệp đến Khách hàng đã có tương tác với OA** của Doanh nghiệp có sử dụng Zalo thông qua định danh User ID (UID)

_Xem thêm_ [_Tổng quan về Tin nhắn UID_](https://developers.zalo.me/docs/official-account/tin-nhan/tong-quan)

- _UID trong Zalo Official Account là định danh của một người dùng xác định đối với một tài khoản OA xác định. Với mỗi cặp User-OA khác nhau sẽ tồn tại UID khác nhau_

- _Tương tác với OA được định nghĩa là một trong các hành động sau: Quan tâm OA, Gửi tin nhắn đến OA, Gọi đến OA hoặc chấp nhận cuộc gọi từ OA, Nhấn menu tương tác nhanh / menu Dịch vụ / CTA của OA Chatbot_

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/e43edff97adce6a8a03a680c9b347642.png" />
</p>

## II. Phân biệt theo chi tiết

Dịch vụ thông báo ZNS và Tin UID cung cấp dịch vụ đa dạng để Doanh nghiệp có thể sử dụng từng loại dịch vụ tùy theo nhu cầu và mục đích sử dụng:

<div class="table">
<table>
  <tbody>
    <tr>
      <td rowspan="2">&nbsp;</td>
      <td rowspan="2">
        <p style="text-align:center;">
          <strong>Thông báo ZNS</strong>
        </p>
      </td>
      <td colspan="3">
        <p style="text-align:center;">
          <strong>Tin UID</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p style="text-align:center;">
          <strong>Tin Tư vấn</strong>
        </p>
      </td>
      <td>
        <p style="text-align:center;">
          <strong>Tin Giao dịch</strong>
        </p>
      </td>
      <td>
        <p style="text-align:center;">
          <strong>Tin Truyền thông</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Mục đích</strong>
      </td>
      <td>
        <p>
          Thông báo đến KH <u>đã tồn tại giao dịch</u> với doanh nghiệp với
          nhiều mục đích:
        </p>
        <ul>
          <li>Giao dịch (mã xác thực, xác nhận giao dịch,…)</li>
          <li>
            Chăm sóc khách hàng (cập nhật chính sách, tài khoản, quyền lợi thành
            viên,…)
          </li>
          <li>Hậu mãi (chương trình khuyến mãi, giới thiệu sản phẩm mới)</li>
        </ul>
        <p>
          <a href="Thiết%20lập%20mục%20đích%20gửi%20khi%20tạo%20mẫu%20ZNS">
            Xem thêm: Cách xác định mục đích
          </a>
        </p>
      </td>
      <td>Tư vấn cho khách hàng về sản phẩm, dịch vụ</td>
      <td>
        Thông báo, cập nhật thông tin đến khách hàng về trạng thái của một giao
        dịch hoặc trao đổi về sản phẩm, dịch vụ, như xác nhận lịch hẹn, thông
        báo hóa đơn,...
      </td>
      <td>
        Cập nhật đến khách hàng những thông tin quảng cáo về sản phẩm, dịch vụ,
        hoặc thông tin chung về doanh nghiệp
      </td>
    </tr>
    <tr>
      <td>
        <strong>Đối tượng nhận</strong>
      </td>
      <td>Số điện thoại của Khách hàng của doanh nghiệp có sử dụng Zalo</td>
      <td colspan="2">Người dùng Zalo đã tương tác với OA (Theo UID)</td>
      <td>Người Quan tâm OA</td>
    </tr>
    <tr>
      <td>
        <strong>Điều kiện cần có</strong>
        <br />
        <strong>(Opt-in Condition)</strong>
      </td>
      <td>Không</td>
      <td>
        OA có được UID người dùng, và
        <br />
        Người dùng có phát sinh tương tác* hoặc cho phép tương tác, và
        <br />
        Tương tác* cuối của người dùng trong khoảng thời gian cho phép (07
        ngày).
      </td>
      <td>
        OA có được UID người dùng, và
        <br />
        Người dùng có phát sinh tương tác* hoặc cho phép tương tác.
      </td>
      <td>
        OA có được UID người dùng, và
        <br />
        Người dùng đang quan tâm OA.
      </td>
    </tr>
    <tr>
      <td>
        <strong>Công cụ gửi</strong>
      </td>
      <td>
        <ul>
          <li>
            <a
              target="_blank"
              rel="noopener noreferrer"
              href="https://developers.zalo.me/docs/zalo-notification-service/bat-dau/gioi-thieu-zalo-notification-service-api"
            >
              API
            </a>
            <br />
            <a
              target="_blank"
              rel="noopener noreferrer"
              href="https://developers.zalo.me/docs/zalo-notification-service/bat-dau/gioi-thieu-zalo-notification-service-api"
            >
              Xem thêm tại LINK
            </a>
          </li>
          <li>
            <a
              target="_blank"
              rel="noopener noreferrer"
              href="https://zalo.cloud/blog/huong-dan-su-dung-tinh-nang-gui-zns-theo-chien-dich-khong-can-thong-qua-api/pdujnyqpydqrepnq"
            >
              Gửi theo chiến dịch
            </a>
            <br />
            <a
              target="_blank"
              rel="noopener noreferrer"
              href="https://zalo.cloud/blog/huong-dan-su-dung-tinh-nang-gui-zns-theo-chien-dich-khong-can-thong-qua-api/pdujnyqpydqrepnq"
            >
              Xem thêm tại LINK
            </a>
          </li>
        </ul>
      </td>
      <td>
        <ul>
          <li>OA OpenAPI</li>
          <li>OA Manager</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>OA OpenAPI</li>
          <li>OA Manager (coming soon)</li>
        </ul>
      </td>
      <td>
        <ul>
          <li>OA OpenAPI</li>
          <li>OA Manager</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Hình thức (Format)</strong>
      </td>
      <td>
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://account.zalo.cloud/tool/zns/manage/template?sort=1&amp;status=4"
        >
          Theo template ZNS đã được xét duyệt
        </a>
      </td>
      <td>
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://stc-developers.zdn.vn/docs/v2/official-account/tin-nhan/tin-tu-van/gui-tin-tu-van-dang-van-ban"
        >
          Theo định dạng Tư vấn. Xem thêm.
        </a>
      </td>
      <td>
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://stc-developers.zdn.vn/docs/v2/official-account/tin-nhan/tin-giao-dich/gui-tin-giao-dich"
        >
          Theo định dạng Giao dịch. Xem thêm.
        </a>
      </td>
      <td>
        <a
          target="_blank"
          rel="noopener noreferrer"
          href="https://stc-developers.zdn.vn/docs/v2/official-account/tin-nhan/tin-truyen-thong/gui-tin-truyen-thong-ca-nhan"
        >
          Theo định dạng Truyền thông. Xem thêm.
        </a>
      </td>
    </tr>
    <tr>
      <td>
        <strong>Chi phí</strong>
        <br />
        <strong>(Chưa gồm VAT)</strong>
      </td>
      <td>
        <p>
          ZNS Xác thực: 300 VND / ZNS
          <br />
          ZNS Khác: 200 VND / ZNS
          <br />
          *Chưa gồm các tùy chọn bổ sung
        </p>
        <p>
          <a
            target="_blank"
            rel="noopener noreferrer"
            href="https://zalo.cloud/zns/pricing"
          >
            Xem thêm tại LINK
          </a>
        </p>
      </td>
      <td>50 VND/tin</td>
      <td>150 VND/tin</td>
      <td>Miễn phí</td>
    </tr>
  </tbody>
</table>
</div>

## III. Một số trường hợp ứng dụng ZNS

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/fe12844e8136aedbf9de497cb23b2280.png" />
</p>

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/6c5f0fa13650452167552f421536c387.png" />
</p>

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/4565c49f8bc9f5de67ba8bf4d3855105.png" />
</p>

## IV. Một số trường hợp sử dụng Tin UID

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/39eed5a495e2580694b1aa165203f8a8.png" />
</p>

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ Chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
