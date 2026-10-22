---
title: "Bản tóm tắt nhiệm vụ AI: từ vấn đề đến nghiệm thu thủ công"
description: "Viết rõ nhiệm vụ thực tế, ranh giới dữ liệu, nguồn, tập đánh giá, trách nhiệm của con người, chi phí, cách xử lý thất bại và điều kiện bàn giao trước khi bắt đầu học AI hoặc dự án."
updated: 2026-10-16
---

# Bản tóm tắt nhiệm vụ AI: từ vấn đề đến nghiệm thu thủ công

Sao chép vào thư mục dự án riêng tư và điền trước khi gọi mô hình. Đây không phải là nơi thu thập prompt, mà là giấy phép bắt đầu: nếu nhiệm vụ, dữ liệu, nguồn, tiêu chí nghiệm thu hoặc người chịu trách nhiệm vẫn chưa rõ ràng thì trước tiên đừng để mô hình tạo ra kết quả cuối cùng.

Không ghi mật khẩu, giấy tờ tùy thân, địa chỉ chính xác, thông tin y tế riêng tư, dữ liệu trẻ em, hồ sơ khách hàng, lỗ hổng chưa công bố hoặc nội dung của bên thứ ba mà bạn không có quyền sử dụng. Trước tiên hãy ẩn danh tài liệu nhạy cảm hoặc chuyển sang môi trường được tổ chức phê duyệt.

## 1. Nhiệm vụ và trách nhiệm

```markdown
# AI Task Brief - YYYY-MM-DD

真实场景：
使用者/受众：
要完成的决策或动作：
为什么现在做：
截止时间与不可错过的节点：
最终负责人与人工审阅者：
如果不做或延迟，谁会受影响：
```

Hãy chuyển “học AI” hoặc “làm một trợ lý thông minh” thành các hành động có thể quan sát được, chẳng hạn như “người dùng có thể nhập một tệp trong vòng 10 phút và xem một báo cáo có thể giải thích nguồn gốc và lỗi”.

## 2. Dữ liệu đầu vào, nguồn và ranh giới dữ liệu

| Đầu vào/khẳng định | Loại | Nguồn, phiên bản và vị trí | Có thể cung cấp cho mô hình không | Người xác minh | Điều kiện mất hiệu lực |
| --- | --- | --- | --- | --- | --- |
| | Sự thật / suy luận / kinh nghiệm cá nhân / dữ liệu người dùng / nội dung bên thứ ba | | Công khai / đã ẩn danh / được tổ chức phê duyệt / cấm | | |

```markdown
允许使用的文件和字段：
明确不提供的材料：
数据敏感等级：公开 / 内部 / 机密 / 受限
收集、传输、留存和删除期限：
是否取得必要同意：
版权、许可证、引用和署名要求：
模型能接触的最小数据范围：
```

Nguồn không đồng nghĩa với sự thật. Mỗi khẳng định quan trọng phải có thể truy về văn bản gốc, phiên bản, phạm vi dữ liệu hoặc quan sát trực tiếp; các liên kết, con số và trích dẫn do mô hình đưa ra vẫn cần được con người xác minh.

## 3. Kết quả đầu ra và tập đánh giá

```markdown
最终交付物：
格式、长度和受众：
可观察的完成标准：
必须通过的硬门：
允许的可接受变体：
明确不能出现的内容：
```

Hãy xây dựng một tập đánh giá nhỏ nhưng chân thực, đừng chỉ sử dụng những ví dụ mà mô hình làm tốt nhất:

| Mẫu | Điều kiện đầu vào | Kết quả mong đợi | Kết quả không thể chấp nhận | Kết quả thực tế | Vị trí bằng chứng |
| --- | --- | --- | --- | --- | --- |
| Mẫu thông thường | | | | | |
| Mẫu biên | | | | | |
| Đầu vào thiếu/mâu thuẫn | | | | | |
| Mẫu lịch sử thực tế (đã ẩn danh) | | | | | |

Nghiệm thu ít nhất phải trả lời được: sự thật có thể truy nguyên không, các hành động quan trọng đã hoàn thành chưa, lỗi có thể nhìn thấy không, quyền hạn có chính xác không, và khi thất bại có thể dừng lại không. Trôi chảy, nhanh hoặc “giống con người” không phải là tiêu chí nghiệm thu.

## 4. Phạm vi công việc của AI

```markdown
AI 可以做：提问 / 分类 / 候选解释 / 反例 / 转写 / 草稿 / 测试建议
AI 不可以做：最终事实判断 / 虚构来源 / 代替责任人批准 / 越过权限
                    / 完成禁止外部帮助的考试或申请 / 自动发布
使用模式：诊断 / 辅助 / 生成候选 / 批量处理 / 其他
模型、版本、区域和调用日期：
外部工具、MCP 服务器或其他协议及版本：
每个工具的读取/写入范围、授权人和撤回方式：
提示词、系统指令或工作流版本位置：
```

Nếu nhiệm vụ sẽ chạy trong thời gian dài hoặc gọi các công cụ bên ngoài, cũng cần ghi lại:

```markdown
运行/任务编号及父任务编号：
异步或同步；预计与最大墙钟时间：
检查点位置与恢复步骤：
最大重试次数、超时和重复安全标识：
浏览器页面、截图和外部指令均视为不可信输入：
网络出口白名单与凭证范围：
外部写入、收据和最终环境状态：
人工接管点与紧急停止方式：
供应商政策/版本、生效日期、地区和高风险复核：
```

Trước tiên hãy để mô hình nhắc lại mục tiêu, đầu vào, giới hạn, các mục chưa biết và tiêu chí nghiệm thu, rồi mới bắt đầu tạo nội dung. Quản lý phiên bản prompt; đừng coi một cửa sổ trò chuyện duy nhất là hồ sơ dự án duy nhất.

## 5. Cổng kiểm tra thủ công

| Cổng | Ai bắt buộc phải xác nhận | Bằng chứng đạt | Khi không đạt |
| --- | --- | --- | --- |
| Cổng nguồn | | Liên kết gốc, phiên bản, vị trí | Đánh dấu chưa xác minh, không phổ biến |
| Cổng sự thật | | Đối chiếu lấy mẫu, phạm vi dữ liệu | Xóa hoặc hạ mức khẳng định |
| Cổng quyền riêng tư/quyền hạn | | Phạm vi dữ liệu, sự đồng ý, nhật ký truy cập | Dừng xử lý và ẩn danh |
| Cổng chất lượng | | Tập đánh giá, mẫu biên, phản hồi thực tế | Sửa chữa, thu hẹp hoặc từ chối bàn giao |
| Cổng chi phí | | Token, thời gian, công sức làm lại thủ công và ngân sách | Hạ cấp mô hình hoặc dừng |
| Cổng cấp quyền công cụ | | Phạm vi công cụ, nhật ký gọi, ủy quyền đích danh và cách thu hồi | Cấm gọi hoặc quay lại xử lý thủ công |
| Cổng trách nhiệm | | Phê duyệt đích danh và nội dung công bố | Không công bố, không tự động thực thi |

Các quyết định quan trọng không thể chỉ do mô hình tạo sinh, hệ thống chấm điểm tự động hoặc một lập trình viên duy nhất tự phê duyệt. Trong các lĩnh vực rủi ro cao, hãy quay lại tài liệu nguồn hiện hành và chuyên gia có đủ năng lực.

## 6. Chi phí, lưu giữ và khả năng đảo ngược

```markdown
预计调用量、时间和费用上限：
人工审阅与返工预算：
数据是否进入训练、日志或第三方留存：
可接受延迟与降级方案：
可以撤回、重跑或恢复到哪个版本：
发布范围与灰度对象：
```

Một lần gọi rẻ tiền nếu gây ra sự cố quyền riêng tư, quyết định sai hoặc khối lượng làm lại lớn thì chi phí thực tế không hề rẻ. Ngoài chi phí mô hình, hãy ghi lại thời gian của con người, công việc thẩm định, thất bại, chạy lại và trao đổi.

## 7. Thất bại, tạm dừng và khôi phục

| Điều kiện kích hoạt | Hành động ngay lập tức | Thông báo cho ai | Vị trí khôi phục/hoàn tác |
| --- | --- | --- | --- |
| Không tìm thấy nguồn hoặc phiên bản | Dừng phổ biến, quay lại tài liệu gốc | | |
| Không đạt cổng bắt buộc của tập đánh giá | Cấm công bố hoặc tự động thực thi | | |
| Đầu vào vượt qua ranh giới quyền hạn | Dừng tải lên, thu hồi quyền truy cập | | |
| Chi phí/độ trễ vượt quá giới hạn | Hạ cấp, giới hạn lưu lượng hoặc dừng | | |
| Người dùng thực tế báo cáo tổn hại | Gỡ xuống, lưu giữ bằng chứng, chuyển cấp xử lý | | |

Nếu chưa có người chịu trách nhiệm dừng, quy trình thông báo và phiên bản có thể sử dụng đã biết, thì vẫn chưa sẵn sàng tích hợp vào quy trình thực tế.

## 8. Bàn giao và thông tin công khai

```markdown
当前状态：未开始 / 实验 / 内部试用 / 灰度 / 已交付 / 已停止
已完成与证据位置：
未决问题和风险：
下一项最小任务：
交接负责人、时间和权限：
读者/用户需要知道的 AI 参与范围：
来源、隐私、版权和利益关系说明：
```

Người nhận bàn giao không nên phải lục tìm lịch sử trò chuyện mới biết bước tiếp theo. Văn bản công khai ít nhất phải nêu rõ công cụ đã tham gia vào bước nào, những sự thật nào đã được con người xác nhận và nội dung nào vẫn chỉ là đề xuất.

## 9. Kiểm tra trước khi bắt đầu

- [ ] Đối tượng thực tế, hành động, thời hạn và người phụ trách đã được ghi rõ;
- [ ] Các trường đầu vào, mức độ nhạy cảm, sự đồng ý, bản quyền và ranh giới lưu giữ đã được xác nhận;
- [ ] Nguồn, phiên bản và điều kiện mất hiệu lực quan trọng có thể truy nguyên;
- [ ] Các mẫu thông thường, biên, mâu thuẫn và lịch sử đã ẩn danh đã được đưa vào tập đánh giá;
- [ ] Phạm vi những gì AI có thể và không thể làm đã được ghi rõ;
- [ ] Khi phù hợp, đã ghi lại các điểm kiểm tra của tác vụ dài, quy tắc an toàn khi thử lại/lặp lại, ranh giới nhập liệu trên trình duyệt và lối ra mạng;
- [ ] Các cổng kiểm tra thủ công, giới hạn chi phí, điều kiện dừng và vị trí hoàn tác đã được chỉ định;
- [ ] Việc bàn giao, công bố và ngày rà soát tiếp theo đã được xác định.