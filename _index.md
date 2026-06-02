---
author: Khoa
title: "Virtual Private Cloud"
weight: 5
icon: fa fa-cloud-upload
---
*Kính chào quý khách,*

***Virtual Private Cloud** (**VPC**) là công nghệ không còn quá mới mẻ với cộng đồng công nghệ nói chung và lĩnh vực cloud nói riêng. Đa số các nhà cung cấp dịch vụ Cloud lớn như AWS, Azure hay GCP đều cung cấp công nghệ này, và VNDATA hiện tại cũng đang cung cấp dịch vụ này. Xin mời quý khách cùng xem qua bài viết bên dưới của VNDATA để cùng hiểu rõ hơn về định nghĩa cũng như ứng dụng của **VPC**.*

## VPC là gì?

* VPC là mạng riêng ảo được triển khai trên hạ tầng Cloud, cho phép người dùng định nghĩa và tự kiểm soát không gian địa chỉ IP (CIDR), phân chia Subnet, cấu hình routing và chính sách bảo mật cho các tài nguyên.
* Các tài nguyên trong VPC được cô lập ở mức network với các tenant khác, đồng thời có thể kết nối ra bên ngoài thông qua các cơ chế như NAT hoặc Internet Gateway.

## Vì sao cần sử dụng dịch vụ VPC?

* Mỗi VPC được cách ly hoàn toàn ở mức mạng, không bị ảnh hưởng bởi tenant khác. Điều này giúp an toàn về mặt thông tin, cũng như tránh conflict các tài nguyên.
* Toàn quyền kiểm soát mạng, Người dùng có thể tùy chỉnh CIDR (IP Range), tạo subnet từ CIDR ban đầu, cấu hình routing cũng như firewall. Vì vậy, người dùng hoàn toàn chủ động thiết kế kiến trúc (fe/be/db...).
* Performance cao, Traffic nội bộ trong VPC không đi qua internet, giúp latency thấp, bandwidth cao, và ổn định hơn so với public internet.
* Dễ dàng mở rộng hệ thống mạng và tài nguyên tính toán khi cần thiết.
* Kết nối linh hoạt khi hỗ trợ các tính năng NAT, Internet Gateway và kết nối VPN.

## VPC hoạt động như thế nào?

![001](001.png)

Tuỳ vào dịch vụ của từng nhà cung cấp thì cách hoạt động của VPC có thể khác nhau đôi chút, trong khuôn khổ bài viết chúng tôi sẽ giới thiệu về cách hoạt động của dịch vụ **VPC** do VNDATA cung cấp như sau:
* Lựa chọn gói tài nguyên phù hợp với quy mô ứng dụng, đăng ký và bắt đầu sử dụng. Tạo project, đặt tên và mục đích của project.
* Tạo các instances, chọn hệ điều hành, tài nguyên cho từng instance phù hợp với yêu cầu.
* Tạo VPC Network, Public Network... theo thiết kế.

# Vì sao nên chọn nhà cung cấp dịch vụ VPC tại Việt Nam?

* Nhà cung cấp Public Cloud ở Việt Nam, nên việc hỗ trợ dịch vụ rất nhanh chóng, việc liên lạc cũng thuận lợi hơn các nhà cung cấp nước ngoài.
* Đảm bảo được vấn đề về giá cả, pháp lý và bảo mật dữ liệu do nhà cung cấp tại Việt Nam sẽ đảm bảo tuân thủ các quy định do chính phủ đưa ra.

