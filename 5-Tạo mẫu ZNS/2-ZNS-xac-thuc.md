---
id: cach-su-dung-va-ung-dung-cua-mau-tin-zns-xac-thuc
title: Cách sử dụng và ứng dụng của mẫu tin ZNS Xác thực
slug: /cach-su-dung-va-ung-dung-cua-mau-tin-zns-xac-thuc
---

# <p align="center">Cách sử dụng và ứng dụng của mẫu tin ZNS Xác thực</p>

Với tinh thần luôn luôn lắng nghe và thấu hiểu nhu cầu của khách hàng muốn trải nghiệm mua sắm thuận tiện và dễ dàng, đội ngũ nghiên cứu và phát triển sản phẩm Zalo Notification Service (ZNS) chính thức ra mắt mẫu ZNS Xác thực như một công cụ tối ưu hỗ trợ người dùng bảo vệ tài khoản và nâng cao trải nghiệm của mình.

## 1. ZNS Xác thực là gì? Cách ứng dụng ZNS Xác thực:

ZNS Xác thực là mã xác thực một lần được gửi đến người dùng Zalo thông qua dịch vụ Zalo Notification Service (ZNS). Với mục đích xác nhận đăng nhập các ứng dụng online, thông báo về quá trình tạo hoặc thay đổi trạng thái người dùng (gửi mã xác thực cho khách hàng tạo tài khoản mới, xác nhận đổi mật khẩu, xác thực tài khoản, xác thực giao dịch,…)

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/bc9ff84938b6177ec056ad11aabbd7f2.png" />
</p>

## 2. Cấu trúc của một mẫu tin ZNS Xác thực:

Doanh nghiệp sử dụng mẫu ZNS Xác thực mặc định trên tài khoản Zalo Cloud Account và cấu trúc mặc định của 1 mẫu tin ZNS Xác thực bao gồm:

- Logo OA
- Thông tin **“Mã xác thực của bạn là &lt;otp&gt;”**

Doanh nghiệp có thể sao chép mã xác thực từ thông báo ZNS. Thông tin chi tiết về tính năng sao chép mã xác thực, xem tại [**ĐÂY**](https://zalo.cloud/blog/cap-nhat-kha-nang-sao-chep-doi-voi-mau-zns-xac-thuc/erub6bg47kawnvqnk)

Bên cạnh những nội dung mặc định, doanh nghiệp cũng có thể chỉnh sửa nội dung ZNS gửi kèm mã xác thực.

<div class="table" align="center">
    <table>
  <tbody>
    <tr>
      <td>
        <p style="margin-left:0px;">&nbsp;</p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <strong>Phần cố định của hệ thống</strong>
          <span style="color:rgb(0,120,212);">&nbsp;</span>
        </p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <strong>Phần có thể chỉnh sửa theo nhu cầu sử dụng</strong>
          <span style="color:rgb(0,120,212);">&nbsp;</span>
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <strong>Logo đăng ký</strong>
          <span style="color:rgb(0,120,212);">&nbsp;</span>
        </p>
        <p style="margin-left:0px;">
          <img
            class="image_resized"
            style="width:243px;"
            src="https://stc-oa.zdn.vn/uploads/c12c01a6a2ae55ce0fc01486e4648c0c.png"
          />
          &nbsp;
        </p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <img
            class="image_resized"
            style="width:44px;"
            src="https://stc-oa.zdn.vn/uploads/48dca6d085589412dc674bdacab21356.png"
          />
          &nbsp;
        </p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <img
            class="image_resized"
            style="width:46px;"
            src="https://stc-oa.zdn.vn/uploads/aff4f9e3fc3b3dc2b53bd35fe0fdcf9b.png"
          />
          &nbsp;
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <strong>Nội dung:</strong>
          <span style="color:rgb(0,120,212);">&nbsp;</span>
        </p>
        <p style="margin-left:0px;">Mã xác thực của bạn là&nbsp;</p>
        <p style="margin-left:0px;">&lt;otp&gt;&nbsp;</p>
        <p style="margin-left:0px;">
          <img
            class="image_resized"
            style="width:243px;"
            src="https://stc-oa.zdn.vn/uploads/7bbd4cb6d07beb06026b99abedd2961e.png"
          />
          &nbsp;
        </p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <img
            class="image_resized"
            style="width:46px;"
            src="https://stc-oa.zdn.vn/uploads/9e596c24460ba39c0d93c59f7449b8ed.png"
          />
          &nbsp;
        </p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <img
            class="image_resized"
            style="width:44px;"
            src="https://stc-oa.zdn.vn/uploads/178e3d805c9a0fd9c5ad95e4efafa1c3.png"
          />
          &nbsp;
        </p>
      </td>
    </tr>
    <tr>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <strong>Nội dung gửi kèm mã xác thực:</strong>
          <span style="color:rgb(0,120,212);">&nbsp;</span>
        </p>
        <p style="margin-left:0px;text-align:center;">
          &nbsp;
          <br />
          <img
            class="image_resized"
            style="width:243px;"
            src="https://stc-oa.zdn.vn/uploads/fd570f0d04e02aed9563b0edeccfe8c5.png"
          />
          &nbsp;
        </p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <img
            class="image_resized"
            style="width:44px;"
            src="https://stc-oa.zdn.vn/uploads/ccfa2437879f54b0a323eaed34da4e3c.png"
          />
          &nbsp;
        </p>
      </td>
      <td>
        <p style="margin-left:0px;text-align:center;">
          <img
            class="image_resized"
            style="width:46px;"
            src="https://stc-oa.zdn.vn/uploads/f58ad0f0d4a2c61d7042197cbebe6e79.png"
          />
          &nbsp;
        </p>
      </td>
    </tr>
  </tbody>
</table>
</div>

**Lưu ý:** Mẫu tin ZNS Xác thực không hỗ trợ sử dụng nút CTA. Trong trường hợp xác thực tài khoản, doanh nghiệp có thể ngoại lệ gửi thông báo đến khách hàng chưa phát sinh giao dịch với OA.

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/0fda1184d57035a621a484d173c4f1ab.png" />
</p>

_<p align="center">Hình ảnh minh hoạ mẫu tin ZNS Xác thực ở cả 2 giao diện sáng và tối</p>_

## 3. Hướng dẫn tạo mẫu tin ZNS Xác thực trên trang tài khoản ZCA:

**Xem thêm:** [**Các bước thiết lập ban đầu để gửi ZNS**](https://zalo.cloud/zns/guidelines/set-up)

_**Bước 1:**_ Truy cập vào trang tài khoản [**ZCA**](https://account.zalo.cloud/spending/overview) và chọn **“Dịch vụ ZNS”**

![](https://stc-oa.zdn.vn/uploads/e8bd8069b8b228fcb09ddac86927ff65.png)

_**Bước 2:**_ Tại trang [**“Dịch vụ ZNS”**](https://account.zalo.cloud/9GUDMAJZZREQ9MZP/tool/zns/manage/template), chọn [**“Tạo mẫu ZNS”**](https://account.zalo.cloud/tool/zns/createTemplate)

![](https://stc-oa.zdn.vn/uploads/b65fbf3254201d2f1a439793d095d43c.png)

_**Bước 3:**_ Thiết lập các thông tin chung

Nhập tên mẫu ZNS, chọn OA và Ứng dụng (AppID) để gửi ZNS

![](https://stc-oa.zdn.vn/uploads/2ec2dd87befdda0612c275efbedf4f83.png)

_**Bước 4:**_ Tại trang **“Khai báo nội dung”**, chọn loại ZNS **“ZNS Xác thực”**. Sau đó, thao tác tải logo lên và điều chỉnh **“Nội dung gửi kèm mã OTP”** phù hợp với nhu cầu sử dụng rồi nhấn **“Tiếp tục”**.

![](https://stc-oa.zdn.vn/uploads/3436683c88056aabccb842978f11d2a8.png)

_**Bước 5:**_ Nhập nội dung truyền vào tham số, tick vào mục **“đồng ý với Điều khoản và Chính sách sử dụng của Zalo Cloud”** rồi nhấn **“Hoàn thành”**.

![](https://stc-oa.zdn.vn/uploads/da993decbb75dbdc27f768d08ee12218.png)

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ Chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
