---
id: cach-su-dung-va-ung-dung-cua-mau-xac-thuc
title: Cách sử dụng và ứng dụng của Mẫu Xác thực
slug: /cach-su-dung-va-ung-dung-cua-mau-xac-thuc
---
     **1. Mẫu Xác thực là gì? Cách ứng dụng Mẫu Xác thực:**

Mẫu Xác thực là mã xác thực một lần được gửi đến người dùng Zalo thông qua dịch vụ Tin nhắn ZBS Template. Với mục đích xác nhận đăng nhập các ứng dụng online, thông báo về quá trình tạo hoặc thay đổi trạng thái người dùng (gửi mã xác thực cho khách hàng tạo tài khoản mới, xác nhận đổi mật khẩu, xác thực tài khoản, xác thực giao dịch,…)

![](https://stc-oa.zdn.vn/uploads/bc9ff84938b6177ec056ad11aabbd7f2.png)

     **2. Cấu trúc của một Mẫu Xác thực:** 

Doanh nghiệp sử dụng Mẫu Xác thực mặc định trên tài khoản ZBS và cấu trúc mặc định của 1 Mẫu Xác thực bao gồm:

*   Logo OA
*   Thông tin “Mã xác thực của bạn là <otp>”

Doanh nghiệp có thể sao chép mã xác thực từ tin nhắn ZBS Template. Thông tin chi tiết về tính năng sao chép mã xác thực, xem tại [ĐÂY](https://zalo.solutions/blog/cap-nhat-kha-nang-sao-chep-doi-voi-mau-zns-xac-thuc/a73khxv3py264sshlwkhnm0l)

Bên cạnh những nội dung mặc định, doanh nghiệp cũng có thể chỉnh sửa nội dung gửi kèm mã xác thực.

<table><tbody><tr><td><p style="margin-left:0px;">&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;"><strong>Phần cố định của hệ thống</strong><span style="color:rgb(0,120,212);">&nbsp;</span></p></td><td><p style="margin-left:0px;text-align:center;"><strong>Phần có thể chỉnh sửa theo nhu cầu sử dụng</strong><span style="color:rgb(0,120,212);">&nbsp;</span></p></td></tr><tr><td><p style="margin-left:0px;text-align:center;"><strong>Logo đăng ký</strong><span style="color:rgb(0,120,212);">&nbsp;</span></p><p style="margin-left:0px;"><img class="image_resized" style="width:243px;" src="https://stc-oa.zdn.vn/uploads/c12c01a6a2ae55ce0fc01486e4648c0c.png">&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;"><img class="image_resized" style="width:44px;" src="https://stc-oa.zdn.vn/uploads/48dca6d085589412dc674bdacab21356.png">&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;"><img class="image_resized" style="width:46px;" src="https://stc-oa.zdn.vn/uploads/aff4f9e3fc3b3dc2b53bd35fe0fdcf9b.png">&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;text-align:center;"><strong>Nội dung:</strong><span style="color:rgb(0,120,212);">&nbsp;</span></p><p style="margin-left:0px;">Mã xác thực của bạn là&nbsp;</p><p style="margin-left:0px;">&lt;otp&gt;&nbsp;</p><p style="margin-left:0px;"><img class="image_resized" style="width:243px;" src="https://stc-oa.zdn.vn/uploads/7bbd4cb6d07beb06026b99abedd2961e.png">&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;"><img class="image_resized" style="width:46px;" src="https://stc-oa.zdn.vn/uploads/9e596c24460ba39c0d93c59f7449b8ed.png">&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;"><img class="image_resized" style="width:44px;" src="https://stc-oa.zdn.vn/uploads/178e3d805c9a0fd9c5ad95e4efafa1c3.png">&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;text-align:center;"><strong>Nội dung gửi kèm mã xác thực:</strong><span style="color:rgb(0,120,212);">&nbsp;</span></p><p style="margin-left:0px;text-align:center;">&nbsp;<br><img class="image_resized" style="width:243px;" src="https://stc-oa.zdn.vn/uploads/fd570f0d04e02aed9563b0edeccfe8c5.png">&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;"><img class="image_resized" style="width:44px;" src="https://stc-oa.zdn.vn/uploads/ccfa2437879f54b0a323eaed34da4e3c.png">&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;"><img class="image_resized" style="width:46px;" src="https://stc-oa.zdn.vn/uploads/f58ad0f0d4a2c61d7042197cbebe6e79.png">&nbsp;</p></td></tr></tbody></table>

**Lưu ý:** Mẫu Xác thực không hỗ trợ sử dụng nút CTA. Trong trường hợp xác thực tài khoản, doanh nghiệp có thể ngoại lệ gửi thông báo đến khách hàng chưa phát sinh giao dịch với OA.  

![](https://stc-oa.zdn.vn/uploads/0fda1184d57035a621a484d173c4f1ab.png)

_(Hình ảnh minh hoạ mẫu tin ZNS Xác thực ở cả 2 giao diện sáng và tối)_ 

     **3. Hướng dẫn tạo Mẫu Xác thực trên trang tài khoản ZBS**

**Xem thêm:** [**Các bước thiết lập ban đầu để gửi Tin nhắn ZBS Template**](https://zalo.solutions/zns/guidelines/intro)

_**Bước 1:**_ Truy cập vào trang tài khoản [**ZBS**](https://account.zalo.solutions/spending/overview) và chọn **“Dịch vụ gửi tin”** 

![image.png](https://content.zalo.cloud/uploads/image_6b19809fb1.png)

_**Bước 2:**_ Tại trang [**“Dịch vụ gửi tin”**](https://account.zalo.solutions/9GUDMAJZZREQ9MZP/tool/zns/manage/template), chọn [**“Tạo Template”**](https://account.zalo.solutions/tool/zns/createTemplate)

![image.png](https://content.zalo.cloud/uploads/image_2ca3803ef1.png)

_**Bước 3:**_ Thiết lập các thông tin chung 

Nhập tên mẫu, chọn OA và Ứng dụng (AppID) để

![image.png](https://content.zalo.cloud/uploads/image_405fd7c205.png)

_**Bước 4:**_ Tại trang **“Khai báo nội dung”**, chọn loại Template **“Mẫu Xác thực”**. Sau đó, thao tác tải logo lên và điều chỉnh **“Nội dung gửi kèm mã OTP”** phù hợp với nhu cầu sử dụng rồi nhấn **“Tiếp tục”**. 

![image.png](https://content.zalo.cloud/uploads/image_7c2424bd87.png)

_**Bước 5:**_ Nhập nội dung truyền vào tham số, tick vào mục **“đồng ý với Điều khoản và Chính sách sử dụng của Zalo Business Solutions”** rồi nhấn **“Hoàn thành”**. 

![image.png](https://content.zalo.cloud/uploads/image_bf002a8eec.png)

_Nếu có bất kì yêu cầu hỗ trợ, Quý khách có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của chúng tôi qua Biểu Mẫu:_ [_Mẫu hỗ trợ Zalo Business Solutions_](https://zalocloud.freshdesk.com/en/support/tickets/new)_. Chúng tôi sẽ phản hồi Quý khách trong vòng 24h làm việc tiếp theo._
