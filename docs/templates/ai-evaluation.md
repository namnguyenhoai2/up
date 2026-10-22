---
title: "Mẫu ghi chép đánh giá AI"
description: "Ghi lại phạm vi nhiệm vụ, mẫu được giữ lại, phiên bản, điều kiện bắt buộc, các lỗi và toàn bộ chi phí, nhằm hỗ trợ quyết định áp dụng, khắc phục hoặc rút lại quy trình AI."
updated: 2026-10-16
---

# Mẫu ghi chép đánh giá AI

Được sử dụng cùng với [Đánh giá và độ tin cậy của AI](../threads/practice/ai-evaluation.md). Trước tiên hãy điền các tiêu chuẩn, sau đó chạy các trường hợp. Bảng trống dùng để ghi chép việc so sánh một phiên bản; các con số minh họa không đại diện cho hiệu suất của mô hình hoặc ngưỡng triển khai chung.

## Bản ghi có thể sao chép

```markdown
# AI Evaluation — 日期 / 任务

## 范围
- 用户和要完成的动作：
- 输入材料、权限和去标识方式：
- 人工基线及总耗时：
- 不支持的任务：

## 测试设置（运行前固定）
- 当前版本 / 候选版本：
- 模型、提示、检索材料、工具版本：
- 运行日期、地区、记忆设置；无法固定的服务版本：
- 本轮只改变什么：
- 开发样本 / 未参与调优的保留样本：
- 每例运行次数及时间、调用、费用上限：
- 必须全部通过的条件：
- 可比较的质量与人工评分说明：
- 评分人 / 争议如何解决：
- 相关失败场景：来源缺失 / 提示注入 / 越权 / 失控重试或重复副作用 / 转写或识图错误：
- 长时任务字段：任务/运行编号、检查点、墙钟时间、超时、最大重试、重复安全标识、人工接管点：
- 隔离字段：干净环境、网络出口白名单、凭证范围、浏览器/页面不可信输入说明：
- 政策字段：供应商政策名称、版本、生效日期、地区、高风险人工复核：

## 逐例记录（每个版本分别复制本区）
- 本区版本：
- ID 使用“案例编号 / 尝试序号”，例如 07 / 2；输入指向固定的案例材料。
### 案例（每次尝试复制一份）
- 案例编号 / 尝试序号：
- 类型与固定输入材料位置：
- 预期行为 / 判断依据：
- 支持结论的原文位置 / 音视频时间段 / 图片区域：
- 实际行为 / 产物位置：
- 过程记录 / 工具调用 / 授权记录位置：
- 检查点 / 恢复编号 / 重试与重复安全记录：
- 网络出口、页面或截图证据、凭证范围：
- 最终环境结果（文件、数据库或用户可见状态）：
- 首次是否合格 / 硬性条件失败：
- 人工修改分钟 / 修改内容：
- 最终状态（失败与超时也保留）：

## 汇总（每个版本单独计算，失败与超时保留在分母中）
- 首次合格数 / 全部尝试数：
- 必须条件失败及具体案例：
- 人工修改后合格数 / 全部尝试数：
- 准备、运行、核验、返工总分钟：
- 工具费用及工时估值口径：
- 本批总过程成本 / 最终合格数量：
- 证据限制与不支持的推断：

## 决定与后续
- 采用 / 维持现状 / 修复复测 / 停止：
- 支持这个决定的案例：
- 新增回归案例及重跑范围：
- 模型、资料、工具或记忆变化后的复测触发；上次合格版本：
- 允许使用范围 / 人工接管 / 撤回触发：
- 换供应商、关闭记忆或断开工具后的退出演练结果：
- 负责人、复查日期、记录位置：
```

Nếu số lượng kết quả đạt yêu cầu cuối cùng bằng không, ghi chi phí cho mỗi kết quả đạt yêu cầu là “không thể tính toán”, giữ nguyên tổng chi phí đã phát sinh, không thay bằng số không.

## Ví dụ điền biểu mẫu: Bảng so sánh tài liệu công khai

Dưới đây là trường hợp giả định, nhất quán với ví dụ trong chương: mỗi trong mười trường hợp được chạy một lần, phiên bản hiện tại A đạt yêu cầu lần đầu ở 8 trường hợp, ứng viên B đạt yêu cầu lần đầu ở 9 trường hợp; sau khi được con người chỉnh sửa, cả hai phiên bản đều đạt yêu cầu ở 10 trường hợp.

| Trường | Nội dung điền mẫu |
| --- | --- |
| Thay đổi trong vòng này | Chỉ sửa lời nhắc trích xuất, tài liệu và công cụ giữ nguyên |
| Điều kiện bắt buộc | Các con số quan trọng phải có nguồn; không được suy đoán giá bị thiếu |
| Ghi chép lỗi B-07 | Văn bản gốc không cung cấp giá; B viết thành “miễn phí”; con người sửa lại thành “không cung cấp” |
| Chi phí của A | Tổng thời gian làm việc 120 phút, định giá theo mức 60 nhân dân tệ/giờ, công cụ 6 nhân dân tệ; tổng cộng 126 nhân dân tệ |
| Chi phí của B | Tổng thời gian làm việc 100 phút, định giá tương tự, công cụ 8 nhân dân tệ; tổng cộng 108 nhân dân tệ |
| Quyết định | Giữ nguyên phạm vi hiện tại; trước tiên khắc phục B, chưa mở rộng sử dụng |
| Bước tiếp theo | Bổ sung các trường hợp thiếu giá, giá đã hết hiệu lực và giá mâu thuẫn, đồng thời chạy lại các trường hợp trước đó đã đạt yêu cầu |
| Hạn chế của bằng chứng | Mẫu nhỏ và mỗi trường hợp chỉ chạy một lần; không thể suy ra tỷ lệ lỗi khi vận hành trực tuyến; đúng sau khi chỉnh sửa không đồng nghĩa với đáng tin cậy một cách tự chủ |

Lưu kết quả thực tế trong các tệp có thể kiểm tra lại. Khi ghi “đã hoàn thành”, hãy đính kèm tệp, đầu ra kiểm thử hoặc trạng thái hệ thống, thay vì chỉ dán tuyên bố hoàn thành của mô hình.

## Từ ghi chép đến hành động

Mỗi vòng chỉ khắc phục một kiểu lỗi chính và kiểm tra xem các trường hợp cũ có bị suy giảm hay không. Khi quy trình vẫn chưa rõ ràng, hãy quay lại [Bản tóm tắt nhiệm vụ AI](ai-task-brief.md); khi dự án sẵn sàng cung cấp dịch vụ ra bên ngoài, hãy điền [Thẻ thử nghiệm khởi nghiệp](startup-experiment.md), lần lượt xác minh chất lượng kết quả và nhu cầu thực tế.