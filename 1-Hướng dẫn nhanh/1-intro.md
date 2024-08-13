---
id: intro
title: Tổng quan về Zalo Notification Service
slug: /guidelines/intro
---

## Tổng quan

Zalo Notification Service (ZNS) là giải pháp gửi thông báo từ Zalo Official Account (OA) của doanh nghiệp tới khách hàng trên nền tảng Zalo. ZNS gồm các thành phần chính như:

- Zalo Cloud Account (ZCA)
- Official Account (OA)
- Ứng dụng (App)
- ZNS Template
- ZNS API

![alt_text](../images/zns.jpg "image_tooltip")

## Giới thiệu về các thành phần của ZNS {#giới-thiệu-về-các-thành-phần-của-zns}

### 1. ZCA

**Zalo Cloud Account (ZCA) **là công cụ quản lý số dư tiền để sử dụng tính năng tính phí của các tài khoản Zalo Official Account - Doanh Nghiệp (OA) và các ứng dụng ủy quyền của Doanh Nghiệp (App). ZCA có các chức năng chính như:

- Quản lý chi tiêu
- Quản lý việc sử dụng các dịch vụ
- Quản lý giao dịch
- Trả phí các dịch vụ
- Quản lý tài sản
- Quản lý chất lượng gửi tin

### 2. OA

**Zalo Official Account doanh nghiệp (OA)** là tài khoản chính thức của doanh nghiệp trên Zalo, giúp doanh nghiệp và khách hàng/người quan tâm tương tác với nhau dễ dàng hơn. Khi thực hiện gửi ZNS, tên OA sẽ đại diện xuất hiện trong thông báo được gửi đến người dùng Zalo.

Tài khoản ZCA cần liên kết với OA để ủy quyền sử dụng các tính năng trả phí. Để liên kết OA, bạn cần có quyền Quản trị viên của OA đó.

### 3. App

**Ứng dụng (App)** là đơn vị đại diện của OA để thực hiện việc gửi thông báo ZNS đến người dùng Zalo. Một Ứng dụng có thể thay mặt nhiều OA thực hiện gửi thông báo ZNS đến khách hàng.

Ứng dụng cần liên kết với ZCA để sử dụng các tính năng trả phí. Để liên kết với ZCA, bạn cần có quyền Quản trị viên của ứng dụng.

### 4. ZNS Template

ZNS Template API cho phép gửi thông báo CSKH thông qua API đến khách hàng của Doanh nghiệp đang sử dụng Zalo trong điều kiện đáp ứng đủ các tiêu chuẩn về <ins>[chính sách dịch vụ](https://zalo.cloud/terms)</ins> được quy định. Để gửi được ZNS Template API, OA cần tạo và gửi duyệt template ZNS trước.

ZNS cung cấp nhiều loại Template khác nhau để phục vụ việc tương tác với người dùng một cách linh hoạt gồm OTP, ZNS dạng bảng, ZNS văn bản, ZNS đánh giá dịch vụ,...

### 5. ZNS API

ZNS API là các phương thức được cung cấp bởi ZNS cho phép Doanh nghiệp tăng cường khả năng tương tác và tiếp cận người dùng thông qua Zalo.

Xem chi tiết các API Zalo cung cấp <ins>[tại đây](https://developers.zalo.me/docs/api/zalo-notification-service-api/bat-dau/gioi-thieu-zalo-notification-service-api-post-5198)</ins>

_Để bắt đầu sử dụng ZNS, vui lòng xem chi tiết <ins>[tại đây](/set-up)</ins>_
