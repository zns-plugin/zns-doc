---
id: nut-thao-tac-cta
title: Nút thao tác CTA trong mẫu thông báo ZNS
slug: /nut-thao-tac-cta
---

# <p align ="center">Nút thao tác CTA trong mẫu thông báo ZNS</p>

Nhằm hỗ trợ khách hàng khai thác tối đa nội dung/mục đích và tối ưu hóa dịch vụ Zalo Notification Service (ZNS), Zalo Cloud giới thiệu nút thao tác (CTA) trong nội dung thông báo ZNS. Bài viết này sẽ hướng dẫn quý khách triển khai tính năng này hiệu quả nhất. 

## 1. Giới thiệu về nút thao tác CTA:

*   Nút thao tác (CTA – Call to Action) là nút gắn kèm trong nội dung mẫu thông báo ZNS, cho phép người nhận click để thực hiện các thao tác bao gồm:
*   Gọi điện liên hệ số điện thoại được doanh nghiệp cung cấp
*   Truy cập đường dẫn (link) được doanh nghiệp cung cấp
*   Nội dung nút thao tác có thể được tùy chỉnh tùy theo nhu cầu sử dụng của doanh nghiệp. Với mỗi mẫu ZNS, bạn có thể thêm tối đa 2 nút thao tác (nút chính và nút phụ).


## 2. Danh sách các loại Nút thao tác CTA:

Xem thêm tại [**Chính sách Dịch vụ ZNS**](https://zalo.cloud/terms).

<div class="table" align="center">
      <table>
<table class="ck-table-resized"><colgroup><col style="width:7.24%;"><col style="width:36.49%;"><col style="width:23.25%;"><col style="width:33.02%;"></colgroup><tbody><tr><td style="background-color:#1E8BCD;border-color:black;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;"><p style="margin-left:0in;text-align:center;"><strong>#</strong></p></td><td style="background-color:#1E8BCD;border-bottom-style:solid;border-color:black;border-left-style:none;border-right-style:solid;border-top-style:solid;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:158.55pt;"><p style="margin-left:0in;text-align:center;"><strong>Tiêu đề</strong></p></td><td style="background-color:#1E8BCD;border-bottom-style:solid;border-color:black;border-left-style:none;border-right-style:solid;border-top-style:solid;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:81.95pt;"><p style="margin-left:0in;text-align:center;"><strong>Đơn giá nút chính (VND)</strong></p></td><td style="background-color:#1E8BCD;border-bottom-style:solid;border-color:black;border-left-style:none;border-right-style:solid;border-top-style:solid;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:1.5in;"><p style="margin-left:0in;text-align:center;"><strong>Đơn giá nút phụ (VND)</strong></p></td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">1</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;">Đến trang của doanh nghiệp</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">0</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">100</td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">2</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;">Gọi điện</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">0</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">100</td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">3</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;">Đến trang thông tin OA</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">0</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">100</td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">4</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;">Đến ứng dụng Zalo Mini App</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">0</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">100</td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">5</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;">Đến trang phân phối sản phẩm</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">400</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">500</td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">6</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;">Đến trang web khác</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">300</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">400</td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">7</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;"><p style="margin-left:0in;">Đến trang tải ứng dụng</p></td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">400</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">500</td></tr><tr><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.5pt;height:15.0pt;padding:0in 5.4pt;width:35.25pt;">8</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:158.55pt;">Đến trang tải ứng dụng khác</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:81.95pt;">600</td><td style="border-bottom:1.5pt solid black;border-left-style:none;border-right:1.5pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;width:1.5in;">700</td></tr></tbody></table>
</div>


## 3. Hướng dẫn thêm nút thao tác CTA vào mẫu tin ZNS:

**Bước 1**. Click **“Nút thao tác”**.

![](https://stc-oa.zdn.vn/uploads/63c38797cc26e1e48e08182bfec28a6b.png)


**Bước 2**. Chọn loại nút thao tác theo nhu cầu, tạo đường dẫn liên kết/số điện thoại mới hoặc chọn từ dữ liệu được lưu từ các mẫu tin trước.

  ![](https://stc-oa.zdn.vn/uploads/1cd2275feda0bfe46c923278e392dee6.png)![](https://stc-oa.zdn.vn/uploads/dfbde94e34e21269e42b7106e4a773bf.png)


**Bước 3.** Thêm nút thao tác thứ 2 theo nhu cầu, lặp lại các bước trước. 


## 4. Hướng dẫn thêm nút thao tác CTA vào mẫu tin ZNS:

Để có thể hỗ trợ doanh nghiệp cá nhân hóa (customize) đường dẫn gửi cho từng người dùng, Zalo Cloud chính thức mở tích hợp khả năng truyền tham số (param) vào nút thao tác (CTA) khi tạo mẫu ZNS. Tính năng này phù hợp cho nhiều doanh nghiệp thuộc nhiều ngành hàng với các nhu cầu tiêu biểu bao gồm nhưng không giới hạn như: 

*   Gửi đường dẫn định danh theo dõi đơn hàng/quá trình giao dịch
*   Gửi đường dẫn định danh các loại hóa đơn/hợp đồng
*   Gửi đường dẫn đăng nhập cho từng tài khoản độc lập
*   Gửi số điện thoại CSKH theo từng khu vực

_Xem thêm bài viết Tham số (Param) là gì? Thế nào là một tham số đúng quy chuẩn? tại_ [_**ĐÂY**_](https://zalo.cloud/blog/tham-so-param-la-gi-the-nao-la-mot-tham-so-dung-quy-chuan-/4kuprg64gyz88qewg).

**Bước 1:** Tạo nút liên kết (CTA) với tham số tương ứng và lưu nút thao tác.

*   **Đối với đường dẫn liên kết:** Tham số cần nằm ở phần path của URL, không được trùng với tham số đã sử dụng trong các phần khác của tin ZNS, và dữ liệu tham số mặc định thuộc data type URL (200). Quý khách cần đảm bảo dữ liệu truyền về được mã hóa chuẩn UTF-8 trước khi truyền vào. 

![](https://stc-oa.zdn.vn/uploads/2491f598361639034facc83b0b157ec5.png)

*   **Đối với số điện thoại:** Cho phép 1 tham số duy nhất, dữ liệu tham số mặc định thuộc data type Phone Number. 

![](https://stc-oa.zdn.vn/uploads/32d1c365f4e8bcd2a20879a24d960ff3.png)

_Hướng dẫn chi tiết Các định dạng dữ liệu khi truyền vào tham số trên nội dung ZNS có thể xem tại [**ĐÂY**](https://zalo.cloud/blog/cac-dinh-dang-du-lieu-khi-truyen-vao-tham-so-tren-noi-dung-zns/9gubbkay4yyrng86a)_.

#### **Bước 2:** Tạo mẫu ZNS thành công 

![](https://stc-oa.zdn.vn/uploads/1f135d505e68a7b7d58e96257546aeef.png) 

Sau khi tạo mẫu ZNS thành công, Quý khách vui lòng lưu ý xem mẫu ZNS hiển thị ghi chú yêu cầu đúng định dạng UTF-8. 

#### **Bước 3:** Truyền dữ liệu và gửi lệnh ZNS đến người dùng cuối 

Khi gửi thông báo ZNS, hệ thống sẽ kiểm tra tất cả các dữ liệu truyền vào các tham số. 

Với các dữ liệu truyền vào tham số (param) trong nút thao tác (CTA), dữ liệu cần chuẩn định dạng UTF-8. Nếu khách hàng chưa mã hoá hoặc mã hóa sai định dạng, hệ thống sẽ báo lỗi -132 Parameter invalid. 

Tham khảo Bảng mã lỗi khi sử dụng dịch vụ Zalo Notification Service tại [**ĐÂY**](https://developers.zalo.me/docs/api/zalo-notification-service-api/phu-luc/bang-ma-loi-post-5233). 

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
