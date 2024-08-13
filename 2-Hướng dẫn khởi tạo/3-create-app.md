---
id: create-app
title: Hướng dẫn khởi tạo Ứng dụng
slug: /create-app
---

## Giới thiệu Ứng dụng (App)

**Ứng dụng (App)** là đơn vị đại diện của Doanh nghiệp (OA) để thực hiện
gửi thông báo ZNS đến khách hàng. Sau khi có tài khoản Zalo Cloud
Account (ZCA), doanh nghiệp có thể tạo Ứng dụngđể truy cập các API được
cung cấp bởi Zalo.

**Lưu ý**: Trong trường hợp doanh nghiệp chưa có tài khoản ZCA, vui lòng
tham khảo bài viết <ins>[tại
đây](https://zalo.cloud/blog/zca-la-gi-huong-dan-dang-ky-tai-khoan-zca/gnuv4gqnejdddvg4m)</ins>
để đăng ký tài khoản.

## Các bước khởi tạo ứng dụng

### Bước 1: Tạo ứng dụng mới

Truy cập trang <ins> [Tạo ứng dụng
mới](https://developers.zalo.me/createapp)</ins> → Điền đầy đủ
các thông tin: Tên hiển thị, Danh mục, Mô tả và chọn "Tôi không phải là
người máy" → "Tạo ID ứng dụng".

![alt_text](https://stc-oa.zdn.vn/uploads/2023/06/13/92df837e93127fae7d89b6dcaa0e6851.png "image create app id")

### Bước 2: Điền thông tin ứng dụng

Sau khi Tạo ứng dụng thành công. Doanh nghiệp tiếp tục điền các thông
tin theo yêu cầu như: số điện thoại, email, biểu tượng (icon ứng dụng)
và miền ứng dụng (tùy chọn) để kích hoạt ứng dụng.

![alt_text](https://stc-oa.zdn.vn/uploads/2023/06/13/4f443e910650fbd72424f64e022f3551.png "image fill app info")

### Bước 3: Kích hoạt ứng dụng

Doanh nghiệp tiến hành **kích hoạt ứng dụng** để có thể gửi thông báo
ZNS đến người dùng thông qua các API được cung cấp bởi Zalo. Ứng dụng đã
được kích hoạt chỉ có thể sử dụng những API đã được xét duyệt.

![alt_text](https://stc-oa.zdn.vn/uploads/2023/06/13/8fc46ce4ebb3e97117606eafc138c856.png "image activate app")

![alt_text](https://stc-oa.zdn.vn/uploads/2023/06/13/2f44de20f2a5e129243ec3c020775d38.png "image activate app success")

### Bước 4: Liên kết ứng dụng với tài khoản ZCA

Để liên kết ứng dụng với tài khoản ZCA, tài khoản Doanh nghiệp cần phải
là Quản trị viên/Quản trị viên cao cấp của ZCA và đồng thời là Quản trị
viên của ứng dụng.

_Các bước liên kết vui lòng tham khảo chi tiết <ins> [tại
đây](https://zalo.cloud/blog/huong-dan-lien-ket-app-id-vao-tai-khoan-zalo-cloud-account-zca/vvurnnpbnqgn8dzbrv) </ins>_

![alt_text](https://stc-oa.zdn.vn/uploads/2023/06/13/9da02b7c78bb2d31151ebfe348b1edd6.png "image link ZCA")

## Hướng dẫn liên kết Ứng dụng và OA dùng để gửi thông báo ZNS

### Bước 1: Liên kết ứng dụng với OA

Truy cập trang [quản lý Ứng
dụng](https://developers.zalo.me/apps) và chọn Ứng dụng
tương ứng. Ở mục "Sản phẩm" chọn "Official Account" → "Quản lý Official
Account" → Chọn OA mà doanh nghiệp muốn liên kết → "Liên kết". Sau đó
chọn đồng ý với việc liên kết Ứng dụng.

![alt_text](https://stc-oa.zdn.vn/uploads/2023/06/13/7c34be81c52147848fff890e15098ed2.png "image link app-oa")

Zalo Notification Service (ZNS) là dịch vụ gửi thông báo chăm sóc khách
hàng qua API tới số điện thoại đang sử dụng Zalo. Vì vậy, doanh nghiệp
cần mua gói OA để tích hợp API và tiến hành gửi ZNS.

_Doanh nghiệp xem thêm thông tin về gói dịch vụ <ins> [tại
đây](https://oa.zalo.me/home/resources/policy/-trien-khai-goi-dich-vu-tra-phi-voi-zalo-oa-doanh-nghiep_4326077009372661188) </ins>_

### Bước 2: Yêu cầu cấp mã truy cập (Access Token) từ OA để gửi ZNS

Để sử dụng hệ thống ZNS API, ứng dụng cần được cấp quyền bằng cách lấy
access token từ OA, nếu không thực hiện bước này sẽ không thể chọn OA
trong quá trình tạo mẫu ZNS.

_Các bước yêu cầu cấp mới Access token vui lòng xem chi tiết <ins> [tại
đây](https://developers.zalo.me/docs/api/official-account-api/xac-thuc-va-uy-quyen/cach-2-xac-thuc-voi-cong-cu-api-explorer/phuong-thuc-lay-oa-access-token-su-dung-cong-cu-api-explorer-post-5004) </ins>_

![alt_text](https://stc-oa.zdn.vn/uploads/2023/06/13/42ad6181b5f0578b703b33558aa8148b.png "image provide AT")

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ
Chăm sóc khách hàng của Zalo Cloud qua email: **support@zalo.cloud**. Đội
ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc
tiếp theo._
