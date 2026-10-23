---
title: "Học mọi thứ cùng AI: từ vấn đề thực tế đến sản phẩm bàn giao có thể kiểm chứng"
description: Dựa trên những thất bại trong sản phẩm, quá trình phục hồi và việc quay lại thực hành AI của Hàn Tiên Khải, xây dựng một vòng khép kín gồm vấn đề, đường cơ sở, bài tập, sản phẩm bàn giao, kiểm chứng và tổng kết dành cho người học phổ thông.
updated: 2026-10-15
sources_checked: 2026-10-15
source_review_interval: 60
---

# Học mọi thứ cùng AI: từ vấn đề thực tế đến sản phẩm bàn giao có thể kiểm chứng

Tôi tên là Hàn Tiên Khải, còn được gọi là Lí Phả. Nhiều người biết đến tôi trước tiên qua việc học tiếng Anh, sau đó đọc về câu chuyện tôi làm phần mềm, mở cơ sở kinh doanh ăn uống, trải qua thất bại của công ty, mất cân bằng thể chất và cuộc sống, rồi quay lại với công nghệ và AI. Ngày nay, tôi thích xem AI như một hạ tầng học tập hơn là một nút bấm suy nghĩ thay mình.

Phương pháp này bắt nguồn từ một sự thật không mấy dễ chịu: câu trả lời có thể rất đầy đủ, nhưng sản phẩm lại có thể không có người dùng; mã nguồn có thể chạy được, nhưng dữ liệu và bảo mật lại có thể không có nền tảng; một người có thể tỏ ra rất thông minh trong cuộc trò chuyện, nhưng sau khi đóng cuộc trò chuyện lại không thể tự mình hoàn thành nhiệm vụ. Kết quả học tập thực sự phải vẫn tồn tại sau khi AI rời đi: bạn có thể giải thích, phán đoán, hoàn thành, chuyển giao và để lại bằng chứng mà người khác có thể kiểm tra.

Khi cần biến một lần cộng tác với AI thành một nhiệm vụ lặp lại, hãy đọc tiếp [Thực hành quy trình làm việc với AI](../practice/ai-workflows.md); khi chuẩn bị so sánh các phiên bản hoặc bàn giao ra bên ngoài, hãy dùng [Nhật ký đánh giá AI](../../templates/ai-evaluation.md) để lưu lại thất bại, chỉnh sửa thủ công và chi phí.

Trước những công cụ mới liên tục xuất hiện, bạn có thể đọc trước [Xu hướng AI và lộ trình học tập](6-ai-trends-and-learning-roadmap.md): phân biệt năng lực đã quan sát được, tuyên bố của nhà cung cấp và dự đoán của chính mình, rồi chọn một thay đổi đáng để kiểm chứng. Bạn không cần chạy theo mọi lần phát hành; điều cần thiết là dần hình thành tiêu chuẩn lựa chọn của riêng mình.

## Tóm tắt chương

- Trước tiên xác định kết quả thực tế, rồi mới quyết định AI tham gia vào bước nào;
- Dùng đường cơ sở không có AI, phiên bản có hỗ trợ và bài kiểm tra độc lập sau một khoảng trì hoãn để phân biệt học tập với làm thay;
- Ghi nguồn, quyền hạn, quyền riêng tư, chi phí và trách nhiệm vào phạm vi nhiệm vụ;
- Khi kết thúc phiên làm việc, lưu trạng thái để lần làm việc sau không phụ thuộc vào trí nhớ của cuộc trò chuyện.

## Trước hết hãy hiểu phương pháp này bắt nguồn từ đâu

Nội dung dưới đây là ghi chép cá nhân của tác giả, không phải kết luận nghiên cứu, cũng không phải lời bảo đảm thành công cho tất cả mọi người. Mỗi trường hợp được đọc theo bốn bước: chuyện gì đã xảy ra, lúc đó đã phán đoán sai ở đâu, hình thành nguyên tắc nào, hôm nay có thể thực hiện bài tập gì.

Nếu muốn phân tích một bài báo công khai, một trải nghiệm dự án AI hoặc ghi chép thất bại của chính mình, bạn có thể sao chép trước [Mẫu tổng kết trải nghiệm AI](../../templates/ai-case-review.md), tách riêng nguồn, sự kiện, phán đoán, kết quả và nguyên tắc có thể chuyển giao. Mẫu không thể thay bạn chứng minh kết quả, nhưng có thể ngăn câu chuyện vô tình biến thành kết luận.

### 2015–2016: Từ chốn không còn nơi để đi đến người dùng thực tế

Tôi từng quay về quê vì gặp trắc trở trong việc thực tập và hoàn tất thủ tục tốt nghiệp. Năm 2016, tôi bắt đầu mày mò làm một website phim `bt0.com`, sau đó nhận các dự án thiết kế website. Đó không phải một sản phẩm vĩ đại, nhưng có người dùng thực tế, phản hồi thực tế và dấu vết sử dụng thực tế.

Sai lầm dễ mắc nhất khi ấy là xem “mình có thể viết ra” đồng nghĩa với “người khác cần nó”. Điều thực sự làm thay đổi phán đoán không phải là học thêm một công nghệ, mà là có người sử dụng, đánh giá, thậm chí rời đi chỉ vì một chi tiết nào đó.

**Nguyên tắc**: Học tập bắt đầu từ vấn đề thực tế; sản phẩm bộc lộ thiếu sót rõ hơn những câu trả lời được lưu trữ.

**Bài tập hôm nay**: Chọn một vấn đề mà người xung quanh thực sự gặp phải. Trước tiên không dùng AI để viết một trang phương án giải quyết; hãy ghi lại đối tượng, hành động, tiêu chuẩn hoàn thành và ba điều bạn chưa biết.

### 2017–2022: Từ tái cấu trúc frontend đến những ràng buộc của tổ chức và sản phẩm

Năm 2017, tôi gia nhập một công ty phần mềm phục vụ luật sư và công ty luật, từ một lập trình viên frontend bình thường trở thành trưởng bộ phận, tổng giám đốc rồi đối tác. Sản phẩm thời kỳ đầu xuất phát từ các dự án gia công, yêu cầu thay đổi liên tục; sau đó tôi phụ trách tái cấu trúc bằng Vue, nhưng sau khi sản phẩm phát hành, trong một thời gian dài vẫn không có đơn hàng.

Trải nghiệm này giúp tôi hiểu rằng nỗ lực, tái cấu trúc và số lượng tính năng đều không thể thay thế việc quản trị nhu cầu, kiểm chứng người dùng và phối hợp nhóm. Một người học được cách viết mã không có nghĩa là tổ chức đã học được cách bàn giao sản phẩm.

**Nguyên tắc**: Mục tiêu học tập phải được viết thành nhiệm vụ thực tế, chứ không phải “tìm hiểu một chủ đề”; mỗi bước đều phải có đối tượng và tiêu chuẩn nghiệm thu.

**Bài tập hôm nay**: Viết lại “học quản lý sản phẩm” thành “trong 45 phút, viết một bản tóm tắt yêu cầu dài một trang cho một người dùng thực tế và để người đó chỉ ra một giả định không đứng vững”.

### 2022: Nhầm tìm kiếm và kết quả định sẵn với AI

Năm 2022, doanh số phần mềm sụt giảm nghiêm trọng. Chỉ sau khi người bạn học cùng bàn thời trung học tham gia, chúng tôi mới nhận ra cấu trúc dự án đã lỗi thời, hiệu năng và bảo mật tồn tại vấn đề; cái gọi là năng lực “dữ liệu lớn” và “AI” cũng không thực sự có bộ dữ liệu hay nền tảng huấn luyện, một số tính năng về bản chất chỉ là tìm kiếm và trả về kết quả định sẵn.

Chúng tôi dành rất nhiều công sức cho UI, khả năng thích ứng đa nền tảng và việc chồng thêm tính năng, nhưng lại không xác nhận trước năng lực cốt lõi và dữ liệu có thực sự tồn tại hay không. Cuối cùng công ty giải thể; thua lỗ và cảm giác day dứt không thể biến mất nhờ một màn trình diễn đẹp mắt hơn.

**Nguyên tắc**: Hiệu quả trình diễn không đồng nghĩa với năng lực, câu trả lời của mô hình không đồng nghĩa với sự thật, tốc độ tạo ra không đồng nghĩa với chất lượng bàn giao. Những kết luận quan trọng phải quay về nguồn, kiểm thử, người dùng và người chịu trách nhiệm.

**Bài tập hôm nay**: Yêu cầu AI tạo lời giải thích về một chủ đề quen thuộc; sau đó không xem lại lịch sử trò chuyện, tự viết ra nguồn, phản ví dụ, điểm chưa biết và một phép thử có thể bác bỏ nó. Phần nào không viết được chính là lỗ hổng học tập.

### 2023: Sau thất bại, trước hết khôi phục khả năng hành động

Sau khi công ty thất bại, tôi đóng GitHub, rời khỏi nhiều nhóm, chìm đắm trong trò chơi, còn cơ thể và cuộc sống thì mất đi ranh giới. Sau khi về quê, bước đầu tiên thực sự không phải là mở một công ty khác, mà là ăn uống, ngủ nghỉ, ra ngoài, đối diện với quá khứ và thu nhỏ mọi việc xuống quy mô có thể hoàn thành trong ngày hôm nay.

**Nguyên tắc**: Hệ thống học tập phải tính đến năng lượng, sức khỏe và trách nhiệm thực tế. Việc thực hiện liên tục quan trọng hơn nỗ lực ngắn hạn; ngay cả trong giai đoạn sa sút cũng không nên lấy “hoàn thành một cuộc đảo ngược vĩ đại” làm tiêu chuẩn nghiệm thu.

**Bài tập hôm nay**: Chỉ sắp xếp 5–15 phút để hoàn thành một hành động có thể lưu lại: sắp xếp một trang ghi chú, chạy một bài kiểm thử, nghe một đoạn tài liệu hoặc viết ba câu; sau đó ghi lại tình hình hoàn thành thực tế, không dùng kế hoạch để che giấu việc chưa hành động.

### 2026: Quay lại với AI và các ngành công nghiệp thực

Năm 2026, với tư cách chủ tịch Công ty TNHH Điện toán đám mây Từ Nguyên Trung Quốc, tôi một lần nữa bước vào thực tiễn công nghệ, dịch vụ doanh nghiệp và các ngành công nghiệp thực, khám phá việc đưa AI vào những bối cảnh thực tế như nông nghiệp, lâm nghiệp, chăn nuôi và ngư nghiệp, đồng thời dự định cung cấp chương trình đào tạo cơ bản miễn phí cho các hợp tác xã nông thôn. Đây là định hướng thực hành và kế hoạch cá nhân, không phải doanh thu, số lượng khách hàng hay hiệu quả đã được chứng minh.

**Nguyên tắc**: Cuối cùng AI phải đi vào quy trình thực tế và chịu những ràng buộc về chi phí, quyền hạn, quyền riêng tư, phản hồi người dùng, sự cố và khả năng khôi phục.

**Bài tập hôm nay**: Chọn một vấn đề của một tổ chức thực tế, viết rõ dữ liệu đến từ đâu, ai có thể xem, kết quả thế nào được xem là đạt, thất bại thì dừng ra sao, và trách nhiệm thủ công nào bạn sẵn sàng đảm nhận.

## Vòng khép kín bảy bước: Làm việc trước, nói về prompt sau

1. **Xác định kết quả thực tế**: Viết rõ bối cảnh, đối tượng, hành động, thời hạn và tiêu chuẩn nghiệm thu.
2. **Lưu đường cơ sở không có AI**: Trước tiên tự mình làm một lần để bộc lộ lỗ hổng kiến thức và điểm mù phán đoán.
3. **Chuẩn bị tài liệu đáng tin cậy**: Ưu tiên tài liệu chính thức, giáo trình, bài nghiên cứu, dữ liệu, mã nguồn hiện có và trường hợp thực tế.
4. **Thiết kế bài tập hướng dẫn**: Để AI đặt câu hỏi, giải thích, so sánh, gợi ý và tạo bài tương tự, không thay thế các bước then chốt.
5. **Chủ động tạo sản phẩm**: Đóng tài liệu rồi tự giải thích, lập trình, viết, tính toán, trình diễn hoặc ra quyết định.
6. **Tiếp nhận phản hồi từ nhiều nguồn**: AI chỉ là một ý kiến; nguồn, kiểm thử, chuyên gia, người dùng và đánh giá an toàn cùng nhau đưa ra phán đoán.
7. **Cập nhật trạng thái**: Lưu sản phẩm, lỗi, chi phí, câu hỏi còn bỏ ngỏ và nhiệm vụ nhỏ nhất tiếp theo.

Thiếu bước 1, AI sẽ đóng gói mong muốn thành câu trả lời; thiếu bước 2, bạn không biết năng lực có tăng lên hay không; thiếu bước 6 và 7, lỗi sẽ lặp lại trong cuộc trò chuyện tiếp theo.

## Học AI, trước hết hãy hiểu năm tầng

“Dùng AI để học” và “học cách xây dựng ứng dụng AI” có thể thúc đẩy lẫn nhau, nhưng cần những bài tập khác nhau. Vế trước cần bảo vệ trước hết khả năng ghi nhớ, hiểu và diễn đạt của bản thân; vế sau còn phải giải thích dữ liệu đi vào hệ thống thế nào, công cụ thực thi ra sao và kết quả được kiểm chứng thế nào. Có thể dùng các tầng dưới đây để định vị vấn đề, không cần ngay từ đầu đã huấn luyện mô hình.

| Tầng | Cần giải thích bằng lời của mình | Một bài tập có thể để lại bằng chứng |
| --- | --- | --- |
| Mô hình và đầu ra | Câu trả lời chịu ảnh hưởng của đầu vào và quá trình tạo sinh; trôi chảy không đồng nghĩa với đúng sự thật | Tìm một câu trả lời sai cho một vấn đề quen thuộc, lưu lại bằng chứng phản bác |
| Ngữ cảnh và truy xuất | Ngữ cảnh là tài liệu được cung cấp trong lần này; truy xuất là tìm tài liệu liên quan rồi đưa cho mô hình | Dùng ba trang tài liệu công khai để trả lời câu hỏi, ghi rõ vị trí trong văn bản gốc cho từng kết luận |
| Cấu trúc và công cụ | Đầu ra phù hợp định dạng trường không có nghĩa dữ liệu trong trường là thật; đề xuất gọi công cụ không có nghĩa hành động đã hoàn thành | Kiểm tra ba trường hợp: thiếu trường, sai số và công cụ thất bại |
| Quy trình và đánh giá | Các bước, quyền hạn, xử lý thất bại và nghiệm thu cùng quyết định hệ thống có dùng được hay không | So sánh quy trình thủ công với quy trình AI, lưu lại thất bại và tổng thời gian |
| Học tập và chuyển giao | Chất lượng sản phẩm khi có công cụ và năng lực độc lập của bản thân phải được đánh giá riêng | Sau ba đến bảy ngày, thay đổi một điều kiện và làm lại mà không xem đáp án cũ |

Retrieval-Augmented Generation (RAG) thường đưa tài liệu được truy xuất vào trước khi trả lời; tinh chỉnh thì thay đổi tham số mô hình thông qua quá trình huấn luyện. Hai phương pháp này giải quyết những vấn đề khác nhau. Khi tài liệu đã được cập nhật, thiếu nguồn trích dẫn hoặc phạm vi truy xuất sai, trước hết cần kiểm tra tài liệu và việc truy xuất; không thể kỳ vọng tinh chỉnh tự động cung cấp sự thật mới nhất, tính xác thực của trích dẫn hoặc quyền thao tác. Trước tiên hãy có thể chỉ ra thất bại nằm ở tầng nào, rồi mới quyết định cần công nghệ gì.

Có thể tham khảo sự khác biệt giữa các khái niệm trên tại [Giải thích của IBM về RAG và tinh chỉnh](https://www.ibm.com/think/topics/rag-vs-fine-tuning) (phát hành ngày 2024-08-14, kiểm tra ngày 2026-10-15). Các bài tập và thứ tự kiểm tra trong bảng là thiết kế giảng dạy của hướng dẫn này, không phải sự bảo đảm của nguồn đó về hiệu quả học tập.

Độc giả không viết mã cũng có thể hoàn thành các bài tập này: quản lý tài liệu bằng thư mục, ghi lại quá trình bằng bảng tính, còn việc kiểm tra do chính mình hoặc độc giả thực tế thực hiện. Khi chuẩn bị bước vào phát triển, hãy học tiếp về giao diện, đầu ra có cấu trúc, gọi công cụ và kiểm thử; mỗi khi thêm một khái niệm, hãy để nó giải quyết một vấn đề đã gặp phải.

## Bản tóm tắt nhiệm vụ một trang

Trước tiên hãy sao chép đầy đủ [Bản tóm tắt nhiệm vụ AI](../../templates/ai-task-brief.md) vào thư mục dự án riêng tư của mình. Dưới đây là các trường tối thiểu; trước tiên hãy khử nhận dạng dữ liệu nhạy cảm, không trực tiếp đưa mật khẩu, giấy tờ tùy thân, hồ sơ khách hàng hoặc thông tin riêng tư của bên thứ ba cho mô hình dùng chung.

```markdown
# AI Task Brief

真实场景：
使用者/受众：
要完成的决策或动作：
截止时间：

已知事实与来源：
允许使用的文件：
数据敏感等级：公开 / 内部 / 机密 / 受限
明确不提供的材料：

最终交付物：
格式与长度：
验收标准：
必须由人确认的事项：

AI 可以做：
AI 不可以做：
人工审阅者：
失败时如何回滚或停止：
```

“Trải nghiệm tốt”, “kiến trúc tiên tiến”, “học được AI” đều không phải tiêu chuẩn nghiệm thu. Hãy viết thành một hành động có thể quan sát, chẳng hạn như “người dùng có thể hoàn thành một lần nhập dữ liệu trong vòng 10 phút và nhìn thấy một báo cáo lỗi có thể giải thích được”.

## Giao thức tối thiểu cho một phiên làm việc

Trước khi bắt đầu, yêu cầu AI chỉ nhắc lại phạm vi:

```text
请用不超过 8 条要点复述目标、受众、输入、验收标准、限制、未知项和你无法确认的内容。
列出准备使用的来源。没有来源的事实标记为待核验。
先不要生成最终交付，先指出最可能导致返工的 3 个风险。
```

Trong quá trình thực hiện, mỗi lần chỉ thúc đẩy một phần có thể kiểm tra:

```text
把任务拆成最小可验证切片。每次只推进一个切片，并说明输入、假设、改动、检查方式和下一步。
如果前提冲突，暂停并提问，不要悄悄替换需求。保留失败方案和原因。
```

Khi kết thúc, tạo bản cập nhật trạng thái thay vì một bản tổng kết bóng bẩy:

```text
根据本次实际完成内容输出：
1. 已完成与证据位置；
2. 已被来源、测试或人工确认的判断；
3. 仍会重复的错误、风险和未决问题；
4. 下一项最小任务、完成标准和需要的材料。
不要声称记得其他会话，也不要把推断写成事实。
```

## Các đầu ra khác nhau cần bằng chứng khác nhau

| Đầu ra | Bằng chứng tối thiểu | Bằng chứng mạnh hơn |
| --- | --- | --- |
| Giải thích | Nguồn gốc, thuật ngữ then chốt, điểm chưa chắc chắn | Nhắc lại khi không xem tài liệu, phản ví dụ, bài tập chuyển giao |
| Mã nguồn | Kết quả chạy, kiểm thử cơ bản | Kiểm thử biên, kiểm tra tĩnh, đánh giá bảo mật, mẫu thực tế |
| Nghiên cứu | Liên kết gốc của các sự kiện quan trọng | Kiểm chứng từ nhiều nguồn, phạm vi dữ liệu, ngày phát hành, phản ví dụ |
| Bản thảo | Đối tượng, mục đích, sự kiện, cấu trúc | Phản hồi của độc giả thực tế, lịch sử chỉnh sửa, so sánh phiên bản |
| Quyết định | Các phương án, giả định, chi phí, rủi ro | Thử nghiệm quy mô nhỏ, nhật ký quyết định, tổng kết sau sự việc |
| Giảng dạy | Mục tiêu học tập, kết quả bài tập | Chuyển giao độc lập, kiểm tra lại sau một khoảng trì hoãn, sự thay đổi của lỗi |

Đối với nội dung rủi ro cao, viết “chưa xác nhận” chuyên nghiệp hơn là biến một suy đoán trôi chảy thành sự thật.

## Ba lần đối chiếu: Chứng minh AI đã giúp gì

Dùng [Nhật ký học tập với AI](../../templates/ai-learning-log.md) để lưu lại ít nhất ba mẫu cho cùng một nhiệm vụ:

1. **Đường cơ sở không có AI**: Trước tiên tự mình hoàn thành, ghi lại thời gian, chất lượng, điểm vướng và mức độ tự tin;
2. **Phiên bản có AI hỗ trợ**: Chỉ để AI thực hiện phần việc đã thỏa thuận; ghi lại prompt, nguồn, các đề xuất được chấp nhận và từ chối, cũng như việc làm lại;
3. **Phiên bản độc lập sau một khoảng trì hoãn**: Sau 3–7 ngày, đóng cuộc trò chuyện và đáp án, thay đổi một điều kiện tương tự rồi tự hoàn thành lại.

| Kết quả đối chiếu | Cách giải thích thận trọng hơn |
| --- | --- |
| Cả phiên bản hỗ trợ và phiên bản độc lập đều tốt hơn | AI có thể đã cung cấp giàn giáo hữu ích, năng lực có cơ hội được lưu lại |
| Phiên bản hỗ trợ tốt hơn, phiên bản độc lập kém đi | Sản phẩm đã được cải thiện, nhưng các bước then chốt có thể đã bị thuê ngoài |
| Thời gian ngắn hơn, việc làm lại và lỗi nhiều hơn | Có được tốc độ nhưng tích lũy “món nợ tốc độ” |
| Mức độ tự tin cao hơn, độ chính xác sự thật không đổi hoặc giảm | Cần hiệu chỉnh sự tự tin trước, rồi mới tăng quyền hạn của công cụ |

Ít nhất hãy ghi lại năm mục: hoàn thành nhiệm vụ, chất lượng, khả năng độc lập, việc làm lại, chi phí và khả năng chuyển giao. Một lần đối chiếu không thể chứng minh quan hệ nhân quả, nhưng gần với phán đoán có thể kiểm tra hơn câu “cảm thấy AI rất hữu ích”.

## Những điểm thường mất kiểm soát và bàn giao

| Điểm mất kiểm soát | Tín hiệu tại hiện trường | Hành động ngay lập tức |
| --- | --- | --- |
| Bịa đặt sự thật | Không tìm thấy văn bản gốc, phiên bản hoặc vị trí dữ liệu | Tạm dừng truyền bá, quay lại nguồn cấp một và đánh dấu là chưa kiểm chứng |
| Trôi dạt yêu cầu | Câu trả lời ngày càng đầy đủ nhưng không còn trả lời nhiệm vụ ban đầu | Dán lại bản tóm tắt nhiệm vụ, yêu cầu liệt kê các xung đột và điểm chưa biết |
| Rò rỉ quyền riêng tư | Đầu vào chứa thông tin khách hàng, danh tính, y tế hoặc khóa bảo mật | Dừng tải lên, khử nhận dạng hoặc chuyển sang môi trường đã được phê duyệt |
| Hoàn thành giả | Mã chạy được nhưng không có kiểm thử biên; bài viết đọc được nhưng không có trích dẫn | Kiểm thử tối thiểu theo tiêu chuẩn nghiệm thu, không chấp nhận sự trôi chảy là hoàn thành |
| Phụ thuộc vào phiên trò chuyện | Rời khỏi cuộc trò chuyện là không thể giải thích bước tiếp theo | Ghi kết quả vào [Nhật ký học tập với AI](../../templates/ai-learning-log.md) và [Trạng thái học tập](../../templates/learning-state.md) |

Khi bàn giao, ít nhất hãy lưu: mục tiêu hiện tại, phần đã hoàn thành và vị trí bằng chứng, các sự kiện vẫn chưa được xác nhận, lỗi và rủi ro, chi phí, nhiệm vụ nhỏ nhất tiếp theo và điều kiện dừng/khôi phục. Cửa sổ trò chuyện chỉ là không gian làm việc tạm thời, không phải kho lưu trữ duy nhất của dự án.

## Từ học tập đến bàn giao dự án

Khi nhiệm vụ bước vào dự án mã nguồn hoặc dự án nhóm, hãy thêm ba cánh cửa:

- **Có thể giải thích**: Không có lịch sử trò chuyện, người phụ trách vẫn có thể giải thích các quyết định then chốt và giới hạn;
- **Có thể kiểm thử**: Đầu vào thực tế, trường hợp biên, quyền hạn và đường đi khi thất bại đều được kiểm tra;
- **Có thể khôi phục**: Khi xuất hiện rủi ro dữ liệu, nhà cung cấp gián đoạn hoặc chất lượng giảm, biết ai sẽ tạm dừng, thông báo thế nào và khôi phục ra sao.

Thư mục dự án có thể sử dụng:

```text
00-brief/       任务简报和验收标准
01-baseline/    无 AI 样本和初始测试
02-sources/     原始资料、许可和来源索引
03-working/     草稿、实验和提示词
04-output/      可交付版本、录音或构建产物
05-feedback/    用户反馈和错误分类
06-decisions/   决策日志和未决问题
07-operations/  权限、监控、部署和回滚
learning-state.md
```

## Dữ liệu, quyền riêng tư và bản quyền

| Cấp độ | Ví dụ | Cách xử lý mặc định |
| --- | --- | --- |
| Công khai | Tài liệu đã phát hành, mã nguồn công khai, dữ liệu công khai | Kiểm tra nguồn và giấy phép trước khi sử dụng |
| Nội bộ | Kế hoạch chưa phát hành, quy trình, nhật ký không nhạy cảm | Chỉ dùng công cụ được tổ chức phê duyệt, giới hạn thành viên và thời gian lưu giữ |
| Mật | Thông tin khách hàng, hợp đồng, chiến lược kinh doanh, lỗ hổng chưa công bố | Không tải lên nếu chưa được phê duyệt rõ ràng; ưu tiên xử lý cục bộ hoặc khử nhận dạng |
| Hạn chế | Khóa bảo mật, dữ liệu danh tính/y tế, dữ liệu trẻ em, quyền riêng tư của bên thứ ba | Không đưa vào mô hình dùng chung, tuân thủ chính sách tổ chức và pháp luật áp dụng |

Xóa tệp không đồng nghĩa với xóa lịch sử, liên kết chia sẻ, bản xuất, bộ nhớ đệm và bản sao lưu. Bài viết công khai cũng có thể chứa thông tin cá nhân; trước tiên hãy xác nhận quyền cho phép, phạm vi tối thiểu cần thiết và thời hạn xóa.

## 7 ngày, 30 ngày, 12 tuần

### 7 ngày: Hoàn thành một sản phẩm bàn giao nhỏ có thể tái lập

- Viết bản tóm tắt nhiệm vụ và tiêu chuẩn nghiệm thu;
- Lưu đường cơ sở không có AI;
- Dùng vòng khép kín bảy bước để hoàn thành một sản phẩm bàn giao trong 1–3 giờ;
- Lưu nguồn, prompt, kiểm thử, phản hồi và cập nhật trạng thái;
- Viết lại AI đã giúp gì, đã dẫn sai điều gì và sau khi bỏ AI bạn vẫn có thể làm được gì.

### 30 ngày: Xây dựng một quy trình làm việc lặp lại

- Hoàn thành bốn vòng khép kín cho các nhiệm vụ cùng loại;
- So sánh thời gian, chất lượng, việc làm lại, chi phí và năng lực độc lập;
- Xóa những bước không thể cải thiện kết quả;
- Thực hiện một lần tổng kết thất bại, thay vì chỉ trình bày các trường hợp thành công.

### 12 tuần: Bàn giao cho người dùng hoặc tổ chức thực tế

- Cứ mỗi 2–4 tuần, mời đối tượng thực tế phản hồi;
- Hoàn thành kiểm tra về sự thật, kiểm thử, an toàn, quyền riêng tư, bản quyền, chi phí và bàn giao;
- Xuất tài liệu và trạng thái, viết một trang tổng kết và quyết định cho chu kỳ tiếp theo;
- Khi bằng chứng chưa đủ, thu hẹp vấn đề, thay đổi đối tượng hoặc dừng lại; không dùng thêm prompt để che giấu thiếu sót.

Đưa kết quả của ba lần đối chiếu và kết quả theo chu kỳ vào [Bảng tổng hợp hành động 90 ngày](../../templates/90-day-cycle.md), mỗi chu kỳ tiếp theo chỉ thay đổi một biến.

## Giải thích về nguồn và kiểm chứng

- **Trải nghiệm cá nhân**: Chủ yếu lấy từ [Câu chuyện của tôi](../part-2/my-story.md), [Chương khởi nghiệp](../part-2/entrepreneurship.md) và [Dự án của tác giả và thực tiễn đời sống](../../projects.md), thuộc ghi chép cá nhân của tác giả, không phải quy luật phổ quát.
- **Thông tin sản phẩm**: Sử dụng các trang trợ giúp chính thức được liệt kê trong [Học tiếng Anh cùng AI](../part-1/7-ai.md); tính năng, khu vực và gói dịch vụ có thể thay đổi.
- **Tình hình dự án**: Trung tâm Điện toán đám mây Từ Nguyên Trung Quốc, `token.love`, các bài viết công khai và kế hoạch về ngành công nghiệp thực đều có liên quan lợi ích hoặc phạm vi cần kiểm chứng, không thể xem là đánh giá độc lập hay bằng chứng về doanh thu.
- **Ngày kiểm chứng gần nhất**: 2026-10-15. Tính năng sản phẩm và tình hình dự án vẫn cần được kiểm tra lại trước khi sử dụng thực tế; các nguồn khái niệm AI mới được bổ sung trong lần này xem ở phần nội dung chính và đăng ký quy thuộc.

## Lời kết: Giữ năng lực ở lại trong con người

Điều AI dễ tạo ra nhất không chỉ là những câu trả lời sai, mà còn là cảm giác hoàn thành quá sớm. Lời giải thích rất trôi chảy, mã nguồn có thể chạy được, kế hoạch đã được sắp xếp, nên chúng ta tưởng rằng vấn đề đã thực sự được hiểu. Nhưng tốc độ xuất hiện của câu trả lời thường nhanh hơn tốc độ hình thành phán đoán.

Nếu một lần học tập đáng để tiếp tục, khi kết thúc nó nên để lại những thứ mà lịch sử trò chuyện không thể mang đi: một câu hỏi chính xác hơn, một nguồn có thể truy xuất, một lần kiểm thử thất bại, một phán đoán đã được bằng chứng thay đổi, một sản phẩm người khác có thể sử dụng, và một người sau khi đóng công cụ vẫn biết phải tiếp tục thế nào.

Học tập không phải là để AI thay bạn đi đến đích, mà là nhờ nó đưa bạn đến những nơi vốn không thể nhìn thấy, rồi tự mình xác nhận dưới chân mình là gì. Đóng cửa sổ, giải thích cho một người thực tế, hoàn thành bước tiếp theo và chịu trách nhiệm về kết quả. Nếu năng lực có thể theo bạn rời khỏi cuộc trò chuyện, thì nó mới thực sự ở lại.