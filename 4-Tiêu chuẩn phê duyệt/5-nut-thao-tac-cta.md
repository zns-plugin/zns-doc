---
id: nut-thao-tac-cta
title: Nút thao tác CTA trong mẫu thông báo ZNS
slug: /nut-thao-tac-cta
---

# <p align ="center">Nút thao tác CTA trong mẫu thông báo ZNS</p>

Nhằm hỗ trợ khách hàng khai thác tối đa nội dung/mục đích và tối ưu hóa dịch vụ Zalo Notification Service (ZNS), Zalo Business Solutions giới thiệu nút thao tác (CTA) trong nội dung thông báo ZNS. Bài viết này sẽ hướng dẫn quý khách triển khai tính năng này hiệu quả nhất. 

## 1. Giới thiệu về nút thao tác CTA:

*   Nút thao tác (CTA – Call to Action) là nút gắn kèm trong nội dung mẫu thông báo ZNS, cho phép người nhận click để thực hiện các thao tác bao gồm:
*   Gọi điện liên hệ số điện thoại được doanh nghiệp cung cấp
*   Truy cập đường dẫn (link) được doanh nghiệp cung cấp
*   Nội dung nút thao tác có thể được tùy chỉnh tùy theo nhu cầu sử dụng của doanh nghiệp. Với mỗi mẫu ZNS, bạn có thể thêm tối đa 2 nút thao tác (nút chính và nút phụ).


## 2. Danh sách các loại Nút thao tác CTA:

Xem thêm tại [**BẢNG GIÁ ZNS**](https://zalo.cloud/zns/pricing).


## 3. Hướng dẫn thêm nút thao tác CTA vào mẫu tin ZNS:

**Bước 1**. Click **“Nút thao tác”**.

![](https://stc-oa.zdn.vn/uploads/63c38797cc26e1e48e08182bfec28a6b.png)


**Bước 2**. Chọn loại nút thao tác theo nhu cầu, tạo đường dẫn liên kết/số điện thoại mới hoặc chọn từ dữ liệu được lưu từ các mẫu tin trước.

  ![](https://content.zalo.cloud/uploads/image_fa118fa78b.png)![](https://stc-oa.zdn.vn/uploads/dfbde94e34e21269e42b7106e4a773bf.png)


**Bước 3.** Thêm nút thao tác thứ 2 theo nhu cầu, lặp lại các bước trước. 


## 4. Hướng dẫn thêm nút thao tác CTA vào mẫu tin ZNS:

Để có thể hỗ trợ doanh nghiệp cá nhân hóa (customize) đường dẫn gửi cho từng người dùng, Zalo Business Solutions chính thức mở tích hợp khả năng truyền tham số (param) vào nút thao tác (CTA) khi tạo mẫu ZNS. Tính năng này phù hợp cho nhiều doanh nghiệp thuộc nhiều ngành hàng với các nhu cầu tiêu biểu bao gồm nhưng không giới hạn như: 

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

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của chúng tôi qua **Biểu Mẫu: [Mẫu hỗ trợ Zalo Business Solutions](https://go.zalo.me/SupportZBS )**. Đội ngũ CSKH Zalo Business Solutions sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._

_**Lưu ý:**_ _Từ 06/08/2025, **Zalo Cloud** chính thức đổi tên thành **Zalo Business Solutions.** Việc ra mắt thương hiệu Zalo Business Solutions (ZBS) là sự thay đổi về mặt nhận diện thương hiệu, không làm thay đổi về mặt pháp lý đối với các hoạt động, giao dịch và cam kết đã có trước đây dưới tên gọi Zalo Cloud._
