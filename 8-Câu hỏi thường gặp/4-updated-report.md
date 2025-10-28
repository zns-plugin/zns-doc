---
id: bao-xau-mau-thong-bao-zns-duoc-ghi-nhan-khi-nao
title: Báo xấu mẫu thông báo ZNS được ghi nhận khi nào?
slug: /bao-xau-mau-thong-bao-zns-duoc-ghi-nhan-khi-nao
---

# <p align="center">Báo xấu mẫu thông báo ZNS được ghi nhận khi nào?</p>

Để đảm bảo trải nghiệm của người dùng cuối (end-user), user có quyền lựa chọn báo xấu các mẫu thông báo Zalo Notification Service (ZNS) đã nhận để phản ánh chất lượng dịch vụ.

## 1. Cơ chế Báo xấu (Report):

- Các điều chỉnh áp dụng từ **07/01/2025**:

1.  **Thay Đổi Entry Point Báo Xấu:** người dùng có thể báo xấu thông qua 1 trong 2 cách sau:

    - Nút 3 chấm phía trên bên phải của mẫu thông báo ZNS
    - Bong bóng  **“Bạn cảm thấy phiền? Báo xấu”** bên dưới ZNS  
      (Bong bóng sẽ tồn tại trong 48 giờ từ lúc user nhận ZNS. Sau thời gian này, bong bóng sẽ biến mất.)

2.  **Hành động Báo xấu và ngừng nhận ZNS được xác định là hai hành động độc lập:**

    - Khi user báo xấu 1 ZNS từ OA Brand A, hệ thống sẽ **KHÔNG tự động** ngừng nhận ZNS từ OA này. Nếu user muốn ngừng nhận ZNS từ OA này, user có thể chủ động thao tác **“Ngừng nhận thông báo từ doanh nghiệp này”**.
    - Xem thêm tại phần 2 (bên dưới) Cơ chế ngừng nhận ZNS từ OA.  
      Nếu user chọn “Nội dung tin không hiển thị hoặc hiển thị lỗi” hoặc “Lý do khác” _**=> Không tính vào tỉ lệ báo xấu (report rate) của OA.**_

**Các lượt báo xấu sau 48 giờ từ lúc user nhận ZNS sẽ không ảnh hưởng đến tỉ lệ report và chất lượng của OA.**

- Ngoài ra, giao diện báo xấu mới sẽ được đồng bộ với giao diện báo xấu của tin UID, bao gồm danh sách lý do báo xấu.
- *Tham khảo thêm* [_Làm thế nào để giảm tỷ lệ báo xấu (report) khi gửi mẫu thông báo ZNS_](https://zalo.cloud/blog/lam-the-nao-de-giam-ty-le-bao-xau-report-khi-gui-mau-thong-bao-zns-/j4uvw9eppb98eka4a9).

### **Giao diện báo xấu và ngừng nhận thông báo ZNS của người dùng**
<p style={{ textAlign: "center" }}>
  <img src="https://content.zalo.cloud/uploads/image_b7668ff91a.png" /></p>
<p align="center">Giao diện khi bấm vào nút "..." góc phải thông báo ZNS</p>

<p style={{ textAlign: "center" }}>
  <img src="https://content.zalo.cloud/uploads/image_99a5c1ccca.png" /></p>
<p align="center">Giao diện khi bấm báo xấu tại bong bóng báo xấu bên dưới thông báo ZNS</p>

**Lưu ý**: Sản phẩm và giao diện thực tế có thể được điều chỉnh để đáp ứng yêu cầu vận hành và cải thiện trải nghiệm của người dùng cuối.

## 2. Cơ chế Ngừng nhận thông báo ZNS từ OA:

*   Khi đã thiết lập thành công việc cài đặt ngừng nhận thông báo từ OA, nếu muốn nhận lại thông báo ZNS, người dùng cần chủ động truy cập trang Quản lý tương tác OA và bật lại nút đồng ý nhận Thông báo từ OA.
*   Các điểm (Entry point) Ngừng nhận thông báo/Nhận lại thông báo: Người dùng có thể truy cập tính nắng ngừng nhận/nhận lại thông báo ZNS tại hai điểm:
    *   Trang cài đặt của Official Account (OA) > Chọn "Quản lý tương tác"**.**
    *   Giao diện báo xấu (ngay khi user thao tác báo xấu) (ngừng hỗ trợ từ 27/08/2025).
*   Ngoài ra, giao diện Ngừng nhận thông báo ZNS sẽ được đồng bộ với giao diện Ngừng nhận tin UID từ OA, nhằm mang đến trải nghiệm đồng nhất.

<p align="center">
  <img src="https://stc-oa.zdn.vn/uploads/2025/01/09/2a3bf36c22cb3cb664886f39a7c70e6d.png" />
</p>

_<p align="center">Giao diện mở nhận lại thông báo tại Trang cài đặt của Official Account (OA)</p>_

**Ghi chú:**

- User có thể tự thao tác trên thiết bị di động bất kì lúc nào (Zalo Business Solutions không hỗ trợ việc can thiệp quyền ngừng nhận ZNS của user).
- Khi OA gửi thông báo ZNS đến người dùng đã ngừng nhận thông báo ZNS từ OA, hệ thống sẽ trả về mã lỗi: _**\-141 User refused to receive ZNS**_. Mã lỗi này cho biết người dùng đã từ chối nhận ZNS từ Official Account.
- Từ ngày **07/01/2025**, **bỏ cơ chế ngừng nhận thông báo theo Tag:** người dùng đã cài đặt ngừng nhận thông báo ZNS của một số Tag hoặc toàn bộ Tag trước ngày 07/01 sẽ được chuyển đổi như sau:

<div class="table" align="center">
    <table class="ck-table-resized" style="border-collapse:collapse;border-style:none;margin-left:.75in;" border="1" cellspacing="0" cellpadding="0"><colgroup><col style="width:37.82%;"><col style="width:62.18%;"></colgroup><tbody><tr style="height:15.0pt;"><td style="border-color:black;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:396.8pt;" colspan="2" width="529"><p style="line-height:normal;margin-bottom:0in;text-align:center;"><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI"><strong>Cài đặt Ngừng nhận thông báo ZNS của User</strong></span></span></p></td></tr><tr style="height:15.0pt;"><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:198.4pt;" width="265"><p style="line-height:normal;margin-bottom:0in;"><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">Trước 07/01/2025</span></span></p></td><td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:198.4pt;" width="265"><p style="line-height:normal;margin-bottom:0in;"><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">Từ 07/01/2025</span></span></p></td></tr><tr style="height:15.0pt;"><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:198.4pt;" width="265"><p style="line-height:normal;margin-bottom:0in;"><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">Ngừng nhận <strong><u>bao gồm</u></strong> Tag 1 <strong><u>hoặc</u></strong> Tag 2&nbsp;</span></span></p></td><td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:198.4pt;" width="265"><p style="line-height:normal;margin-bottom:0in;"><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">Ngừng nhận toàn bộ ZNS ở tất cả các Tag</span></span></p></td></tr><tr style="height:15.0pt;"><td style="border-bottom-style:solid;border-color:black;border-left-style:solid;border-right-style:solid;border-top-style:none;border-width:1.0pt;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:198.4pt;" width="265"><p style="line-height:normal;margin-bottom:0in;"><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">Ngừng nhận chỉ ZNS Tag 3</span></span><br><br><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">Và không có ngừng nhận Tag 1 hoặc Tag 2</span></span></p></td><td style="border-bottom:1.0pt solid black;border-left-style:none;border-right:1.0pt solid black;border-top-style:none;height:15.0pt;padding:0in 5.4pt;vertical-align:top;width:198.4pt;" width="265"><p style="line-height:normal;margin-bottom:0in;"><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">Tự động bỏ cài đặt ngừng nhận ZNS</span></span></p><p style="line-height:normal;margin-bottom:0in;"><br><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><span lang="VI">User có thể chủ động thao tác tắt mở cài đặt này tùy theo nhu cầu.&nbsp;</span></span><br><span style="font-family:&quot;Aptos&quot;,sans-serif;font-size:18px;"><i><span lang="VI">Xem thêm tại phần 2 - Cơ chế ngừng nhận thông báo ZNS</span></i></span></p></td></tr></tbody></table>
</div>

_Nếu có bất kì yêu cầu hỗ trợ, Quý khách có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của chúng tôi qua **Biểu Mẫu: [Mẫu hỗ trợ Zalo Business Solutions](https://go.zalo.me/SupportZBS )**. Chúng tôi sẽ phản hồi Quý khách trong vòng 24h làm việc tiếp theo._

_**Lưu ý:**_ _Từ 06/08/2025, **Zalo Cloud** chính thức đổi tên thành **Zalo Business Solutions.** Việc ra mắt thương hiệu Zalo Business Solutions (ZBS) là sự thay đổi về mặt nhận diện thương hiệu, không làm thay đổi về mặt pháp lý đối với các hoạt động, giao dịch và cam kết đã có trước đây dưới tên gọi Zalo Cloud._

