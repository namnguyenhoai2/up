---
title: "Bản tóm tắt sản phẩm và thẻ bàn giao"
description: "Quản lý một sản phẩm học tập hoặc dự án có thể kiểm tra và bàn giao bằng đối tượng, đường cơ sở, phiên bản, phản hồi, cổng chất lượng và điều kiện khôi phục."
updated: 2026-08-31
---

# Bản tóm tắt sản phẩm và thẻ bàn giao

Sản phẩm không nhất thiết phải hoàn chỉnh ngay từ đầu, nhưng ngay từ đầu phải có ranh giới rõ ràng. Sao chép thẻ này vào thư mục dự án riêng tư, lưu giữ các phiên bản độc lập, sửa đổi, phản hồi và bàn giao riêng biệt. Không ghi mật khẩu, thông tin khách hàng, thông tin bên thứ ba chưa được cấp phép hoặc dữ liệu riêng tư không cần thiết.

## 1. Phạm vi sản phẩm

```markdown
# Artifact Brief — YYYY-MM-DD

作品名称：
真实场景：
受众/使用者：
要解决的一个问题：

输入材料与来源：
我当前的基线：
关键假设：

最小交付物：
格式、时间与其他限制：
完成标准：
明确不做什么：

第一版截止时间：
谁会提供反馈：
需要保留的证据：
失败时如何缩小、暂停或回滚：
下一次复查日期：
```

## 2. Bốn phiên bản

| Phiên bản | Điều kiện hoàn thành | Nội dung cần lưu giữ |
| --- | --- | --- |
| Độc lập | Hoàn thành thao tác tối thiểu mà không xem đáp án, không để AI viết thay | Tệp gốc, thời gian thực hiện, điểm vướng mắc |
| Cấu trúc | Đối tượng có thể tìm thấy vấn đề, kết luận và bước tiếp theo | Khác biệt về cấu trúc, đánh dấu sự kiện và suy đoán |
| Phản hồi | Người đọc, người dùng, đồng nghiệp thực tế hoặc AI đóng vai trò cụ thể hoàn tất việc xem xét | Phản hồi, phân loại lỗi, lý do tiếp nhận/từ chối |
| Bàn giao | Người khác có thể bắt đầu sử dụng mà không phụ thuộc vào phần bổ sung bằng lời nói của bạn | Phiên bản, giới hạn, nguồn, vấn đề đã biết, ghi chép bàn giao |

## 3. Cổng chất lượng

| Cổng | Câu hỏi kiểm tra | Vị trí bằng chứng | Người phụ trách/ngày |
| --- | --- | --- | --- |
| Rõ ràng | Đối tượng có biết vấn đề và bước tiếp theo không? | | |
| Chính xác | Sự kiện, trích dẫn, mã và số liệu có thể truy về nguồn hoặc kiểm thử không? | | |
| Khả dụng | Thao tác chính có thể hoàn thành trong các giới hạn thực tế không? | | |
| Có thể bảo trì | Phiên bản, phần phụ thuộc, giới hạn và người tiếp nhận có rõ ràng không? | | |
| Có trách nhiệm | Quyền riêng tư, bản quyền, quyền hạn và hậu quả của lỗi đã được xử lý chưa? | | |

Những nội dung “đạt” không có bằng chứng trước tiên hãy ghi là “chờ xác minh”. Tốc độ, số từ và số lượng tính năng chỉ là các chỉ số đại diện, không thể thay thế cho cổng chất lượng.

## 4. Ghi chép về AI và phản hồi

```markdown
AI/工具与日期：
允许它做的工作：
我保留的人类判断：
它指出的三个最高影响问题：
我采纳/拒绝了什么，为什么：
真实读者/用户复述的主旨：
最需要修正的一处：
```

Trước tiên hãy lưu phiên bản của chính mình, sau đó mới để AI chẩn đoán, mô phỏng đối tượng hoặc tạo nhiệm vụ song song. Con người phải xác nhận các sự kiện quan trọng, quyền hạn, quyền riêng tư, chi phí và tên người chịu trách nhiệm cuối cùng.

## 5. Bàn giao và khôi phục

```markdown
交付对象与授权范围：
交付日期与版本：
使用说明：
已知限制：
支持与联系人：
成本与留存期限：
暂停/降级/回滚触发条件：
发现问题后的通知对象：
下一次复查日期：
```

Bàn giao không phải là điểm kết thúc. Ít nhất sau 3–7 ngày, hãy kiểm thử lại một lần trong các điều kiện tương tự, ghi lại liệu người khác có thể tự mình bắt đầu hay không, nơi nào cần giải thích, và phiên bản tiếp theo chỉ thay đổi điều gì.

Chương liên quan: [Chương sản phẩm: Biến việc học được thành việc làm ra](../threads/part-3/4-artifacts-and-delivery.md) ｜ [Bảng tổng hợp hành động trong chín mươi ngày](90-day-cycle.md)