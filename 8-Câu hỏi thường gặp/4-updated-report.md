---
id: bao-xau-mau-tin-nhan-zbs-template-duoc-ghi-nhan-khi-nao
title: Báo xấu tin nhắn ZBS Template được ghi nhận khi nào?
slug: /bao-xau-mau-tin-nhan-zbs-template-duoc-ghi-nhan-khi-nao
---

# <p align="center">Báo xấu tin nhắn ZBS Template được ghi nhận khi nào?</p>

Để đảm bảo trải nghiệm của người dùng cuối (end-user), user có quyền lựa chọn báo xấu các tin nhắn ZBS template đã nhận để phản ánh chất lượng dịch vụ.

## 1. Cơ chế Báo xấu (Report):

1.  **Thay Đổi Entry Point Báo Xấu:** người dùng có thể báo xấu thông qua Chạm và giữ tin nhắn ZBS template
2.  **Hành động Báo xấu và ngừng nhận tin được xác định là hai hành động độc lập:**

    - Khi user báo xấu 1 tin nhắn ZBS template từ OA Brand A, hệ thống sẽ **KHÔNG tự động** ngừng nhận tin nhắn ZBS template từ OA này. Nếu user muốn ngừng nhận ZNS từ OA này, user có thể chủ động thao tác **“Chặn OA”**.
      Nếu user chọn “Nội dung tin không hiển thị hoặc hiển thị lỗi” hoặc “Lý do khác” _**=> Không tính vào tỉ lệ báo xấu (report rate) của OA.**_

**Các lượt báo xấu sau 48 giờ từ lúc user nhận tin nhắn ZBS template sẽ không ảnh hưởng đến tỉ lệ report và chất lượng của OA.**

- Ngoài ra, giao diện báo xấu mới sẽ được đồng bộ với giao diện báo xấu của tin UID, bao gồm danh sách lý do báo xấu.
- *Tham khảo thêm* [_Làm thế nào để giảm tỷ lệ báo xấu (report) khi gửi tin nhắn ZBS template_](https://zalo.solutions/blog/lam-the-nao-de-giam-ty-le-bao-xau-report-khi-gui-mau-thong-bao-zns-/j4uvw9eppb98eka4a9).

**Lưu ý**: Sản phẩm và giao diện thực tế có thể được điều chỉnh để đáp ứng yêu cầu vận hành và cải thiện trải nghiệm của người dùng cuối.

## 2. Cơ chế Ngừng nhận tin nhắn ZBS template từ OA:

*   Khi đã thiết lập thành công việc cài đặt ngừng nhận tin từ OA, nếu muốn nhận lại tin nhắn ZBS template, người dùng cần chủ động truy cập trang OA, và tiến hành bỏ chặn OA.
*   Các điểm (Entry point) Ngừng nhận thông báo/Nhận lại thông báo: Người dùng có thể truy cập tính nắng ngừng nhận/nhận lại tin nhắn ZBS template tại Trang cài đặt của Official Account (OA) > Chọn "Quản lý chặn"**.**

<p align="center">
  <img src="https://content.zalo.cloud/uploads/image_e5ef2485a8.png" />
</p>

_<p align="center">Giao diện mở nhận lại tin nhắn tại Trang cài đặt của Official Account (OA)</p>_

**Ghi chú:**

- User có thể tự thao tác trên thiết bị di động bất kì lúc nào (Zalo Business Solutions không hỗ trợ việc can thiệp quyền ngừng nhận ZNS của user).
- Khi OA gửi tin nhắn ZBS template đến người dùng đã ngừng nhận tin từ OA, hệ thống sẽ trả về mã lỗi: _**\-141 User refused to receive ZNS**_. Mã lỗi này cho biết người dùng đã từ chối nhận tin nhắn ZBS template từ Official Account.>


_Nếu có bất kì yêu cầu hỗ trợ, Quý khách có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của chúng tôi qua **Biểu Mẫu: [Mẫu hỗ trợ Zalo Business Solutions](https://zalo-solutions.freshdesk.com/en/support/tickets/new)**. Chúng tôi sẽ phản hồi Quý khách trong vòng 24h làm việc tiếp theo._

