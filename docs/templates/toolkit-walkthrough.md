---
title: "Thực hành với bộ công cụ: Giúp AI tiếp tục một quá trình học tập kéo dài 90 ngày qua nhiều phiên"
description: "Trình bày đầy đủ, qua một trường hợp học Python được đánh dấu rõ ràng là minh họa tổng hợp, cách bàn giao trạng thái học tập, bản tóm lược nhiệm vụ AI, đường cơ sở độc lập, sản phẩm, chuỗi bằng chứng, tổng kết hằng tuần và phản hồi của độc giả."
updated: 2026-09-02
---

# Thực hành với bộ công cụ: Giúp AI tiếp tục một quá trình học tập kéo dài 90 ngày qua nhiều phiên

Nhiều người không thiếu kế hoạch, mà không biết nên mở những bảng này vào lúc nào. Một vấn đề phổ biến khác là: khi một quá trình học kéo dài ba tháng, các phiên AI ngày càng dài; đến khi đổi sang phiên mới, trạng thái trước đó lại như biến mất hoàn toàn.

Giải pháp không phải là yêu cầu AI nhớ bạn mãi mãi. **Hãy để tệp lưu trạng thái, còn AI chỉ xử lý nhiệm vụ hiện tại.**

Trang này dùng một người học Python đang chuẩn bị chuyển nghề để trình bày đầy đủ. Nhân vật, nhiệm vụ, kết quả mã, điểm số và phản hồi đều là dữ liệu tổng hợp, chỉ nhằm minh họa cách điền, không phải thành quả thực tế của độc giả và cũng không thể chứng minh rằng 90 ngày chắc chắn đủ để chuyển nghề.

## Đây không phải là câu chuyện thành công

Người học trong phần minh họa có những điều kiện sau:

- Có thể đọc hiểu biến, điều kiện và vòng lặp đơn giản, nhưng không thể tự mình hoàn thành một chương trình nhỏ;
- Có thể ổn định dành 45 phút, bốn lần mỗi tuần;
- Mục tiêu trong 90 ngày là tự mình hoàn thành một công cụ dòng lệnh có thể đọc CSV, kiểm tra dữ liệu và xuất bản tóm tắt;
- Không tải dữ liệu công ty lên, không để AI viết thay sản phẩm cuối cùng, không thức đêm để bù cho thời gian gián đoạn;
- Nếu đến ngày thứ 14 vẫn không thể giải thích mã cốt lõi, sẽ không thêm framework hay khóa học mới.

Những điều kiện này chỉ là ranh giới của phần minh họa. Điểm xuất phát, thời gian, thể trạng, công việc và mục tiêu của bạn có thể hoàn toàn khác.

## Bối cảnh: Vì sao kế hoạch lại mất trí nhớ

Cách làm sai ban đầu là giữ mọi thứ trong một cửa sổ trò chuyện:

1. Yêu cầu AI lập kế hoạch 12 tuần;
2. Mỗi ngày đặt câu hỏi, luyện tập và sửa mã trong cùng một phiên;
3. Dựa vào phần ngữ cảnh phía trên để ghi nhớ lỗi, tiến độ và bước tiếp theo;
4. Khi ngữ cảnh quá dài, câu trả lời mới bắt đầu trộn lẫn các nhiệm vụ cũ;
5. Khi đổi phiên, lại dùng một đoạn hồi tưởng dài để giới thiệu lại bản thân.

Vấn đề không chỉ nằm ở độ dài ngữ cảnh. Lịch sử trò chuyện không có phiên bản ổn định, cũng không phân biệt rõ “sự việc đã hoàn thành”, “lời giải thích của AI” và “giả định cho lần sau”. Trạng thái học tập thực sự không nên bị mắc kẹt trong bất kỳ công cụ hay phiên trò chuyện nào.

## Năm công cụ, mỗi công cụ làm gì

| Công cụ | Vai trò trong trường hợp này | Không phụ trách việc gì |
| --- | --- | --- |
| [Trạng thái học tập](learning-state.md) | Lưu các sự kiện, bằng chứng, lỗi, giới hạn và nhiệm vụ tiếp theo xuyên suốt nhiều phiên | Không lưu từng câu trò chuyện |
| [Bản tóm lược nhiệm vụ AI](ai-task-brief.md) | Giới hạn nhiệm vụ 45 phút hiện tại, đầu vào, cách hỗ trợ và tiêu chí nghiệm thu | Không lập kế hoạch cho cả cuộc đời |
| [Chuỗi bằng chứng](evidence-chain.md) | So sánh đường cơ sở độc lập, phiên bản có hỗ trợ, bài kiểm tra lại sau một khoảng trễ và khả năng chuyển giao | Không dùng một điểm số để chứng minh “đã học được” |
| [Tổng kết hằng tuần](weekly-review.md) | Dựa trên bằng chứng trong một tuần để chỉ thay đổi một biến số | Không biến một trạng thái tồi tệ nhất thời thành kết luận về nhân cách |
| [Phản hồi thực hành của độc giả](reader-field-note.md) | Ghi lại liệu phương pháp này có thực sự đi vào hành động hay không, và điểm nào vẫn chưa biết cách sử dụng | Không yêu cầu công khai thông tin riêng tư hoặc chấm điểm cuốn sách |

Nếu lần đầu sử dụng bộ công cụ, trước hết hãy làm theo trang này trong một tuần, đừng mở tất cả các mẫu còn lại cùng lúc.

## Bước một: Đưa trạng thái ra ngoài phiên trò chuyện

Trước tiên, người học tạo `python-learning-state.md`, thay vì coi phiên AI là bộ nhớ:

```markdown
# Learning State — python-90d-v1

更新日期：2026-09-02
九十天场景：独立交付一个 CSV 摘要命令行工具，并能解释输入校验、错误处理和测试。
当前基线：能写变量、if 和 for；不能独立读取 CSV、拆函数或写测试。
可用容量：周一、周三、周五、周日各 45 分钟。
已有证据：baseline/day-01.py；运行后在空值行报错。
反复错误：先看答案；把能运行误认为能解释；修改多个变量后无法判断原因。
边界：不用真实公司数据；先提交自己的版本；不在 23:00 后补课。
当前阶段：第 1–14 天校准。
下一项最小任务：读取一份 12 行合成 CSV，跳过空行，输出有效行数与总金额。
完成标准：独立版能运行；我能解释每个函数；至少保存一个失败测试。
停止条件：45 分钟结束即保存状态，不用熬夜完成。
```

Tệp trạng thái chỉ giữ lại những nội dung có thể làm thay đổi hành động lần sau. Các trích đoạn khóa học, toàn bộ cuộc trò chuyện và mọi chi tiết của từng lần thử được đặt trong thư mục bằng chứng, không nhồi vào trang trạng thái.

## Bước hai: Mỗi lần chỉ giao cho AI một nhiệm vụ

Khi bắt đầu phiên mới, không yêu cầu AI “nhớ tôi”. Chỉ gửi trạng thái mới nhất và bản tóm lược nhiệm vụ lần này:

```markdown
下面是我的学习状态文件。请先用不超过 6 条要点复述版本、目标、当前证据、主要错误、边界和下一任务，指出冲突或缺口。不要补写文件里没有的事实。

本次只做一项任务：读取合成 CSV，跳过空行，输出有效行数与总金额。
流程：先让我提交独立版；你最多指出 3 个影响结果的问题，不直接给完整代码；我修改后，再用两个测试检查。45 分钟结束时，输出“完成、证据、错误/风险、交接、下一步”五项更新。
```

Công việc đầu tiên của AI là nhắc lại trạng thái, không phải lập tức giảng bài. Nếu phần nhắc lại có sai sót, trước hết hãy sửa trạng thái hoặc lời nhắc, đừng tiếp tục tạo kế hoạch dựa trên tiền đề sai.

## Bước ba: Làm đường cơ sở trước, rồi mới yêu cầu hỗ trợ

Phiên bản độc lập trong phần minh họa tổng hợp cho kết quả sau:

| Điều kiện | Kết quả | Bằng chứng |
| --- | --- | --- |
| 25 phút, không xem đáp án | Có thể đọc các dòng hợp lệ; giá trị tiền trống gây ra lỗi; toàn bộ logic nằm trong một hàm | `evidence/week-01/baseline.py` |
| AI chỉ ra ba vấn đề | Nhận diện việc kiểm tra giá trị trống, trách nhiệm của hàm và phần kiểm thử còn thiếu | `evidence/week-01/feedback.md` |
| Sau khi sửa | Vượt qua bài kiểm tra với dòng hợp lệ và dòng trống; vẫn chưa xử lý định dạng tiền tệ không hợp lệ | `evidence/week-01/revision.py` |

Đây không phải là “AI đã giúp tôi viết xong chương trình”. Cách ghi chép chính xác hơn là: phiên bản độc lập làm lộ ra ba vấn đề, AI giúp phân loại, người học sửa được hai vấn đề, còn vấn đề thứ ba được đưa vào nhiệm vụ tiếp theo.

Nếu ngay từ đầu đã yêu cầu toàn bộ mã, tệp cuối cùng có thể đẹp hơn, nhưng sẽ mất đường cơ sở và không thể biết phần năng lực nào thuộc về người học.

## Bước bốn: Đưa sản phẩm vào chuỗi bằng chứng

Trong tuần đầu tiên, đừng lưu kết luận kiểu “đã học CSV”, mà hãy ghi lại bốn thời điểm:

| Thời điểm | Điều kiện | Kết quả tổng hợp | Vẫn chưa thể nói lên điều gì |
| --- | --- | --- | --- |
| Đường cơ sở | Không có AI, 25 phút | Đạt 1/3 tiêu chí nghiệm thu | Không thể chứng minh đã hiểu xử lý lỗi |
| Sau khi được hỗ trợ ngay lập tức | Đã xem ba phản hồi | Đạt 2/3, có thể giải thích hai hàm | Không thể chứng minh vài ngày sau vẫn viết được |
| Kiểm tra lại sau một khoảng trễ vào ngày thứ 7 | Không xem mã cũ, đổi sang một tệp CSV có cùng cấu trúc | Đạt 2/3; lại bỏ sót giá trị tiền tệ không hợp lệ | Không thể chứng minh có thể xử lý trường mới |
| Chuyển giao | Thêm trường `currency` | Có thể xác định vị trí cần thay đổi, chưa hoàn thành kiểm tra loại tiền tệ | Cho thấy cấu trúc bắt đầu được chuyển giao, nhưng kiến thức nền còn thiếu |

Kết quả này không đạt điểm tối đa, nhưng cung cấp nhiều thông tin hơn “đã kiên trì một tuần”. Biến số tiếp theo không phải là thêm pandas, framework web và cơ sở dữ liệu, mà là chuyên tâm luyện tập kiểm tra đầu vào và kiểm thử thất bại.

## Bước năm: Tiếp tục trong phiên mới

Cuối tuần, phần tổng kết chỉ ghi lại vào tệp trạng thái những nội dung làm thay đổi quyết định:

```markdown
# Learning State — python-90d-v2

更新日期：2026-09-08
已完成：CSV 正常行与空行处理；拆成 read_rows / summarize 两个函数。
证据：week-01/baseline.py；revision.py；day-07-retest.py；tests.md。
延迟结果：第 7 天仍能完成 2/3 条件；非法金额校验再次失败。
主要错误：错误路径缺少测试；看到正常输出后过早停止检查。
保留边界：合成数据；先独立作答；45 分钟停止；不补做错过时长。
下一项最小任务：先写三个失败测试，再实现 parse_amount。
完成标准：空值、字母、负数三类输入都有明确结果；能口头解释设计选择。
下一次复查：2026-09-15。
```

Có thể đóng phiên cũ. Phiên mới chỉ cần `v2` và vị trí của các bằng chứng liên quan, không cần dán hàng chục nghìn chữ trong cuộc trò chuyện. **AI không theo dõi việc học xuyên suốt các phiên; tệp trạng thái hoàn thành việc theo dõi, còn AI đọc và phục vụ tệp đó.**

## Bước sáu: Điền phản hồi của độc giả sau bảy ngày

Phần minh họa tổng hợp cũng cần kiểm tra: bản thân bộ công cụ có giúp thúc đẩy hành động hay không.

```markdown
进入问题：不知道新 AI 会话怎样继续三个月计划。
实际行动：建立版本化学习状态；完成一项 CSV 小任务；保存独立版与复测。
七天后留下：可以不看原会话写出状态 v2，并在新会话继续一个明确任务。
迁移失败：知道要保存错误，却仍不知道怎样给错误分类。
最有帮助：五张工具的职责表和状态文件示例。
仍然抽象：阶段门槛需要更多不同目标的示例。
不能推出：这套流程能保证九十天后达到就业要求。
```

Phản hồi này trước tiên được lưu trong ghi chú riêng tư. Chỉ sau khi xóa đường dẫn, danh tính và nội dung nhạy cảm mới cân nhắc gửi phiên bản công khai.

## Nếu bị gián đoạn trong một tuần

Tệp trạng thái không yêu cầu bạn bù lại toàn bộ kế hoạch. Bước đầu tiên sau khi gián đoạn là ghi lại sự việc:

```markdown
中断事实：七天没有练习。
原因证据：两次加班；一次身体不适；没有完成复测。
不做的事：不把四次课程压进周末，不用熬夜偿还。
回归动作：运行上次测试，写一个失败用例，更新状态文件。
24 小时完成标准：保存失败测试和下一次 25 分钟入口。
```

Nếu sức khỏe, an toàn, trách nhiệm công việc hoặc các mối quan hệ cần được ưu tiên xử lý, việc khôi phục nhịp học cũng có thể trở thành kết quả của tuần đó. Kế hoạch phục vụ cuộc sống, không yêu cầu cuộc sống phải xin lỗi kế hoạch.

## Giao thức phiên trò chuyện bạn có thể sao chép trực tiếp

```markdown
1. 先复述我提交的状态版本、目标、证据、错误、边界和下一任务。
2. 指出冲突与缺失，不推测未写明的历史。
3. 本次只处理一项最小任务，先让我提交独立版。
4. 反馈最多三个影响结果的问题，区分观察、解释和建议。
5. 除非我明确请求，不直接给完整答案。
6. 结束时输出：完成、证据、错误/风险、交接、下一步。
7. 所有长期状态以文件为准，不声称记得其他会话。
```

Giao thức này không thể đảm bảo AI không bao giờ mắc lỗi. Nó giúp lỗi dễ được phát hiện hơn, đồng thời giúp người học giữ quyền sở hữu đối với vấn đề, trạng thái và mọi phán đoán cuối cùng.

## Phần minh họa này chứng minh điều gì, và vẫn chưa chứng minh điều gì

Nó cho thấy năm công cụ có thể tạo thành một quy trình bàn giao rõ ràng: trạng thái được lưu bên ngoài phiên, nhiệm vụ được thu hẹp, phiên bản độc lập và phiên bản có hỗ trợ được tách riêng, có kiểm tra lại sau bảy ngày, và phiên mới có điểm bắt đầu đáng tin cậy.

Nó chưa chứng minh rằng:

- Nhân vật tổng hợp này sẽ kiên trì trong 90 ngày;
- Độ khó của nhiệm vụ này phù hợp với mọi người mới bắt đầu;
- Học bằng AI chắc chắn nhanh hơn học không dùng AI;
- Hoàn thành một công cụ dòng lệnh đồng nghĩa với việc có năng lực làm việc thực tế;
- Kết quả của một tuần có thể đại diện cho khả năng chuyển giao dài hạn.

Khi thực sự áp dụng, hãy giữ lại đường cơ sở, sản phẩm, thời gian, chi phí và thất bại của chính bạn. Ví dụ chỉ có nhiệm vụ giải thích cách điền; thực tế mới quyết định nó có hữu ích hay không.

## Lời kết: Giao việc ghi nhớ cho tệp, giữ quyền phán đoán cho chính mình

Một quá trình học tập dài hạn không nên đánh mất quá khứ chỉ vì cửa sổ trò chuyện bị đóng, cũng không nên giả vờ có tính liên tục chỉ vì cửa sổ trò chuyện rất dài.

Hãy để tệp trạng thái ghi nhớ những sự việc đã xảy ra, để bằng chứng lưu lại các phiên bản bạn thực sự tạo ra, và để phiên tiếp theo chỉ đảm nhận bước tiếp theo. Công cụ có thể thay đổi, mô hình có thể được cập nhật, kế hoạch cũng có thể được thu nhỏ. Chỉ cần bạn vẫn biết mình đã đi từ đâu, điều gì chưa được chứng minh và nhiệm vụ tiếp theo nằm ở đâu, việc học sẽ không bị mắc kẹt trong bất kỳ cuộc trò chuyện nào.

Lối vào liên quan: [Trạng thái học tập](learning-state.md) ｜ [Bản tóm lược nhiệm vụ AI](ai-task-brief.md) ｜ [Chuỗi bằng chứng](evidence-chain.md) ｜ [Phản hồi thực hành của độc giả](reader-field-note.md)