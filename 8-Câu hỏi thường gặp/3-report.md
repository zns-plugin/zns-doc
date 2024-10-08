---
id: bao-xau-mau-thong-bao-zns-duoc-ghi-nhan-khi-nao
title: Báo xấu mẫu thông báo ZNS được ghi nhận khi nào?
slug: /bao-xau-mau-thong-bao-zns-duoc-ghi-nhan-khi-nao
---

# <p align="center">Báo xấu mẫu thông báo ZNS được ghi nhận khi nào?</p>

Để đảm bảo trải nghiệm của người dùng cuối (end-user), user có quyền lựa chọn báo xấu các mẫu thông báo Zalo Notification Service (ZNS) đã nhận để phản ánh chất lượng dịch vụ.

Điều này cũng sẽ ảnh hưởng đến [Cơ chế đánh giá chất lượng và quyền lợi gửi ZNS](https://zalo.cloud/blog/co-che-danh-gia-chat-luong-va-quyen-loi-gui-zns/rzu6k97e8vkbnmereg).

## 1. Giao diện báo xấu mẫu thông báo ZNS của người dùng

<div style="text-align:center;"><img class="image_resized" style="width:48.89%;" src="https://stc-oa.zdn.vn/uploads/cf1255bf5b13b0c32eccb5fa26fd64da.png"><img class="image_resized" style="width:42.05%;" src="https://stc-oa.zdn.vn/uploads/76f78e0f93bec203d8432085014dd0d1.png"></div>

**Quy định:**

- Bong bóng **“Bạn cảm thấy phiền? Báo xấu”** sẽ tồn tại trong 48 giờ từ lúc user nhận ZNS. Sau thời gian này, bong bóng sẽ biến mất.
- Khi user report thông báo Tag 1 - Giao dịch **hoặc** Tag 2 - Chăm sóc khách hàng → User sẽ tự động ngừng nhận toàn bộ ZNS từ OA
  - Khi OA tiếp tục gửi thông báo cho user này sẽ nhận mã lỗi -141: User refused to receive ZNS / Người dùng từ chối nhận ZNS từ Official Account
- Khi user report các thông báo Tag 3 - Hậu mãi → User sẽ tự động ngừng nhận toàn bộ ZNS Tag 3 (Các thông báo Tag 1 và 2 vẫn nhận bình thường)
  - Khi OA tiếp tục gửi thông báo template Tag 3 cho user này sẽ nhận mã lỗi -139: User refused to receive this type of ZNS / Người dùng từ chối nhận loại ZNS này.
- User có thể tự điều chỉnh quyền nhận tin nhắn và bỏ chặn nếu có nhu cầu (vẫn tính report rate theo [Cơ chế đánh giá chất lượng và quyền gửi tin ZNS](https://zalo.cloud/blog/co-che-danh-gia-chat-luong-va-quyen-loi-gui-zns/rzu6k97e8vkbnmereg))
- Nếu user chọn **“Nội dung tin không hiển thị hoặc hiển thị lỗi”** hoặc **“Lý do khác”** → Không tính vào tỉ lệ báo xấu (report rate) của OA

_Tham khảo thêm_ [_Làm thế nào để giảm tỷ lệ báo xấu (report) khi gửi mẫu thông báo ZNS_](https://zalo.cloud/blog/lam-the-nao-de-giam-ty-le-bao-xau-report-khi-gui-mau-thong-bao-zns-/j4uvw9eppb98eka4a9)

## 2. Cách thay đổi quyền nhận mẫu thông báo ZNS (sau khi user báo xấu)

### **Cách 1: Thao tác ngay khi gửi phản hồi báo xấu mẫu thông báo ZNS**

<p style="text-align:center;"><img class="image_resized" style="width:24.73%;" src="https://stc-oa.zdn.vn/uploads/a9d5f78ffe78611ca2f5596a7d7d9243.png"><img class="image_resized" style="width:24.73%;" src="https://stc-oa.zdn.vn/uploads/b472b64d3abac70f892b4af175d6976e.png"></p>

### **Cách 2: Thao tác trên bong bóng phản hồi tại giao diện chat với OA ngay khi báo xấu**

<p style="margin-left:0px;text-align:center;"><img class="image_resized" style="width:20.22%;" src="https://stc-oa.zdn.vn/uploads/722a04e1f4429d2a0cbc3927b57063ac.png"><img class="image_resized" style="width:20.23%;" src="https://stc-oa.zdn.vn/uploads/fccce5ad2630c23114198c8c5f59f3f9.png"></p>

**Ghi chú:**

- User có thể tự thao tác trên thiết bị di động bất kì lúc nào (Zalo Cloud không hỗ trợ việc can thiệp quyền nhận ZNS của user)
- Chỉ nhận thông báo liên quan giao dịch: Chỉ nhận mẫu thông báo Tag 1 - Giao dịch
- Chỉ nhận thông báo liên quan giao dịch và cập nhật: Chỉ nhận mẫu thông báo Tag 1 - Giao dịch và mẫu thông báo Tag 2 - Chăm sóc khách hàng
- Nhận tất cả thông báo: Nhận mẫu thông báo ở tất cả Tag 1 - Giao dịch, Tag 2 - Chăm sóc khách hàng, Tag 3 - Hậu mãi

_Nếu có bất kì yêu cầu hỗ trợ, khách hàng có thể liên hệ với đội ngũ hỗ trợ và chăm sóc khách hàng của Zalo Cloud qua email:_ [_support@zalo.cloud_](mailto:support@zalo.cloud)_. Đội ngũ CSKH Zalo Cloud sẽ phản hồi cho khách hàng trong vòng 24h làm việc tiếp theo._
