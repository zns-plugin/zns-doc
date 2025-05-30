---
id: cap-nhat-moi-zns-yeu-cau-thanh-toan-payment-request
title: Giới thiệu về mẫu thông báo ZNS Yêu cầu thanh toán (Payment Request)
slug: /cap-nhat-moi-zns-yeu-cau-thanh-toan-payment-request
---

# <p align="center">Giới thiệu về mẫu thông báo ZNS Yêu cầu thanh toán (ZNS Payment Request)</p>

Với tinh thần luôn luôn lắng nghe và thấu hiểu nhu cầu của khách hàng muốn trải nghiệm mua sắm thuận tiện và dễ dàng, đội ngũ nghiên cứu và phát triển sản phẩm Zalo Notification Service (ZNS) chính thức ra mắt mẫu ZNS Yêu cầu thanh toán (Payment Request) như một giải pháp toàn diện, mang lại giải pháp Yêu cầu thanh toán tiện lợi, dễ hiểu giữa Doanh nghiệp và khách hàng của mình.

## 1. Lợi ích khi sử dụng ZNS Yêu cầu thanh toán (Payment Request)

Với phương thức hay dạng template truyền thống, người dùng cuối (user) phải thao tác nhiều bước để thực hiện thao tác thanh toán.   
Template **ZNS Yêu cầu thanh toán** mới, hỗ trợ nút **Thanh toán ngay**, cho phép user thao tác thanh toán thuận lợi, hạn chế rủi ro do lỗi chủ quan.

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/b023e9d92376a4030d41ae2ab384ab7e.jpg" />
</p>

## 2. Cấu trúc của Template ZNS Yêu cầu thanh toán (Payment Request)

Cấu trúc của **ZNS Yêu cầu thanh toán** bao gồm:

- Các thành phần logo, văn bản, bảng, CTA… tùy chọn.
- Card thanh toán với nút **Thanh toán ngay** vô cùng tiện dụng và dễ hiểu.

Mẫu template này áp dụng các **Quy định chung khi kiểm duyệt mẫu ZNS**, quý khách có thể xem thêm tại [**ĐÂY**](https://zalo.cloud/news/quy-dinh-chung-khi-kiem-duyet-mau-tin-zns/baujzpyvjjrz7776m).

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/3c1a1704c72b6d016219d55bb7da9a51.png" />
</p>

## 3. Thao tác của người dùng khi thanh toán với ZNS Yêu cầu thanh toán (Payment Request)

Để tiện lợi cho user tiến hành thanh toán bằng nhiều ngân hàng khác nhau, Zalo đã tiến hành liên kết với nhiều ngân hàng lớn tại Việt Nam.

Khi user chọn thanh toán bằng một ngân hàng đã liên kết với Zalo, tất cả thông tin về tài khoản thụ hưởng như ngân hàng, số tài khoản, số tiền, ghi chú,… đều sẽ được tự động đồng bộ, đồng thời dẫn sang Ứng dụng của ngân hàng tương ứng. User sẽ không cần sao chép thủ công các thông tin này nữa.

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/dec12d9541d01ee0ce583f7385f8e34a.png" />
</p>

_<p align="center">Các bước thao tác của người dùng (Người dùng chọn chuyển tiền bằng với ngân hàng đã liên kết Zalo)</p>_

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/71fbfbbce1a22e87365b407bb14cb114.png" />
</p>

_<p align="center">Các bước thao tác của người dùng (Người dùng chọn chuyển tiền bằng ngân hàng chưa liên kết Zalo)</p>_

**Lưu ý:**

- Nếu user chọn thanh toán bằng ngân hàng chưa liên kết với Zalo, user sẽ cần chủ động thao tác để sao chép các thông tin thanh toán.
- Khi user click nút **“Thanh toán ngay”**, Zalo sẽ hiển thị những Ngân hàng có Ứng dụng (App) đã được cài đặt trên thiết bị của người dùng.
- Các ngân hàng đã liên kết với Zalo sẽ có biểu tượng phía bên phải ![](https://stc-oa.zdn.vn/uploads/0f14ebd01e5692c664fa6d1c21238efe.png)
- Danh sách các ngân hàng đã liên kết với Zalo (Cập nhật đến 18/07/2024, xem thêm tại [LINK](https://help.zalo.me/huong-dan/chuyen-muc/nhan-tin-va-goi/nhan-tin/ho-tro-chuyen-khoan-ngan-hang-nhanh-ngay-tu-tin-nhan-zalo/?gidzl=vXOz5NyfZJlY3peJUZ-CDE8EEnrbCOarzGfg6JbaZMIaNsaVD3MDDVW8FXmmPOnc-Wa-J32f28OVVIwCEm&gidzl=tCXnRm2TAG3GrtXg18ie3zFVUcOOZYzOdjn-OqhUB0Z9stip7OylNfoFAp9Ctta9dzyWCMFbP61T2fKc1W&gidzl=jKQIK0M9EcMmKP9I1PyxQxLRaLmVc3eu-LZ12H_AEp3-39PLJfyzO_vGbLD9n3nc-G2JKcI4zfa00eOuPm)):
  1.  Ngân hàng TMCP Kỹ thương Việt Nam (Techcombank)
  2.  Ngân hàng TMCP Đầu tư và Phát triển Việt Nam (BIDV)
  3.  Ngân hàng TMCP Việt Nam Thịnh Vượng (VPBank)
  4.  Ngân hàng TMCP Phương Đông (OCB) _(tạm ngừng hỗ trợ do bảo trì liên kết)_
  5.  Ngân hàng TMCP Tiên Phong (TPBank)
  6.  Ngân hàng TMCP Nam Á (NamABank)
  7.  Ngân hàng TMCP Hàng Hải (MSB)
  8.  Ngân hàng TMCP Đại Chúng Việt Nam (PVcomBank)
  9.  Ngân hàng TMCP PT Thành phố Hồ Chí Minh (HDBank)
  10. Ngân hàng TMCP Bản Việt (BVBank)

## 4. Cách đăng ký mẫu ZNS Yêu cầu thanh toán

Mẫu template này áp dụng các **Quy định chung khi kiểm duyệt mẫu ZNS**, quý khách có thể xem thêm tại [**ĐÂY**](https://zalo.cloud/news/quy-dinh-chung-khi-kiem-duyet-mau-tin-zns/baujzpyvjjrz7776m).

**Hướng dẫn đăng ký mẫu ZNS Yêu cầu thanh toán:**

**Bước 1:** Tại [Zalo Cloud Account (ZCA)](https://account.zalo.cloud/) → Truy cập [Tạo mẫu ZNS](https://account.zalo.cloud/tool/zns/createTemplate) → Chọn **ZNS yêu cầu thanh toán**

![](https://stc-oa.zdn.vn/uploads/89dc23844aab407eb8edb1c0524cdda4.png)

**Bước 2:** Với **ZNS yêu cầu thanh toán**, quý khách cần sử dụng Logo. Ngoài ra, quý khách có thể tùy chỉnh số lượng Văn bản và Bảng, sử dụng tùy chọn CTA theo nhu cầu.

**Bước 3:** Điền thông tin thanh toán (thông tin tài khoản thụ hưởng)

![](https://stc-oa.zdn.vn/uploads/de3ca369d5707b4b0a770de9534b086b.png)

_Mục điền thông tin thanh toán_

- **Chi tiết lưu ý như sau:**  
  **Tài khoản thụ hưởng cần là thông tin tài khoản doanh nghiệp sở hữu OA.** Trong trường hợp khác, vui lòng ghi chú vào phần Ghi chú kiểm duyệt và cung cấp giấy tờ chứng minh: Chủ tài khoản là chủ doanh nghiệp hoặc người đại diện pháp lý của doanh nghiệp/Chủ tài khoản được doanh nghiệp ủy quyền thu hộ. \=> Xem thêm tại [LINK](https://zalo.cloud/news/quy-dinh-chung-khi-kiem-duyet-mau-tin-zns/baujzpyvjjrz7776m)

  - **Ngân hàng:**
    - Chọn ngân hàng theo danh sách có sẵn
  - **Tên tài khoản**:
    - Tên tài khoản cần khớp với tên doanh nghiệp sở hữu OA
  - **Số tài khoản**
    - Lưu ý điền đúng format số tài khoản:
      - 33281826868 **✓**
      - 3328 1826 868**✗**
  - **Số tiền:**

    - **Format:** 100000 **✓** 100.000 **✗**
    - **Giới hạn:** Lớn hơn 2.000 VND và nhỏ hơn 500.000.000 VND
    - Truyền tham số, hoặc điền số tiền cố định.

  - **Nội dung chuyển khoản**:
    - **Format:** Không chứa ký tự đặc biệt `@\[\]^\_!"•#$%¥&'()\*+,€-./:;{|<}=~>?.`)
    - Truyền tham số, hoặc điền nội dung cố định.

**Lưu ý:**

- **Thông tin tài khoản thụ hưởng cần là thông tin của chính doanh nghiệp sở hữu OA.** Trong trường hợp khác, vui lòng ghi chú vào phần Ghi chú kiểm duyệt và cung cấp giấy tờ chứng minh: Chủ tài khoản là chủ doanh nghiệp hoặc người đại diện pháp lý của doanh nghiệp/Chủ tài khoản được doanh nghiệp ủy quyền thu hộ.   
  → Xem thêm tại [LINK](https://zalo.cloud/news/quy-dinh-chung-khi-kiem-duyet-mau-tin-zns/baujzpyvjjrz7776m)
- Chỉ hỗ trợ sử dụng tham số cho thông tin tài khoản với một số khách hàng phù hợp (với các điều kiện liên quan đến ngành nghề kinh doanh, sản lượng và tần suất sử dụng ZNS,…).
- **Quý khách vui lòng kiểm tra kĩ thông tin thanh toán, Zalo không chịu trách nhiệm nếu thông tin thanh toán không chính xác.**

## 5. Chuẩn hóa các template mục đích Yêu cầu thanh toán

Để chuẩn hóa và tối ưu sản phẩm, với sự ra mắt template Yêu cầu thành toán, tất cả các template có mục đích Yêu cầu thanh toán, trả cước, trả phí đến một số tài khoản ngân hàng nhất định **bắt buộc** sử dụng ZNS yêu cầu thanh toán.

_Chi tiết quy định xem tại_ [_Quy định chung khi kiểm duyệt mẫu ZNS_](https://zalo.cloud/news/quy-dinh-chung-khi-kiem-duyet-mau-tin-zns/baujzpyvjjrz7776m) _(Yêu cầu theo mục đích - Tag 1 - về Yêu cầu thanh toán, trả cước, trả phí,..)_

**Các template ID sử dụng định dạng (format) template ZNS thông tin Thanh toán (cũ) hoặc các format khác có mục đích Yêu cầu thanh toán, trả cước, trả phí đến một số tài khoản ngân hàng nhất định sẽ ngừng hỗ trợ từ 01/08/2024**. Quý Đối tác vui lòng sắp xếp và đăng ký template ZNS yệu cầu thanh toán (mới) để thay thế trước 31/07/2024 để tránh ảnh hưởng vận hành.

## 6. Danh sách mã BIN

BIN viết tắt cho Bank Identification Number - Mã định danh ngân hàng theo Ngân hàng Nhà nước Việt Nam.

<div class="table" align="center">
  <table>
    <tbody>
      <tr>
        <td>
          <strong>BIN Code</strong>
        </td>
        <td>
          <strong>Tên ngân hàng</strong>
        </td>
      </tr>
      <tr>
        <td>970425&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP An Bình (ABBANK)</td>
      </tr>
      <tr>
        <td>970416&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Á Châu (ACB)</td>
      </tr>
      <tr>
        <td>970405&nbsp;&nbsp;</td>
        <td>
          Ngân hàng Nông nghiệp và Phát triển Nông thôn Việt Nam (Agribank)
        </td>
      </tr>
      <tr>
        <td>970409&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Bắc Á (BacABank)</td>
      </tr>
      <tr>
        <td>970438&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Bảo Việt (BaoVietBank)</td>
      </tr>
      <tr>
        <td>970418&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Đầu tư và Phát triển Việt Nam (BIDV)</td>
      </tr>
      <tr>
        <td>546034&nbsp;&nbsp;</td>
        <td>Ngân hàng số CAKE by VPBank (CAKE)</td>
      </tr>
      <tr>
        <td>970444&nbsp;&nbsp;</td>
        <td>Ngân hàng TM TNHH MTV Xây dựng Việt Nam (CBBank)</td>
      </tr>
      <tr>
        <td>422589&nbsp;&nbsp;</td>
        <td>Ngân hàng TNHH MTV CIMB Việt Nam (CIMB)</td>
      </tr>
      <tr>
        <td>970446&nbsp;&nbsp;</td>
        <td>Ngân hàng Hợp tác xã Việt Nam (COOPBANK)</td>
      </tr>
      <tr>
        <td>796500&nbsp;&nbsp;</td>
        <td>DBS Bank Ltd - Chi nhánh TP. Hồ Chí Minh (DBSBank)</td>
      </tr>
      <tr>
        <td>970406&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Đông Á (DongABank)</td>
      </tr>
      <tr>
        <td>970431&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Xuất Nhập khẩu Việt Nam (Eximbank)</td>
      </tr>
      <tr>
        <td>970408&nbsp;&nbsp;</td>
        <td>Ngân hàng Thương mại TNHH MTV Dầu Khí Toàn Cầu (GPBank)</td>
      </tr>
      <tr>
        <td>970437&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP PT Thành phố Hồ Chí Minh (HDBank)</td>
      </tr>
      <tr>
        <td>970442&nbsp;&nbsp;</td>
        <td>Ngân hàng TNHH MTV Hong Leong Việt Nam (HongLeong)</td>
      </tr>
      <tr>
        <td>458761&nbsp;&nbsp;</td>
        <td>Ngân hàng TNHH MTV HSBC (Việt Nam) (HSBC)</td>
      </tr>
      <tr>
        <td>970456&nbsp;&nbsp;</td>
        <td>
          Ngân hàng Công nghiệp Hàn Quốc - Chi nhánh TP. Hồ Chí Minh (IBKHCM)
        </td>
      </tr>
      <tr>
        <td>970455&nbsp;&nbsp;</td>
        <td>Ngân hàng Công nghiệp Hàn Quốc - Chi nhánh Hà Nội (IBKHN)</td>
      </tr>
      <tr>
        <td>970434&nbsp;&nbsp;</td>
        <td>Ngân hàng TNHH Indovina (IndovinaBank)</td>
      </tr>
      <tr>
        <td>668888&nbsp;&nbsp;</td>
        <td>Ngân hàng Đại chúng TNHH Kasikornbank (KBank)</td>
      </tr>
      <tr>
        <td>970452&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Kiên Long (KienLongBank)</td>
      </tr>
      <tr>
        <td>970463&nbsp;&nbsp;</td>
        <td>Ngân hàng Kookmin - Chi nhánh Tp. Hồ Chí Minh (KookminHCM)</td>
      </tr>
      <tr>
        <td>970462&nbsp;&nbsp;</td>
        <td>Ngân hàng Kookmin - Chi nhánh Hà Nội (KookminHN)</td>
      </tr>
      <tr>
        <td>970449&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Bưu Điện Liên Việt (LienVietPostBank)</td>
      </tr>
      <tr>
        <td>970422&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Quân đội (MBBank)</td>
      </tr>
      <tr>
        <td>970426&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Hàng Hải (MSB)</td>
      </tr>
      <tr>
        <td>970428&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Nam Á (NamABank)</td>
      </tr>
      <tr>
        <td>970419&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Quốc Dân (NCB)</td>
      </tr>
      <tr>
        <td>801011&nbsp;&nbsp;</td>
        <td>Ngân hàng Nonghyup - Chi nhánh Hà Nội (Nonghyup)</td>
      </tr>
      <tr>
        <td>970448&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Phương Đông (OCB)</td>
      </tr>
      <tr>
        <td>970414&nbsp;&nbsp;</td>
        <td>Ngân hàng Thương mại TNHH MTV Đại Dương (Oceanbank)</td>
      </tr>
      <tr>
        <td>970430&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Xăng dầu Petrolimex (PGBank)</td>
      </tr>
      <tr>
        <td>970439&nbsp;&nbsp;</td>
        <td>Ngân hàng TNHH MTV Public Việt Nam (PublicBank)</td>
      </tr>
      <tr>
        <td>970412&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Đại Chúng Việt Nam (PVcomBank)</td>
      </tr>
      <tr>
        <td>970403&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Sài Gòn Thương Tín (Sacombank)</td>
      </tr>
      <tr>
        <td>970400&nbsp;</td>
        <td>Ngân hàng TMCP Sài Gòn Công Thương (SaigonBank)</td>
      </tr>
      <tr>
        <td>970429&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Sài Gòn (SCB)</td>
      </tr>
      <tr>
        <td>970440&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Đông Nam Á (SeABank)</td>
      </tr>
      <tr>
        <td>970443&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Sài Gòn - Hà Nội (SHB)</td>
      </tr>
      <tr>
        <td>970424&nbsp;&nbsp;</td>
        <td>Ngân hàng TNHH MTV Shinhan Việt Nam (ShinhanBank)</td>
      </tr>
      <tr>
        <td>970410&nbsp;&nbsp;</td>
        <td>Ngân hàng Standard Chartered Việt Nam (Standard Chartered)</td>
      </tr>
      <tr>
        <td>970407&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Kỹ thương Việt Nam (Techcombank)</td>
      </tr>
      <tr>
        <td>970423&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Tiên Phong (TPBank)</td>
      </tr>
      <tr>
        <td>546035&nbsp;&nbsp;</td>
        <td>Ngân hàng số Ubank by VPBank (Ubank)</td>
      </tr>
      <tr>
        <td>970458&nbsp;&nbsp;</td>
        <td>
          Ngân hàng United Overseas - Chi nhánh TP. Hồ Chí Minh (United
          Overseas)
        </td>
      </tr>
      <tr>
        <td>970441&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Quốc tế Việt Nam (VIB)</td>
      </tr>
      <tr>
        <td>970427&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Việt Á (VietABank)</td>
      </tr>
      <tr>
        <td>970433&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Việt Nam Thương Tín (VietBank)</td>
      </tr>
      <tr>
        <td>970454&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Bản Việt (BVBank)</td>
      </tr>
      <tr>
        <td>970436&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Ngoại Thương Việt Nam (Vietcombank)</td>
      </tr>
      <tr>
        <td>970415&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Công thương Việt Nam (VietinBank)</td>
      </tr>
      <tr>
        <td>970432&nbsp;&nbsp;</td>
        <td>Ngân hàng TMCP Việt Nam Thịnh Vượng (VPBank)</td>
      </tr>
      <tr>
        <td>970421&nbsp;&nbsp;</td>
        <td>Ngân hàng Liên doanh Việt - Nga (VRB)</td>
      </tr>
      <tr>
        <td>970457&nbsp;&nbsp;</td>
        <td>Ngân hàng TNHH MTV Woori Việt Nam (Woori)</td>
      </tr>
    </tbody>
  </table>
</div>

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của Zalo Cloud qua email: support@zalo.cloud. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
