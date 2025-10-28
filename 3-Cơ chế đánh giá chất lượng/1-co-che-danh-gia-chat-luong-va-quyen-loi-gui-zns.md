---
id: co-che-danh-gia-chat-luong-va-quyen-loi-gui-zns
title: Cơ chế đánh giá chất lượng và quyền lợi gửi ZNS
slug: /coi-che-danh-gia-chat-luong-va-quyen-loi-gui-zns
---

# <p align="center">Cơ chế đánh giá chất lượng và quyền lợi gửi thông báo ZNS</p>


Trong hoạt động gửi thông báo chăm sóc khách hàng qua Zalo, tỷ lệ báo xấu (phản hồi tiêu cực) của người nhận thông báo Zalo Notification Services sẽ ảnh hưởng đến quyền lợi của doanh nghiệp vì liên quan trực tiếp đến số lượng ZNS gửi mỗi ngày cũng như loại nội dung thông báo có thể gửi. Để có thể nắm các thông tin về cơ chế đánh giá chất lượng và quyền lợi gửi ZNS từ Zalo Business Solutions chính xác nhất, quý doanh nghiệp vui lòng tham khảo bài viết sau đây.


## A. Quyền lợi gửi ZNS của OA 

### **A.1 - Số lượng ZNS có thể gửi mỗi ngày (Daily quota)**

**Từ 0H ngày 12/03/2024:** Quyền lợi gửi ZNS của OA sẽ được thể hiện theo từng mốc của chỉ số **“Số lượng ZNS có thể gửi mỗi ngày (Daily quota)”** , mỗi mốc sẽ có quyền lợi tương ứng như bảng bên dưới

<div class="table" align="center">
      <table>
<table><tbody><tr><td><p style="margin-left:0px;text-align:center;"><strong>Mốc</strong></p><p style="margin-left:0px;text-align:center;"><strong>(= Daily quota)&nbsp;</strong></p></td><td><p style="margin-left:0px;text-align:center;"><strong>Quyền lợi về các mục đích (Tag) được gửi</strong></p></td><td><p style="margin-left:0px;text-align:center;"><strong>Mô&nbsp;tả&nbsp;</strong></p></td></tr><tr><td><p style="margin-left:0px;">500&nbsp;</p></td><td colspan="1" rowspan="4"><p>Tag 1 - Giao dịch (Transaction)</p><p>Tag 2 - Chăm sóc khách hàng (Customer Care)</p></td><td colspan="1" rowspan="2"><p style="margin-left:0px;">Vùng&nbsp;phạt với những OA bị hạ mốc dưới mốc mặc định</p></td></tr><tr><td><p style="margin-left:0px;">2,000&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;"><span style="background-color:hsl(60,75%,60%);"><strong>5,000&nbsp;</strong></span></p></td><td><p style="margin-left:0px;"><span style="background-color:hsl(60,75%,60%);"><strong>Điểm&nbsp;bắt&nbsp;đầu&nbsp;mặc&nbsp;định</strong></span><br><i>(OA mới được khởi tạo mặc định nằm ở mốc này)&nbsp;</i></p></td></tr><tr><td><p style="margin-left:0px;">10,000&nbsp;</p></td><td><p style="margin-left:0px;">&nbsp;-</p></td></tr><tr><td><p style="margin-left:0px;"><span style="background-color:hsl(90,75%,60%);"><strong>20,000</strong>&nbsp;</span></p></td><td colspan="1" rowspan="4"><p>Tag 1 - Giao dịch (Transaction)</p><p>Tag 2 - Chăm sóc khách hàng (Customer Care)</p><p><span style="background-color:hsl(90,75%,60%);"><strong>Tag 3 - Hậu mãi (Promotion)</strong></span></p></td><td><p style="margin-left:0px;"><span style="background-color:hsl(90,75%,60%);"><strong>Điểm&nbsp;Mở&nbsp;quyền&nbsp;gửi&nbsp;tin (Tag Hậu mãi)&nbsp;</strong></span></p></td></tr><tr><td><p style="margin-left:0px;">50,000&nbsp;</p></td><td><p style="margin-left:0px;">&nbsp;-</p></td></tr><tr><td><p style="margin-left:0px;">100,000&nbsp;</p></td><td><p style="margin-left:0px;">&nbsp;-</p></td></tr><tr><td><p style="margin-left:0px;">500,000&nbsp;</p></td><td><p style="margin-left:0px;">&nbsp;-</p></td></tr></tbody></table>
</table>
</div>

_<p align="center">Xem thêm [Quy định chung khi kiểm duyệt mẫu ZNS](https://zalo.cloud/news/quy-dinh-chung-khi-kiem-duyet-mau-tin-zns/baujzpyvjjrz7776m).</p>_


### A.2 - Cơ chế gửi và nhận ZNS template tag Hậu mãi

<div class="table" align="center">
   <table>
<table><tbody><tr><td><p style="margin-left:0px;text-align:center;"><strong>Phân loại</strong></p></td><td><p style="margin-left:0px;text-align:center;"><strong>Chi tiết cơ chế</strong></p></td><td><p style="text-align:center;"><strong>Diễn giải, ví dụ,…</strong></p></td></tr><tr><td><strong>Hạn mức nhận ZNS tag Hậu mãi của User mỗi tháng</strong></td><td><p style="margin-left:0px;text-align:center;">Mỗi đối tượng nhận tin (user) nhận <strong>tối đa </strong><span style="background-color:hsl(60,75%,60%);"><strong>4</strong></span><strong> ZNS tag Hậu mãi/tháng</strong> từ 1 OA</p></td><td><p>User A có SĐT 0123456789:</p><ul><li>User A nhận <u>tối đa 4</u> ZNS tag Hậu mãi mỗi tháng từ OA Brand name X</li><li>User A nhận <u>tối đa 4</u> ZNS tag Hậu mãi mỗi tháng từ OA Ngân hàng Y</li><li>Số lượng ZNS tag Giao dịch và Chăm sóc khách hàng mà user A có thể nhận mỗi tháng từ cả 2 OA X và OA Y là không giới hạn</li></ul></td></tr><tr><td><strong>Điều kiện nhận ZNS tag Hậu mãi của User</strong></td><td>OA chỉ có thể gửi ZNS tag Hậu mãi cho <strong>user đã từng nhận</strong> ZNS tag Giao dịch (tag 1) <u>hoặc</u> tag Chăm sóc sách hàng (tag 2) từ OA trong 6 tháng gần nhất</p><p><span style="font-size:12px;"><i><u>Ghi chú: </u>Nếu OA chưa gửi ZNS tag 1 hoặc tag 2 cho user nhưng gửi tag 3, hệ thống tự động trả mã lỗi -140 (xem thêm tại </i></span><a target="_blank" rel="noopener noreferrer" href="https://developers.zalo.me/docs/zalo-notification-service/phu-luc/bang-ma-loi"><span style="font-size:12px;"><i>Bảng mã lỗi ZNS</i></span></a><span style="font-size:12px;"><i>)</i></span></p></td><td><p>Một OA có các tệp người dùng (user) sau:</p><ul><li>User A đã nhận 1 ZNS tag giao dịch từ OA</li><li>User B đã nhận 1 ZNS tag giao dịch từ OA</li><li>User C chưa từng nhận bất kì ZNS tag giao dịch/chăm sóc khách hàng nào từ OA</li><li>User D chưa từng nhận bất kì ZNS nào từ OA</li></ul><p>=&gt; OA có thể gửi ZNS tag Hậu mãi cho user A + B; không thể gửi ZNS tag Hậu mãi cho user C + D</p></td></tr><tr><td><strong>Hạn mức gửi ZNS hậu mãi của OA theo tháng (Promotion Quota)</strong><br><span style="background-color:hsl(60,75%,60%);"><strong>(Áp dụng từ 01/11/2024)</strong></span></td><td><strong>Promotion Quota = 1/6 * (Tổng số ZNS Giao dịch và ZNS CSKH đã gửi thành công trong hai tháng trước đó)</strong><br><br>Promotion Quota sẽ được điều chỉnh theo công thức trên vào ngày đầu tiên của mỗi tháng</td><td><p>OA Brand name A có daily quota ở mốc 50,000</p><ul><li>Tháng 9: OA đã gửi thành công <strong>tổng 10,000 ZNS Giao dịch và CSKH</strong></li><li>Tháng 10: OA đã gửi thành công <strong>tổng 50,000 ZNS Giao dịch và CSKH</strong></li></ul><p>=&gt; Hạn mức ZNS hậu mãi tối đa trong tháng 11 của A được tính theo công thức là:&nbsp;<strong>Promotion Quota = 1/6 * (10,000+50,000) = 10,000</strong>&nbsp;<br>=&gt; A có thể gửi tối đa 10,000 ZNS hậu mãi trong tháng 11.</p></td></tr></tbody></table>
</div>

Với mục đích tối ưu hóa sản phẩm và mang đến trải nghiệm tốt hơn cho người dùng cuối, **từ 0H ngày 01/11/2024**, cơ chế đánh giá chất lượng và quyền lợi gửi tin dịch vụ ZNS sẽ có những điều chỉnh sau: 

*   **Bổ sung chỉ số "Hạn mức gửi ZNS hậu mãi của OA theo tháng" - Promotion Quota** (bỏ “Hạn mức gửi ZNS Hậu mãi của OA mỗi ngày”)  
    **Công thức tính Promotion Quota = 1/6 \* (Tổng số ZNS Giao dịch và ZNS CSKH đã gửi thành công trong hai tháng trước đó)**
*   Khi OA lần đầu tiên được gửi ZNS hậu mãi, mức Promotion Quota của tháng đó sẽ tự động được tăng thêm 10,000.
*   Promotion Quota sẽ được điều chỉnh theo công thức trên vào ngày đầu tiên của mỗi tháng  
     

## B. Chất lượng gửi ZNS của Zalo Official Account (OA)

### B.1 - Cơ chế đánh giá chất lượng - xét duyệt tăng/giảm hạn mức

Chất lượng gửi ZNS của OA sẽ được chia làm 3 mức độ, ứng với các quyền lợi như sau:

<div class="table" align="center">
   <table>
<table><tbody><tr><td><p style="margin-left:0px;text-align:center;"><strong>Mức độ&nbsp;</strong></p></td><td><p style="margin-left:0px;text-align:center;"><strong>Tỷ lệ báo xấu của người nhận với ZNS đã gửi&nbsp;</strong></p></td><td><p style="margin-left:0px;text-align:center;"><strong>Quy định về quyền lợi&nbsp;</strong></p></td></tr><tr><td><p style="margin-left:0px;text-align:center;"><strong>Tốt</strong>&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;">Nhỏ hơn hoặc bằng mức tiêu chuẩn của hệ thống.&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;">Được xét duyệt tăng quyền lợi.&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;text-align:center;"><strong>Trung bình</strong>&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;">Cao hơn mức tiêu chuẩn nhưng vẫn nằm trong mức giới hạn cho phép.&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;">Giữ nguyên quyền lợi cho đến khi chất lượng được cải thiện. Nếu duy trì thời gian dài ở mức này có thể dẫn đến việc giảm quyền lợi.&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;text-align:center;"><strong>Kém</strong>&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;">Vượt mức giới hạn cho phép.&nbsp;</p></td><td><p style="margin-left:0px;text-align:center;">Giảm quyền lợi. Ngoài ra, các mẫu ZNS ở mức kém sẽ bị vô hiệu hoá.&nbsp;</p></td></tr></tbody></table>
</div>

Khởi đầu, Zalo OA của doanh nghiệp sẽ chỉ được gửi các mẫu thông báo ZNS có cấp độ thấp. Sau đó, dựa theo chất lượng gửi ZNS, hệ thống sẽ tự động điều chỉnh cho phép OA gửi các loại nội dung ở cấp độ cao hơn: 

<div class="table" align="center">
<table><tbody><tr><td><p style="text-align:center;"><strong>Cơ chế tăng/giảm hạn mức</strong></p></td><td><p style="text-align:center;"><strong>Điều kiện</strong></p></td></tr><tr><td>Tăng 1 hạn mức</td><td><p style="text-align:center;">Chất lượng gửi ZNS trong 7 ngày gần nhất ở mức <strong>Tốt.</strong> &nbsp;(= <span style="color:#538135;"><strong>High)</strong></span></p><p style="text-align:center;"><strong>VÀ / AND</strong></p><p style="text-align:center;">Số lượng tin đã gửi thành công trong 7 ngày gần nhất <strong>= 2 x [Daily quota hiện tại của OA]</strong></p></td></tr><tr><td>Giảm 1 hạn mức</td><td>Chất lượng gửi ZNS trong 7 ngày gần nhất ở mức <strong>Kém</strong> (= <span style="color:#C00000;"><strong>Low)</strong></span></td></tr></tbody></table>
</div>

**Lưu ý đặc biệt:** 

*   Quyền lợi gửi ZNS của OA sẽ được đánh giá **mỗi ngày** _(trừ giai đoạn chờ sau khi thay đổi hạn mức)_.
    *   Khi có sự thay đổi về hạn mức quyền lợi (tăng hoặc giảm hạn mức/cấp độ gửi tin tối đa), sẽ áp dụng thời gian chờ cho lần đánh giá để xét duyệt thay đổi quyền lợi kế tiếp.
    *   Thời gian chờ kéo dài 7 ngày, từ ngày OA có sự thay đổi về hạn mức quyền lợi.
    *   Đây là khoảng thời gian vừa đủ để đội ngũ hỗ trợ khách hàng và phát triển sản phẩm của Zalo có thể đánh giá chính xác về khả năng gửi ZNS của doanh nghiệp tại hạn mức quyền lợi mới.
    *   Với OA chưa có lịch sử sử dụng dịch vụ ZNS, việc gửi ZNS đầu tiên vào ngày D sẽ kích hoạt cơ chế đánh giá chất lượng từ D+1, đợt đánh giá đầu tiên sẽ thực hiện sau thời gian chờ (7 ngày) vào ngày D+8.
*   Nếu chất lượng gửi ZNS của OA thường xuyên ở mức **Kém**, bên cạnh việc giảm quyền lợi gửi, Zalo có thể đưa ra quyết định tạm ngừng cung cấp dịch vụ ZNS cho doanh nghiệp cho đến khi doanh nghiệp cam kết cải thiện chất lượng gửi thông báo.
*   Chất lượng của OA được xác định bởi Tỉ lệ báo xấu trong khoảng thời gian đánh giá chất lượng tương ứng.
    *   Tỉ lệ báo xấu an toàn mỗi ngày được đề xuất là <0.1% để không bị giảm Chất lượng của OA
    *   Xem thêm: [Báo xấu mẫu thông báo ZNS được ghi nhận khi nào](https://zalo.cloud/blog/bao-xau-mau-tin-thong-bao-zns-duoc-ghi-nhan-khi-nao/yku9nm97wyd7nm8aab)
*   Các template ID có tỉ lệ báo xấu được hệ thống đánh giá là vượt mức báo xấu và mức độ báo xấu cho phép sẽ tự động bị khóa (disabled) để đảm bảo trải nghiệm của người dùng.
    *   Việc khóa các template này diễn ra độc lập với việc xác định Chất lượng OA.


### B.2 - Cơ chế xử lý vi phạm (penalty) tự động

Với mục đích giảm thiểu rủi ro ảnh hưởng đến trải nghiệm của user trong các trường hợp tỉ lệ báo xấu (report) của OA tăng cao đột ngột trong thời gian ngắn, hệ thống sẽ có cơ chế phạt (penalty) với các trường hợp này.

***Điều kiện: Khi \[Tổng số lượng report trong ngày\] > \[2% x Daily quota hiện tại của OA\]***

**Action: OA sẽ bị hạ 1 mức daily quota (diễn ra tối đa 1 lần/ngày)**

**Chi tiết:**

*   **Hoạt động song song với cơ chế tăng/giảm hạn mức daily quota (Cơ chế ở mục B.1).​**
*   Không bị ảnh hưởng bởi thời gian chờ 7 ngày sau khi tăng/giảm hạn mức.​
*   Trong khoảng thời gian 00:00 – 24:00 mỗi ngày, cơ chế penalty diễn ra tối đa 1 lần.​
*   Tần suất đánh giá: Mỗi giờ.​
*   Khung thời gian đánh giá: từ đầu ngày đến thời điểm hiện tại.


## C. Hướng dẫn xem báo cáo chất lượng gửi ZNS trên tài khoản ZCA


Khi bắt đầu hoạt động gửi thông báo ZNS, Zalo Official Account (OA) của doanh nghiệp sẽ chỉ được gửi ZNS có cấp độ thấp. Sau đó, dựa theo chất lượng gửi ZNS, hệ thống sẽ tự động điều chỉnh cho phép OA gửi các loại nội dung ở cấp độ cao hơn. 

Xem thêm [Hướng dẫn xem báo cáo chất lượng gửi ZNS trên tài khoản ZCA](https://zalo.cloud/blog/huong-dan-xem-bao-cao-chat-luong-gui-zns-tren-tai-khoan-zca-/baudd7d9nmvjd9pjav).


## D. Truy xuất thông tin chất lượng và quyền lợi gửi ZNS qua API

Những thông tin về chất lượng và quyền lợi gửi ZNS của OA có thể được truy xuất qua các API như sau: 

<div class="table" align="center">
   <table>
<table><tbody><tr><td><p style="margin-left:0px;"><strong>Thông tin&nbsp;</strong></p></td><td><p style="margin-left:0px;"><strong>API&nbsp;</strong></p></td></tr><tr><td><p style="margin-left:0px;">Số lượng thông báo ZNS có thể gửi mỗi ngày&nbsp;</p></td><td><p style="margin-left:0px;"><a target="_blank" rel="noopener noreferrer" href="https://developers.zalo.me/docs/api/zalo-notification-service-api/truy-xuat-thong-tin/lay-thong-tin-quota-thong-bao-zns-post-5229"><span style="color:rgb(5,99,193);"><u>Lấy thông tin quota thông báo ZNS</u></span></a>&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;">Loại nội dung ZNS có thể gửi&nbsp;</p></td><td><p style="margin-left:0px;"><a target="_blank" rel="noopener noreferrer" href="https://developers.zalo.me/docs/api/zalo-notification-service-api/truy-xuat-thong-tin/lay-thong-tin-loai-noi-dung-zns-duoc-phep-gui-post-5227"><span style="color:rgb(5,99,193);"><u>Lấy thông tin loại nội dung ZNS được phép gửi</u></span></a>&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;">Chất lượng gửi &nbsp;thông báo ZNS của OA&nbsp;</p></td><td><p style="margin-left:0px;"><a target="_blank" rel="noopener noreferrer" href="https://developers.zalo.me/docs/api/zalo-notification-service-api/truy-xuat-thong-tin/lay-thong-tin-chat-luong-gui-zns-hien-tai-cua-oa-post-5214"><span style="color:rgb(5,99,193);"><u>Lấy thông tin chất lượng gửi ZNS hiện tại của OA</u></span></a>&nbsp;</p></td></tr><tr><td><p style="margin-left:0px;">Chất lượng gửi ZNS của mẫu thong báo (template) ZNS cụ thể&nbsp;</p></td><td><p style="margin-left:0px;"><a target="_blank" rel="noopener noreferrer" href="https://developers.zalo.me/docs/api/zalo-notification-service-api/truy-xuat-thong-tin/lay-thong-tin-chi-tiet-template-post-5222"><span style="color:rgb(5,99,193);"><u>Lấy thông tin chi tiết template</u></span></a>&nbsp;</p></td></tr></tbody></table>
</div>

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của chúng tôi qua **Biểu Mẫu: [Mẫu hỗ trợ Zalo Business Solutions](https://go.zalo.me/SupportZBS )**_. Đội ngũ CSKH Zalo Business Solutions sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._

_**Lưu ý:**_ _Từ 06/08/2025, **Zalo Cloud** chính thức đổi tên thành **Zalo Business Solutions.** Việc ra mắt thương hiệu Zalo Business Solutions (ZBS) là sự thay đổi về mặt nhận diện thương hiệu, không làm thay đổi về mặt pháp lý đối với các hoạt động, giao dịch và cam kết đã có trước đây dưới tên gọi Zalo Cloud._
