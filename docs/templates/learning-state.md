---
title: "Mẫu trạng thái học tập"
description: "Dùng một tệp trạng thái duy nhất để lưu mục tiêu, đường cơ sở, nội dung đã hoàn thành, bằng chứng về lỗi và bước tiếp theo. Cả con người lẫn AI đều có thể tiếp tục công việc qua nhiều phiên."
updated: 2026-10-06
---

# Mẫu trạng thái học tập

Sao chép mẫu dưới đây vào ghi chú riêng tư của bạn. Đây là nguồn sự thật dùng xuyên suốt các phiên, không phải nhật ký thể hiện tính kỷ luật. Không ghi mật khẩu, giấy tờ tùy thân, địa chỉ chính xác, thông tin riêng tư về y tế hoặc thông tin của bên thứ ba khi chưa được cho phép.

## Nếu hôm nay chỉ có năm phút

Đừng vội điền đầy đủ cả bảng. Hãy sao chép phiên bản tối thiểu bên dưới, viết xong rồi bắt tay vào hành động; chỉ bổ sung mẫu đầy đủ khi nhiệm vụ cần tiếp tục qua nhiều phiên, bàn giao hoặc xem xét lại.

```markdown
# Learning State — minimum

日期：YYYY-MM-DD
我正在处理的真实问题：
我已经拥有的证据：
今天能完成的最小动作：
完成后要留下的证据：
我不会上传或公开的内容：
```

Tiêu chuẩn hoàn thành của phiên bản tối thiểu là: một phiên bản tương lai khác của chính bạn có thể hiểu hiện tại cần giải quyết điều gì, đã biết những gì, bước tiếp theo là gì và những ranh giới nào không được vượt qua. Đây không phải là kế hoạch hoàn chỉnh, cũng không thể thay thế việc kiểm tra lại một cách độc lập; nó chỉ giúp hành động diễn ra trước.

```markdown
# Learning State

状态版本：v1
更新时间：YYYY-MM-DD
维护人：
主文件位置：

## 目标
- 真实场景：
- 当前主任务：
- 12 周结果：
- 本周重点：
- 完成标准：
- 截止日期：

## 约束与边界
- 每周可用时间/精力：
- 可以使用的材料与工具：
- 不应上传或公开的内容：
- AI 可以协助：
- 必须由人确认：

## 当前水平与基线
- 我现在能完成：
- 基线样本位置：
- 最近一次评分/反馈：

| 样本 | 条件 | 位置 | 日期 | 仍然不能说明什么 |
| --- | --- | --- | --- | --- |
| | | | | |

## 已完成
- [日期] 任务 — 输出/证据位置 — 结果/下一步

## 错误、风险与待补知识
| 错误/风险 | 证据 | 可能原因/置信度 | 下一次处理与停止条件 |
| --- | --- | --- | --- |

## 已验证有效的方法
- 方法 — 在什么条件下有效 — 证据

## 待验证假设
- 假设 — 反例 — 下一次怎么检验 — 截止日期

## 最近一次交接
- 已完成与证据：
- 仍未确认的事实：
- 未决选择：
- 已发生的成本/返工：
- 下一次打开文件先做什么：
- 需要通知或征求意见的人：

## 下一步
1. 下一项最小任务：
2. 预计时长：
3. 需要材料：
4. 完成后保存什么证据：
5. 下次复查日期：
```

## Lời nhắc khôi phục AI qua nhiều phiên

```text
下面是我的学习状态文件。先用不超过 6 条要点复述状态版本、目标、当前证据、主要错误、边界和下一步，指出信息冲突或缺口，不要假装记得其他会话，也不要补写文件里没有的事实。然后只为“下一项最小任务”设计一次练习：先让我作答，再按完成标准反馈；除非我请求，不要直接给完整答案。结束时输出可粘贴回状态文件的“本次完成、证据、错误/风险、交接、下一步”五项更新。

[粘贴 Learning State]
```

Bản tóm tắt trạng thái do AI tạo ra không phải là nguồn sự thật. Mỗi lần khôi phục, hãy lấy tệp, sản phẩm, nguồn và số phiên bản bạn đã lưu làm chuẩn; sau khi hoàn thành một lần xem xét hằng tuần, hãy cập nhật [bản xem xét hằng tuần](weekly-review.md), [chuỗi bằng chứng](evidence-chain.md) và [bảng hành động chín mươi ngày](90-day-cycle.md) theo đúng chức năng của từng tệp, đừng sao chép cùng một đoạn ghi chép.