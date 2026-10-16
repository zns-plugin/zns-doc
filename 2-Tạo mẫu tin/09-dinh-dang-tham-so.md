---
id: cac-dinh-dang-du-lieu-khi-truyen-vao-tham-so-tren-noi-dung-zbs-template-message
title: Các định dạng dữ liệu khi truyền vào tham số trên nội dung tin nhắn ZBS Template
slug: /cac-dinh-dang-du-lieu-khi-truyen-vao-tham-so-tren-noi-dung-zbs-template-message
---

# <p align="center">Các định dạng dữ liệu khi truyền vào tham số trên nội dung tin nhắn ZBS Template</p>


Dữ liệu khi truyền vào tham số (param) được hệ thống cài đặt với một số định dạng nhất định. Trong bài viết này, đội ngũ hỗ trợ khách hàng Zalo Business Solutions sẽ liệt kê các dạng khi truyền vào tham số và cách hiển thị của trên tin nhắn ZBS Template gửi đến người nhận nhằm mục đích giúp đối tác hiểu rõ hơn về cách định dạng dữ liệu trước khi truyền vào tham số cũng như các định dạng sẽ hiển thị của tin nhắn ZBS Template khi đến máy người dùng (người nhận tin nhắn ZBS Template).  

Quý khách có thể xem thêm [Tham số (Param) là gì? Thế nào là một tham số đúng quy chuẩn?](https://zalo.solutions/blog/tham-so-param-la-gi-the-nao-la-mot-tham-so-dung-quy-chuan-/4kuprg64gyz88qewg) 


## 1. Hướng dẫn cài đặt kỹ thuật tham số

Trong quá trình tạo mẫu tin, tại bước “Tạo nội dung” có phần cài đặt kĩ thuật cho tham số.  

Mỗi tham số sẽ có các cài đặt kĩ thuật khác nhau, tùy vào nhu cầu của doanh nghiệp sẽ có cách cài đặt khác nhau. Tuy nhiên, người dùng cần lưu ý chọn đúng cài đặt kĩ thuật cho từng tham số và truyền đúng định dạng, độ dài ký tự vào param.  

**Ví dụ:**  

*   Doanh nghiệp chọn tham số <customer\_name> với cài kỹ thuật là Tên khách hàng (30) thì độ dài kí tự tối đa mà khách hàng truyền vào là 30 kí tự. 
*   Đối với các tham số liên quan đến thời gian (ngày/tháng/năm hoặc giờ:phút:giây), doanh nghiệp nên chọn đúng cài đặt kỹ thuật là thời gian.

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/cfa2338a95f8c9f98a4205bb9644f70c.png" />
</p>

_<p align="center">Tương ứng với từng tham số sẽ có các cài đặt kỹ thuật khác nhau</p>_


## 2. Các định dạng của tham số khi tạo mẫu tin

### a. Tham số trong nội dung chính

Dữ liệu khi truyền vào tham số được hệ thống cài đặt với một số định dạng nhất định. Đối với các tham số được truyền vào ở nội dung chính của template, **không cần thực hiện mã hóa,** mà có thể giữ nguyên dữ liệu gốc khi truyền vào [API để gửi ZNS](https://developers.zalo.me/docs/api/zalo-notification-service-api/gui-zns/gui-zns-post-5208).

<div class="table" align="center">
      <table>
<table><tbody><tr><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>#</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Nhãn tham số</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Tên tham số</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Cài đặt kỹ thuật</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Giới hạn ký tự</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Data type</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Dữ liệu truyền vào</strong></span></p></td></tr><tr><td><span style="background-color:transparent;">1</span></td><td><span style="background-color:transparent;">Tên khách hàng</span></td><td><span style="background-color:transparent;">customer_name</span></td><td><span style="background-color:transparent;">Tên khách hàng (30)</span></td><td><span style="background-color:transparent;">30</span></td><td><span style="background-color:transparent;">string</span></td><td><span style="background-color:transparent;">Nguyễn Văn A</span></td></tr><tr><td><span style="background-color:transparent;">2</span></td><td><span style="background-color:transparent;">Điện thoại</span></td><td>phone_number</td><td><span style="background-color:transparent;">Số điện thoại (15)</span></td><td>15</td><td>string</td><td><span style="background-color:transparent;">096987453x</span></td></tr><tr><td><span style="background-color:transparent;">3</span></td><td>Địa chỉ</td><td>address&nbsp;</td><td>Địa chỉ (80)</td><td>80</td><td><span style="background-color:transparent;">string</span></td><td>104 Tạ Quang Bửu</td></tr><tr><td><span style="background-color:transparent;">4</span></td><td><span style="background-color:transparent;">Mã số</span></td><td><span style="background-color:transparent;">product_code</span></td><td><span style="background-color:transparent;">Mã số (30)</span></td><td><span style="background-color:transparent;">30</span></td><td><span style="background-color:transparent;">string</span></td><td><span style="background-color:transparent;">TP-34512</span></td></tr><tr><td><span style="background-color:transparent;">5</span></td><td><span style="background-color:transparent;">Nhãn tùy chỉnh</span></td><td><span style="background-color:transparent;">custom_field</span></td><td><span style="background-color:transparent;">Nhãn tùy chỉnh (30)</span></td><td><span style="background-color:transparent;">30</span></td><td><span style="background-color:transparent;">string</span></td><td><span style="background-color:transparent;">Mẫu nội dung tuỳ chỉnh</span></td></tr><tr><td><span style="background-color:transparent;">6</span></td><td><span style="background-color:transparent;">Trạng thái giao dịch</span></td><td><span style="background-color:transparent;">transaction_status</span></td><td><span style="background-color:transparent;">Trạng thái giao dịch (30)</span></td><td><span style="background-color:transparent;">30</span></td><td><span style="background-color:transparent;">string</span></td><td>Giao dịch thành công</td></tr><tr><td>7</td><td>Thông tin liên hệ&nbsp;</td><td>contact</td><td><span style="background-color:transparent;">Thông tin liên hệ (50)</span></td><td>50</td><td><span style="background-color:transparent;">string</span></td><td><span style="background-color:transparent;">096987453x</span></td></tr><tr><td>8</td><td><span style="background-color:transparent;">Giới tính / Danh xưng</span></td><td><span style="background-color:transparent;">personal_title</span></td><td><span style="background-color:transparent;">Giới tính / Danh xưng (5)</span></td><td><span style="background-color:transparent;">5</span></td><td><span style="background-color:transparent;">string</span></td><td><span style="background-color:transparent;">Chị</span></td></tr><tr><td>9</td><td><span style="background-color:transparent;">Tên sản phẩm, thương hiệu</span></td><td><span style="background-color:transparent;">product_name</span></td><td><span style="background-color:transparent;">Tên sản phẩm / Thương hiệu (100)</span></td><td><span style="background-color:transparent;">100</span></td><td><span style="background-color:transparent;">string</span></td><td><span style="background-color:transparent;">Bàn phím Razer</span></td></tr><tr><td>10</td><td><span style="background-color:transparent;">Số lượng / Số tiền</span></td><td><span style="background-color:transparent;">amount_vn_standard</span></td><td><span style="background-color:transparent;">Số lượng / Số tiền (20)</span></td><td><span style="background-color:transparent;">20</span></td><td>number</td><td><p><span style="background-color:transparent;">Nếu truyền định dạng dữ liệu số nguyên: 1000</span><br><span style="background-color:transparent;">Dữ liệu hiển thị: 1.000</span></p><p><span style="background-color:transparent;">Nếu truyền định dạng dữ liệu số thập phân: 0.3</span><br><span style="background-color:transparent;">Dữ liệu hiển thị: 0,3</span></p></td></tr><tr><td>11</td><td><span style="background-color:transparent;">Thời gian</span></td><td><span style="background-color:transparent;">time</span></td><td><span style="background-color:transparent;">Thời gian (20)</span></td><td><span style="background-color:transparent;">20</span></td><td><span style="background-color:transparent;">datetime</span></td><td><p><span style="background-color:transparent;">hh:mm:ss,&nbsp;</span><br><span style="background-color:transparent;">hh:mm,&nbsp;</span></p><p><span style="background-color:transparent;">hh:mm:ss dd/mm/yyyy,</span><br><span style="background-color:transparent;">hh:mm dd/mm/yyyy,</span></p><p>dd/mm/yyyy,<br><span style="background-color:transparent;">mm/yyyy&nbsp;</span></p></td></tr><tr><td>12</td><td>Bank Transfer Note</td><td>bank_transfer_note</td><td><span style="background-color:transparent;">Bank Transfer Note (90)</span></td><td>90</td><td>Bank Transfer Note</td><td>Không cho phép các ký tự đặc biệt @[]^_!"•#$%¥&amp;'()*+,€-./:;{|&lt;}=~&gt;?</td></tr></tbody></table>
</div>

_<p align="center">Xem thêm chi tiết các định dạng dữ liệu tại_ [_ĐÂY_](https://zalo.solutions/blog/cac-dinh-dang-du-lieu-khi-truyen-vao-tham-so-tren-noi-dung-zns/9gubbkay4yyrng86a)_._</p>


### b. Tham số tại nút thao tác

_\***Lưu ý**: **Doanh nghiệp nên mã hóa các tham số truyền vào ở đường liên kết CTA, không mã hóa toàn bộ đường liên kết sẽ ảnh hưởng đến chất lượng template và gây ra những lỗi khác.**_

### **CTA Đường dẫn liên kết** 

**Cần đảm bảo tất cả các yếu tố sau**:

*   Nên **mã hóa các dữ liệu truyền vào tham số** ở đường liên kết CTA, không mã hóa toàn bộ đường liên kết sẽ ảnh hưởng đến chất lượng template và gây ra những lỗi khác (không bắt buộc)
*   Các tham số trong CTA phải có tên khác với các tham số đã được định nghĩa trong phần nội dung chính & tiêu đề của Template.

Việc mã hóa dữ liệu truyền vào tham số sẽ giúp Zalo giải mã các tham số một cách chính xác và hoàn chỉnh liên kết mà Doanh nghiệp đã sử dụng để tạo mẫu ZNS. 

VD: Dữ liệu cần truyền vào tham số tại nút thao  là “Nguyễn Văn A”, dữ liệu truyền vào cần được mã hóa trước theo đúng chuẩn UTF-8 như sau:

<div class="table" align="center">
      <table>
<table><tbody><tr><td><span style="background-color:transparent;">#</span></td><td><span style="background-color:transparent;">Nhãn tham số</span></td><td><span style="background-color:transparent;">Tên tham số</span></td><td><span style="background-color:transparent;">Cài đặt kỹ thuật</span></td><td><span style="background-color:transparent;">Data type</span></td><td><span style="background-color:transparent;">Dữ liệu truyền vào</span></td><td><span style="background-color:transparent;">Dữ liệu hiển thị</span></td></tr><tr><td><span style="background-color:transparent;">1</span></td><td><span style="background-color:transparent;">URL</span></td><td><span style="background-color:transparent;">customer_name</span></td><td><span style="background-color:transparent;">URL (200)</span></td><td><span style="background-color:transparent;">string</span></td><td><span style="background-color:transparent;">Nguy%E1%BB%85n+V%C4%83n+A</span></td><td><span style="background-color:transparent;">Giữ nguyên</span></td></tr></tbody></table>
</div>

Sau khi định dạng các tham số, Liên kết (URL) truyền vào CTA sẽ có dạng là: https://example.com/param?customer\_name=<param1>&URL=<param2>

_<p align="center">Xem chi tiết hướng dẫn truyền tham số vào link CTA tại_ [_ĐÂY_](https://zalo.solutions/blog/cap-nhat-tinh-nang-zns-cho-phep-truyen-tham-so-param-vao-nut-thao-tac-cta-/6vuz4a47rd86q99mwd).</p>


## 3. Các định dạng dữ liệu khác

Dành cho các KH có templates được tạo qua yêu cầu đặc biệt. 

<div class="table" align="center">
      <table>
<table><tbody><tr><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>#</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Data type</strong></span></p></td><td><p style="text-align:center;"><span style="background-color:transparent;"><strong>Dữ liệu truyền vào</strong></span></p></td></tr><tr><td>1</td><td><span style="background-color:rgb(255,255,255);">Number</span></td><td><p style="margin-left:0px;">Cho phép ký tự số</p><p style="margin-left:0px;">Cho phép số dương, số âm và số thập phân (ngăn cách phần nguyên và phần thập phân bởi dấu ".")<br><br>123</p><p style="margin-left:0px;">100000</p><p style="margin-left:0px;">-100</p><p style="margin-left:0px;">-100.2</p></td></tr><tr><td>2</td><td><span style="background-color:rgb(255,255,255);">DateTime</span></td><td><p><span style="background-color:transparent;">Các format cho phép:</span><br><br><span style="background-color:transparent;">hh:mm:ss,&nbsp;</span><br><span style="background-color:transparent;">hh:mm,&nbsp;</span></p><p><span style="background-color:transparent;">hh:mm:ss dd/mm/yyyy,</span><br><span style="background-color:transparent;">hh:mm dd/mm/yyyy,</span></p><p>dd/mm/yyyy,<br><span style="background-color:transparent;">mm/yyyy&nbsp;</span></p></td></tr><tr><td>3</td><td>Currency</td><td><p style="margin-left:0px;">Chỉ cho phép các ký tự số 0 → 9</p><p style="margin-left:0px;">Chỉ cho phép số dượng</p></td></tr><tr><td>4</td><td><p style="margin-left:0px;">QR code</p></td><td><p style="margin-left:0px;">Cho phép các ký tự trong bảng mã ascii:</p><ul style="list-style-type:disc;"><li>Chữ cái</li><li>Số</li><li>Các ký tự đặc biệt: @, #, $,%, &amp;, *, +, -,...</li></ul></td></tr><tr><td>5</td><td><p style="margin-left:0px;">Bank Transfer Note</p></td><td>Không cho phép truyền các ký tự đặc biệt trên bàn phím di động, bao gồm: @[]^_!"•#$%¥&amp;'()*+,€-./:;{|&lt;}=~&gt;?</td></tr><tr><td>6</td><td><p style="margin-left:0px;">BIN Code</p></td><td>Mã 6 số theo bảng BIN Code <a target="_blank" rel="noopener noreferrer" href="https://zalo.cloud/news/cap-nhat-moi-zns-yeu-cau-thanh-toan-payment-request/qbu7mzk8yr8njzzav6">tại đây</a>.</td></tr></tbody></table>
</div>


## 4. Hướng dẫn xử lý mã lỗi liên quan thường gặp

Xem thêm chi tiết và hướng dẫn xử lý các mã lỗi tại [ĐÂY](https://zalo.solutions/zns/guidelines/handle-error-code). 
 

_Nếu có bất kì yêu cầu hỗ trợ, Quý khách có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của chúng tôi qua **Biểu Mẫu: [Mẫu hỗ trợ Zalo Business Solutions](https://zalo-solutions.freshdesk.com/en/support/tickets/new)**. Chúng tôi sẽ phản hồi Quý khách trong vòng 24h làm việc tiếp theo._
