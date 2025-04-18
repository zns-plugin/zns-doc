---
id: cac-quy-dinh-xet-duyet-template-zns-chua-module-hinh-anh
title: Các quy định xét duyệt Template ZNS chứa module hình ảnh
slug: /cac-quy-dinh-xet-duyet-template-zns-chua-module-hinh-anh
---

# <p style="text-align: center">Các quy định xét duyệt mẫu thông báo ZNS chứa module hình ảnh</p>

Với kế hoạch ra mắt tính năng cho phép bổ sung hình ảnh cho mẫu tin thông báo ZNS để gia tăng tính tương tác giúp doanh nghiệp có thể truyền đạt thông điệp chăm sóc khách hàng của mình - ở đây là người dùng cuối (end-user).

Bộ phận phát triển sản phẩm Zalo Cloud ra bộ Quy định xét duyệt Template ZNS chứa module hình ảnh như bên dưới

## A. Thông tin cơ bản

### 1. Định nghĩa

- Module hình ảnh là tập hợp một hoặc nhiều ảnh trong nội dung mẫu tin ZNS. Module hình ảnh được đính kèm vào template, là một thành phần của template.

- Template chứa ảnh là template được đính kèm module hình ảnh.

- **Xem thêm** [**Hướng dẫn Tính Năng Thiết Lập Hình Ảnh Trong Mẫu Tin ZNS**](https://zalo.cloud/news/ra-mat-tinh-nang-thiet-lap-hinh-anh-trong-mau-tin-zns/vvupr9ymqqbvdm96by)

### 2. Mục đích của module hình ảnh

- Tăng tương tác, minh họa cho phần nội dung của mẫu tin ZNS. Đồng thời, module hình ảnh giúp tăng nhận diện thương hiệu cho doanh nghiệp.

- Hình ảnh giúp end-user khi nhận được thông báo ZNS có thể nắm bắt được thông tin một cách nhanh chóng hơn.

- Module hình ảnh là thành phần phụ/bổ trợ cho nội dung chính của template.

- Module hình ảnh giúp tăng tỉ lệ và diện tích tương tác của end-user với thông báo ZNS (thông qua click vào ảnh để mở đường link CTA).

### 3. Nguyên tắc trọng tâm

Hình ảnh là một thành phần của nội dung template, vì vậy, nội dung hình ảnh cần liên quan đến các nội dung khác của template.

## B. Quy định về kỹ thuật

<div class="table">
<table>
  <tbody>
    <tr>
      <td colspan="2">
        <p style="text-align:center;">
          <strong>Quy định về kỹ thuật</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>Cơ bản</td>
      <td>
        Một module hình ảnh có tối thiểu 1 ảnh và tối đa 3 ảnh.
        <br />
        Module hình ảnh (nếu có) nằm ở vị trí trên cùng (header) của template.
        Nếu trong một template, đã có module ảnh thì không được có module logo
        và ngược lại.
      </td>
    </tr>
    <tr>
      <td>Tỉ lệ</td>
      <td>Tỉ lệ 16:9 (ngang)</td>
    </tr>
    <tr>
      <td>Kích thước</td>
      <td>=&lt; 500kb</td>
    </tr>
    <tr>
      <td>Định dạng cho phép</td>
      <td>.jpg và .png</td>
    </tr>
    <tr>
      <td>Nút thao tác (CTA)</td>
      <td>
        Với tất cả các mẫu tin (template) ZNS hình ảnh, bắt buộc có CTA
        <br />
        Khi bấm vào hình ảnh sẽ được dẫn theo link/số điện thoại tại chút chính
        (CTA 1)
      </td>
    </tr>
    <tr>
      <td>Khả năng tích hợp</td>
      <td>
        Module hình ảnh có thể tích hợp với tất cả dạng template, ngoại trừ:
        <br />- Template Rating
        <br />- Template Mã xác thực
      </td>
    </tr>
  </tbody>
</table>
</div>

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/603daeeaf36857e16181f8ea4484e320.jpg" />
</p>

## C. Quy định về mục đích

<div class="table">
<table>
  <tbody>
    <tr>
      <td colspan="2">
        <p style="text-align:center;">
          <strong>Quy định về mục đích</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>Về mục đích gửi của template chứa module hình ảnh</td>
      <td>
        Mẫu tin chứa hình ảnh có thể gửi ở bất kỳ mục đích nào (trừ mục đích gửi
        mã xác thực - Tag 0)
      </td>
    </tr>
  </tbody>
</table>
</div>

Xem thêm cách [Thiết lập mục đích gửi khi tạo mẫu ZNS](https://zalo.cloud/blog/thiet-lap-muc-dich-gui-khi-tao-mau-zns/erug88djjgrd9r7zzj)

## D. Quy định về hình thức của module hình ảnh

<div class="table">
<table>
  <tbody>
    <tr>
      <td colspan="2">
        <p style="text-align:center;">
          <strong>Quy định về hình thức</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td rowspan="2">Về thành phần chữ (text) bên trong hình ảnh</td>
      <td>
        Thành phần text cần rõ ràng, dễ đọc.
        <br />
        Không chấp nhận thành phần text không rõ ràng, quá nhỏ gây khó đọc.
      </td>
    </tr>
    <tr>
      <td>
        Tổng diện tích của thành phần text không được chiếm quá 50% diện tích
        hình ảnh.
      </td>
    </tr>
    <tr>
      <td rowspan="9">Về tổng quan hình ảnh</td>
      <td>
        <p>
          Hình trong ảnh phải rõ ràng dễ nhận biết, không chấp nhận các hình ảnh
          quá mờ, quá nhỏ, không thể nhận ra.&nbsp;
        </p>
        <figure class="image image_resized" style="width:202px;">
          <img src="https://stc-oa.zdn.vn/uploads/5a3cfd6ed92862fd0e2145dd8490316e.png" />
        </figure>
      </td>
    </tr>
    <tr>
      <td>Không chấp nhận các hình ảnh được chỉnh sửa/cắt ghép sơ sài.</td>
    </tr>
    <tr>
      <td>Hình ảnh không được chứa các mã QR/Barcode.</td>
    </tr>
    <tr>
      <td>
        Không chấp nhận ảnh có trắng nền xung quanh không liên quan về mặt thiết
        kế.
      </td>
    </tr>
    <tr>
      <td>Không chấp nhận ảnh được đóng khung hoặc gắn viền nổi bật.</td>
    </tr>
    <tr>
      <td>
        <p>
          Không chấp nhận sử dụng một ảnh mà layout bị chia thành nhiều ảnh nhỏ
          bên trong.
        </p>
        <figure class="image">
          <img src="https://stc-oa.zdn.vn/uploads/8644d9d98d49feb7dd4ae20878fd85e0.png" />
        </figure>
      </td>
    </tr>
    <tr>
      <td>
        <p>
          Không chấp nhận hình ảnh có thành phần mang yếu tố đánh lừa/gây hiểu
          lầm là đánh lừa người dùng (end-user) click vào:
          <br />- Hình ảnh làm giả nút bấm play video, nút tắt quảng cáo, nút di
          chuyển hình hoặc thành phần trang web mà không có tác dụng,...
        </p>
        <figure class="image image_resized" style="width:326px;">
          <img src="https://stc-oa.zdn.vn/uploads/bfd23151648e07e74414534cb0607a98.png" />
        </figure>
        <p>
          <br />- Hình ảnh bắt chước hoặc giống hộp thoại hay thông báo lỗi của
          Windows, Mac, Unix, hoặc&nbsp; hệ điều hành khác.
        </p>
      </td>
    </tr>
    <tr>
      <td>
        Không cho phép hình ảnh có thông tin mời liên hệ Số điện thoại (SĐT cần
        được dẫn tại Nút thao tác - CTA)&nbsp;
      </td>
    </tr>
    <tr>
      <td>
        Hình ảnh không được chứa các hình, biểu tượng,... trái quy định của Pháp
        luật Việt Nam và các quy định khác của nền tảng Zalo.
      </td>
    </tr>
  </tbody>
</table>
</div>

![](https://stc-oa.zdn.vn/uploads/66c1e3c91ea8667cadaf8b9c527ed6e5.jpg)

**Ví dụ về kích thước chữ đề xuất:**

![](https://stc-oa.zdn.vn/uploads/781d7e7c6b8c095fce9ee112d9a86b51.jpg)

_<p align="center">Với kích thước ảnh 1140px x 640px - kích thước thành phần chữ đề xuất ở mức tối thiểu 42pt - tối ưu nhất 56pt</p>_

Các kích thước thành phần chữ không yêu cầu bắt buộc tương tự, nhưng cần đảm bảo các quy đinh và chính sách của sản phẩm ZNS.

## E. Quy định về thương hiệu trong ảnh

<div class="table">
<table>
  <tbody>
    <tr>
      <td colspan="2">
        <p style="text-align:center;">
          <strong>Quy định về thương hiệu trong hình ảnh</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>Về Logo của chính doanh nghiệp</td>
      <td>
        Logo của thương hiệu trong ảnh, nếu có, phải rõ ràng, dễ nhận biết.
      </td>
    </tr>
    <tr>
      <td rowspan="2">Về Logo của chính doanh nghiệp, cơ quan, tổ chức khác</td>
      <td>
        Hình ảnh không được chứa logo của các cơ quan chính phủ, hoặc của các
        nhãn hiệu, thương hiệu khác mà không có sự cho phép.&nbsp;
        <br />
        Nếu có, khách hàng cần cung cấp bằng chứng về việc sở hữu logo, thương
        hiệu hoặc ủy quyền, chấp thuận sử dụng thương hiệu.
      </td>
    </tr>
    <tr>
      <td>
        Không cho phép hình ảnh dạng censored (hiệu ứng che, ẩn, làm mờ) một
        phần hoặc toàn bộ brandname/logo của thương hiệu khác.
      </td>
    </tr>
  </tbody>
</table>
</div>

## F. Quy định chung về nội dung

![](https://stc-oa.zdn.vn/uploads/1d9642c58783e247d539156292d6f66c.jpg)

<div class="table">
<table>
  <tbody>
    <tr>
      <td colspan="2">
        <p style="text-align:center;">
          <strong>Quy định về nội dung</strong>
        </p>
      </td>
    </tr>
    <tr>
      <td>Quy định chung về nội dung</td>
      <td>
        Hình ảnh là nội dung bổ trợ/phụ trợ trong mẫu thông báo ZNS, vẫn phải
        đáp ứng chính sách và quy định của nền tảng Zalo nói chung.
      </td>
    </tr>
    <tr>
      <td rowspan="15">Về nội dung hình ảnh chi tiết</td>
      <td>
        Không cho phép có thành phần nội dung chính của hình ảnh là mời follow
        OA
      </td>
    </tr>
    <tr>
      <td>
        Không được sử dụng hình ảnh chụp giấy tờ, văn bản hành chính trên hình
        ảnh quảng cáo, bao gồm: Giấy chứng nhận quyền sử dụng đất (sổ đỏ), các
        loại giấy tờ từ cơ quan Nhà nước, giấy phép liên quan đến sản phẩm (Giấy
        xác nhận nội dung quảng cáo, giấy công bố, giấy an toàn vệ sinh thực
        phẩm…), thẻ bảo hiểm y tế, hợp đồng, và các loại giấy tờ tương tự khác.
      </td>
    </tr>
    <tr>
      <td>
        Không được sử dụng các hình ảnh mồ mả, nghĩa trang, bia mộ hoặc những
        hình ảnh tương tự.
      </td>
    </tr>
    <tr>
      <td>
        Không được sử dụng hình ảnh thuốc lá, khói thuốc lá, thuốc lá điện tử và
        các dạng thuốc lá khác.
      </td>
    </tr>
    <tr>
      <td>Không sử dụng hình ảnh kim tiêm, ống chích, dao kéo, vũ khí.</td>
    </tr>
    <tr>
      <td>
        Không sử dụng hình ảnh của lá cờ Việt Nam hoặc bản đồ hoặc tiền Việt
        Nam. Không dùng ảnh quân nhân, chính trị.
      </td>
    </tr>
    <tr>
      <td>
        Hình ảnh không được khai thác các vấn đề chính sách, giới tính, tôn
        giáo, tình dục hoặc các vấn đề nhạy cảm khác.
      </td>
    </tr>
    <tr>
      <td>
        Hình ảnh quảng cáo không được chứa bộ phận cơ thể được zoom in vượt quá
        50% diện tích hình quảng cáo đó.
      </td>
    </tr>
    <tr>
      <td>
        Hình ảnh không được gợi dục, ngụ ý khỏa thân, hở da, khoe thân hoặc tập
        trung một cách không cần thiết vào các bộ phận cơ thể, hình ảnh mô tả
        con người ở tư thế khiêu dâm, các hoạt động khêu gợi hoặc kích thích quá
        mức.
      </td>
    </tr>
    <tr>
      <td>
        Không sử dụng hình ảnh gây cảm giác tiêu cực cho người xem. Ví dụ, người
        bệnh, chứng bệnh một cách không sạch sẽ: ví dụ người gầy trơ xương, lở
        loét, đau đớn, highlight chỗ đau bằng các vòng tròn đỏ, người bụng phệ
        chảy xệ, vết thương hở và máu me,…
      </td>
    </tr>
    <tr>
      <td>
        Không được sử dụng hình ảnh chứa kết quả bất ngờ, không thể xảy ra.
      </td>
    </tr>
    <tr>
      <td>
        Không được sử dụng các hình ảnh gây chấn động hoặc gây sợ hãi, hình ảnh
        chứa hoặc khơi gợi các từ ngữ, nội dung phản cảm, bạo lực, không thân
        thiện với bất kỳ nhóm người dùng nào.
      </td>
    </tr>
    <tr>
      <td>
        Không được chứa sản phẩm (thuốc cấm, thực phẩm cấm, tiền ảo/crypto, vay
        cá nhân...) / dịch vụ / sản phẩm cấm nói chung.
      </td>
    </tr>
    <tr>
      <td>
        Không cho phép hình ảnh có thông tin kêu gọi mời vào group chat. &nbsp;
      </td>
    </tr>
    <tr>
      <td>
        Hình ảnh không được chưa các hình, biểu tưởng,... trái quy định của Pháp
        luật Việt Nam và các quy định khác của nền tảng Zalo tại thời điểm xét
        duyệt
      </td>
    </tr>
  </tbody>
</table>
</div>

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ Chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
