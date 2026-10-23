---
title: Học AI, phát triển dự án và khởi nghiệp ở tầng tài nguyên
description: Ghi lại lộ trình kỹ thuật, bàn giao, vận hành và kiểm chứng kinh doanh của Han Xiankai, từ học AI, phát triển có AI hỗ trợ đến khởi nghiệp ở tầng tài nguyên AI, đồng thời phân biệt sự thật, thực hành và kết quả chưa biết.
updated: 2026-10-16
sources_checked: 2026-10-16
source_review_interval: 60
---

# Học AI, phát triển dự án và khởi nghiệp ở tầng tài nguyên

Tôi tên là Han Xiankai, còn được gọi là Lý Phổ. Nhiều người biết đến tôi trước tiên qua việc học tiếng Anh, rồi sau đó đọc những ghi chép của tôi về khởi nghiệp phần mềm, thất bại, phục hồi và bắt đầu lại. Hiện nay, tôi công khai thân phận chủ tịch của Công ty TNHH Điện toán Đám mây Từ Nguyên Trung Quốc, đồng thời đặt phần thực hành tiếp theo của cuộc đời vào một câu hỏi cụ thể hơn: **Khi AI trở thành năng lực nền tảng, một người bình thường làm thế nào để đi từ người học đến người xây dựng, rồi trở thành một doanh nhân ở tầng tài nguyên?**

Đây không phải câu chuyện “dùng AI để làm giàu dễ dàng”, cũng không phải cam kết về lợi nhuận. Đây là một bản đồ công việc đang được thực tế kiểm chứng: việc nào đã xảy ra, phương pháp nào có thể tái sử dụng, kết quả kinh doanh nào vẫn phải để người dùng thật, chi phí thật, sự cố thật và thời gian thật trả lời. Khi công ty thất bại vào năm 2022, tôi đã tận mắt chứng kiến cách những tính năng “trông giống AI” che giấu các vấn đề về dữ liệu, kiến trúc và trách nhiệm; những nguyên tắc kiểm soát ngày nay chính là kết quả được hình thành từ thất bại đó.

Các nguyên tắc kỹ thuật và kinh doanh trong chương này có thể được cụ thể hóa hơn qua một thử nghiệm nhỏ về [kiểm chứng khách hàng](../practice/customer-discovery.md), [vận hành bền vững](../practice/sustainable-business.md), [quy trình làm việc AI](../practice/ai-workflows.md) và [đánh giá độ tin cậy](../practice/ai-evaluation.md).

## Trước hết, hãy tách biệt sự thật, thực hành và kết quả

- **Đã xảy ra**: Tôi đảm nhiệm chức vụ chủ tịch tại Công ty TNHH Điện toán Đám mây Từ Nguyên Trung Quốc; hiện tại, trang web chính thức mô tả `token.love` là cổng thông minh AI thống nhất hướng đến các doanh nghiệp và bối cảnh doanh nghiệp–chính phủ, đồng thời liệt kê các năng lực kết nối mô hình, định tuyến và khắc phục thảm họa, đo lường mức sử dụng, lưu vết kiểm toán và triển khai riêng tư/ngoại tuyến.
- **Đang thực hành**: Tôi sử dụng AI để học kiến thức mới, phân rã yêu cầu, phát triển dự án, viết kiểm thử, sắp xếp tài liệu và hoàn thành bàn giao; đồng thời đưa những kinh nghiệm này trở lại kiểm chứng trong bối cảnh đội nhóm và doanh nghiệp.
- **Chưa được kiểm chứng**: Khách hàng có tiếp tục trả phí hay không, dịch vụ có thể mở rộng quy mô hay không, kinh tế đơn vị có đứng vững hay không, sự thay đổi của nhà cung cấp có thể kiểm soát hay không, và doanh thu có đủ bù đắp rủi ro hay không.

Nếu sự thật, nhận định và mong muốn bị trộn lẫn, bài viết khởi nghiệp sẽ biến thành quảng cáo; tách chúng ra mới có khả năng trở thành một bản tổng kết. Khi chuẩn bị phân tích một trải nghiệm công khai, có thể sử dụng [mẫu tổng kết trường hợp trải nghiệm AI](../../templates/ai-case-review.md), trước hết ghi rõ nguồn và sự thật, rồi mới bàn đến nhận định và khả năng chuyển giao.

## Thất bại năm 2022 đã thay đổi các nguyên tắc kiểm soát ngày nay như thế nào

Vấn đề khi đó không phải là không viết mã, mà là chưa chứng minh trước năng lực cốt lõi, tập dữ liệu, hiệu năng, bảo mật và giá trị người dùng. UI, khả năng tương thích đa nền tảng và các kết quả được thiết lập sẵn khiến sản phẩm trông hoàn chỉnh, nhưng không thể trả lời “dữ liệu đến từ đâu”, “kết quả được kiểm chứng như thế nào” và “ai chịu trách nhiệm khi thất bại”.

Vì vậy, hiện nay mỗi dự án AI đều bắt đầu bằng năm câu hỏi:

1. **Năng lực có thực sự tồn tại không**: đó là mô hình, truy xuất, quy tắc hay quy trình thủ công; không thể dùng từ ngữ tiếp thị để thay thế phần giải thích;
2. **Dữ liệu có được phép sử dụng không**: nguồn, quyền cấp phép, mức độ nhạy cảm, thời hạn lưu giữ và xóa dữ liệu đã rõ ràng chưa;
3. **Kết quả được nghiệm thu như thế nào**: mẫu kiểm thử, điều kiện biên, việc rà soát thủ công và tiêu chuẩn của người dùng thực là gì;
4. **Chi phí có thể được bù đắp không**: chi phí mô hình, mạng, kỹ thuật, hỗ trợ, làm lại, tuân thủ và sự cố đã được ghi vào sổ sách chưa;
5. **Khi thất bại thì rút lui như thế nào**: ai có thể tạm dừng, hạ cấp, chuyển đổi, thông báo, khôi phục và tổng kết.

Nếu năm câu hỏi này chưa có câu trả lời, hành động tối thiểu không phải là tiếp tục thêm tính năng, mà là thu hẹp vấn đề và thực hiện một thử nghiệm có thể bác bỏ giả thuyết.

## I. Từ người học đến người xây dựng

Trước đây, tôi từng hiểu việc học tiếng Anh là “ghi nhớ nhiều hơn”, sau này mới nhận ra rằng đích đến của việc học không phải là sưu tầm câu trả lời, mà là có thể độc lập hoàn thành nhiệm vụ. Việc học AI cũng vậy: kết quả thực sự có giá trị không phải là mô hình đưa ra câu trả lời dài đến đâu, mà là sau khi đóng cuộc trò chuyện, tôi có thể giải thích các quyết định quan trọng, chạy chương trình, đối mặt với lỗi và bàn giao sản phẩm hay không.

Hiện nay, tôi sử dụng một vòng khép kín trong công việc:

1. **Đặt ra vấn đề thực tế**: viết rõ ai đang gặp vấn đề gì và kết quả nào mới được xem là hoàn thành;
2. **Thiết lập đường cơ sở không dùng AI**: tự mình thực hiện một lần trước, làm lộ khoảng trống kiến thức, các ràng buộc và điểm mù trong phán đoán;
3. **Chuẩn bị tài liệu đáng tin cậy**: cung cấp tài liệu chính thức, dữ liệu, mã hiện có, chính sách của tổ chức và ranh giới rủi ro;
4. **Để AI hỗ trợ phân rã**: so sánh phương án, tạo các thử nghiệm nhỏ, giải thích giả thuyết, không thuê ngoài phán đoán cuối cùng;
5. **Chủ động phát triển và kiểm chứng**: dùng AI hỗ trợ tạo nguyên mẫu, lập trình, tái cấu trúc, kiểm thử, viết tài liệu và gỡ lỗi;
6. **Tiếp nhận phản hồi từ nhiều nguồn**: kiểm thử, người dùng thực, chuyên gia lĩnh vực, tài liệu nguồn và rà soát an toàn cùng đưa ra phán đoán;
7. **Lưu trạng thái và bằng chứng**: ghi lại việc đã hoàn thành, lỗi, chi phí, quyết định và nhiệm vụ tối thiểu tiếp theo.

Vòng khép kín này liên kết với [dùng AI để học mọi thứ](1-ai-learning.md), nhưng phát triển dự án có thêm một yêu cầu cứng: **mọi quyết định quan trọng đều phải có khả năng được kiểm thử, giải thích hoặc khôi phục**.

## II. Phát triển dự án bằng AI: sau tốc độ vẫn phải có chất lượng

AI có thể tạo ra mã trông hoàn chỉnh chỉ trong vài phút, cũng có thể lan truyền lỗi ra toàn bộ dự án chỉ trong vài phút. Cách làm của tôi không phải là để AI thay thế nhà phát triển, mà là biến nó thành một cộng tác viên có tần suất cao, có thể chất vấn và bắt buộc phải trải qua nghiệm thu.

### 2.1 Bản tóm tắt dự án

Mỗi dự án trước tiên tạo một trang `task-brief.md`:

```markdown
# Task Brief

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

“Trải nghiệm tốt”, “kiến trúc tiên tiến” hay “mức độ thông minh hóa cao” không phải là tiêu chuẩn nghiệm thu. Hãy viết tiêu chuẩn thành những hành động có thể quan sát, chẳng hạn như “người dùng có thể hoàn thành một lần nhập dữ liệu và xem báo cáo lỗi trong vòng 10 phút”.

### 2.2 Chuỗi phát triển có thể rà soát

| Giai đoạn | AI có thể hỗ trợ | Con người phải xác nhận |
| --- | --- | --- |
| Yêu cầu | Sắp xếp người dùng, bối cảnh, giới hạn và vấn đề | Vấn đề có thực hay không, tiêu chuẩn hoàn thành có thể quan sát hay không |
| Phương án | Đề xuất kiến trúc, giao diện và thử nghiệm tối thiểu | Ranh giới dữ liệu, phụ thuộc, chế độ thất bại và chi phí dài hạn |
| Nguyên mẫu | Tạo trang, giao diện, tập lệnh và dữ liệu mẫu | Có giải quyết nhiệm vụ cốt lõi hay chỉ trình diễn hiệu quả |
| Triển khai | Hoàn thiện mã, giải thích thay đổi, tạo kiểm thử | Logic quan trọng, quyền hạn, xử lý ngoại lệ và khả năng bảo trì |
| Kiểm tra | Chạy kiểm thử, kiểm tra tĩnh, kiểm tra hiệu năng và bảo mật | Kiểm thử có bao phủ rủi ro thực tế hay không, kết quả có thể tái hiện hay không |
| Bàn giao | Sắp xếp tài liệu, các bước triển khai, nhật ký thay đổi và phương án khôi phục | Người dùng có thể sử dụng không, đội nhóm có thể tiếp quản không, vấn đề có thể truy xuất không |

Mỗi lần chỉ thúc đẩy một lát cắt logic, không trộn lẫn yêu cầu, tái cấu trúc, định dạng và nâng cấp phụ thuộc vào nhau. Chỉ khi giữ lại một đường cơ sở không dùng AI, một sản phẩm thực sự có thể chạy và một nhật ký lỗi/chỉnh sửa, ta mới có thể phân biệt tốc độ với năng lực.

### 2.3 Cổng kiểm soát mã và phát hành

```text
这是任务简报和当前代码结构。先不要写代码。
提出两个最小实现方案，比较需求覆盖、改动范围、依赖、失败模式、测试难度、数据/权限风险和迁移成本。
明确缺失信息和推断。最后只推荐一个 1–2 小时可验证的切片。
```

Trước khi phát hành, ít nhất phải lưu lại: số phiên bản, tóm tắt thay đổi, các bước di chuyển, chỉ số giám sát, điều kiện kích hoạt khôi phục, người phụ trách và thông báo cho người dùng. Rà soát mã theo mức độ nghiêm trọng, kiểm tra sai lệch yêu cầu, mất dữ liệu, vượt quyền, chèn mã, điều kiện tranh chấp, xử lý ngoại lệ, hiệu năng, khả năng bảo trì và khoảng trống kiểm thử.

Sau mỗi lần thử nghiệm hoặc phát hành, hãy điền [phiếu chấm điểm dự án AI](../../templates/ai-project-scorecard.md), đồng thời giữ lại đường cơ sở không dùng AI, phiên bản có AI hỗ trợ và lần kiểm thử độc lập sau một khoảng trễ; nếu thiếu ba mẫu này, không thể phán đoán công cụ mang lại năng lực, làm thay hay công việc phải làm lại.

## III. Tầng tài nguyên AI là gì

Mô hình là tầng năng lực, ứng dụng là kết quả mà người dùng nhìn thấy; giữa hai bên còn cần một tầng cơ sở hạ tầng giúp năng lực có thể được kết nối, kiểm soát, đo lường và vận hành bền vững. Tôi gọi tầng này là **tầng tài nguyên AI**.

Nó không chỉ là “bán một giao diện mô hình”, mà là sắp xếp các mô hình, tài khoản, năng lực tính toán, ranh giới dữ liệu và quy trình tổ chức phân tán thành một dịch vụ mà đội nhóm có thể hiểu, sử dụng và quản trị.

Khi việc gọi công cụ và điều phối tác nhân trở nên phổ biến, tầng tài nguyên còn phải xử lý khả năng tương tác và ranh giới cấp quyền. [Đặc tả MCP (2026-07-28)](https://modelcontextprotocol.io/specification/2026-07-28) định nghĩa tài nguyên, lời nhắc và công cụ thành các năng lực kết nối có thể kết hợp, đồng thời hỗ trợ mã định danh tác vụ dài hạn tùy chọn; nhưng nó không thay hệ thống hoàn thành việc rà soát an toàn. Trước khi kết nối bất kỳ máy chủ bên ngoài nào, vẫn cần liệt kê phạm vi dữ liệu, quyền ghi, sự đồng ý của người dùng, nhật ký gọi và đường lui. Giao thức làm giảm chi phí kết nối lặp lại, chứ không làm giảm chi phí trách nhiệm. Về thực hành, có thể dùng cổng cấp quyền của [quy trình làm việc AI](../practice/ai-workflows.md) và bản ghi quy trình/kết quả của [đánh giá AI](../practice/ai-evaluation.md) để kiểm chứng trong phạm vi nhỏ trước.

### 3.1 Bản đồ năng lực

| Năng lực tầng tài nguyên | Vấn đề khách hàng gặp phải | Bằng chứng tối thiểu có thể kiểm chứng |
| --- | --- | --- |
| Kết nối và định tuyến đa mô hình | Hoạt động kinh doanh phụ thuộc vào một nhà cung cấp, chi phí chuyển đổi cao | Quy tắc định tuyến và nhật ký so sánh hai mô hình trên cùng một nhiệm vụ |
| Danh tính, quyền hạn và hạn ngạch | Không rõ ai được sử dụng, được dùng bao nhiêu, khi có vấn đề không thể truy xuất | Ma trận vai trò, chính sách hạn ngạch, mẫu nhật ký kiểm toán |
| Đo lường, chi phí và thanh toán | Có thể sử dụng nhưng không biết đội nhóm và dự án đã tốn bao nhiêu | Báo cáo chi phí theo đội nhóm/dự án/lần gọi và quy trình đối soát |
| Triển khai và vận hành | Dịch vụ không thể vào mạng và môi trường được tổ chức phê duyệt | Danh sách triển khai, khác biệt môi trường, nhật ký diễn tập khôi phục |
| Quan sát và xử lý sự cố | Không thể giải thích độ trễ, lỗi và biến động chất lượng | Nhật ký yêu cầu, phân loại lỗi, cảnh báo và nhật ký xử lý |
| Ranh giới dữ liệu và tuân thủ | Không rõ dữ liệu nhạy cảm đi đâu, được lưu giữ bao lâu và phê duyệt thủ công thế nào | Sơ đồ luồng dữ liệu, quy tắc lưu giữ, bằng chứng phê duyệt và xóa |
| Tích hợp hệ thống và hỗ trợ | Năng lực không thể đi vào quy trình kinh doanh, khi có vấn đề không biết tìm ai | Nghiệm thu tích hợp, lịch trực, phiếu hỗ trợ và tài liệu bàn giao |

Đối với khách hàng, giá trị không nằm ở việc “có thêm một tên mô hình”, mà là giảm tích hợp lặp lại, giảm chi phí mất kiểm soát, giảm gián đoạn khi chuyển đổi nhà cung cấp, đồng thời có thêm một giao diện trách nhiệm mà tổ chức có thể hiểu và quản lý.

### 3.2 Vòng đời của một yêu cầu

Kiến trúc tham khảo không phải cam kết sản phẩm, nhưng mọi dịch vụ ở tầng tài nguyên đều phải giải thích được một yêu cầu lưu chuyển như thế nào:

**Xác thực danh tính → Quyền hạn và hạn ngạch → Kiểm tra dữ liệu → Quyết định định tuyến → Gọi mô hình → Lọc kết quả → Ghi nhận đo lường → Giám sát và cảnh báo → Bàn giao cho người dùng**

Mỗi bước đều phải trả lời: ai chịu trách nhiệm, ghi lại điều gì, khi thất bại thì xử lý thế nào, dữ liệu được lưu bao lâu, có thể phát lại hoặc xóa hay không. Chỉ chuyển tiếp giao diện mà không có đo lường, quyền hạn, nhật ký, hạ cấp và kiểm toán thì không thể trở thành dịch vụ doanh nghiệp đáng tin cậy.

### 3.3 Định tuyến không phải là “chọn mô hình mạnh nhất”

Chiến lược định tuyến nên lấy nhiệm vụ và các ràng buộc làm trung tâm:

- Với nhiệm vụ rủi ro thấp, tần suất cao và cấu trúc ổn định, ưu tiên xem xét chi phí và độ trễ;
- Với nhiệm vụ cần suy luận phức tạp hoặc ngữ cảnh dài, so sánh chất lượng, giới hạn ngữ cảnh và tỷ lệ thất bại;
- Với nhiệm vụ liên quan đến dữ liệu nhạy cảm, trước tiên xem xét phạm vi được phê duyệt, vị trí triển khai và chính sách nhật ký;
- Khi nhà cung cấp gặp sự cố, thực hiện hạ cấp, thử lại, chuyển đổi hoặc bàn giao cho con người;
- Mỗi thay đổi định tuyến đều phải ghi lại phiên bản, lý do, mẫu và phương thức khôi phục.

Nếu “mạnh nhất” nhưng không ổn định, không thể kiểm toán hoặc có chi phí không thể chịu đựng, đó chưa chắc là mô hình phù hợp nhất.

## IV. Công ty Từ Nguyên Trung Quốc và token.love: một lộ trình kinh doanh đang được thực hành

Công ty TNHH Điện toán Đám mây Từ Nguyên Trung Quốc là công ty nơi tôi hiện đảm nhiệm chức vụ chủ tịch. Hiện tại, trang web chính thức mô tả `token.love` là cổng thông minh AI thống nhất hướng đến các doanh nghiệp và bối cảnh doanh nghiệp–chính phủ, đồng thời liệt kê các năng lực kết nối mô hình, định tuyến và khắc phục thảm họa, đo lường mức sử dụng, lưu vết kiểm toán và triển khai riêng tư/ngoại tuyến. Đây là định vị sản phẩm trên trang chủ chính thức, không đại diện cho sự chứng thực của bất kỳ tổ chức bên thứ ba nào, cũng không thay thế tài liệu chính thức, phê duyệt tuân thủ, hợp đồng hay hoạt động rà soát an toàn của chính khách hàng.

Nhìn từ tầng tài nguyên, lộ trình kinh doanh này có thể được tách thành:

**Tài nguyên mô hình và năng lực tính toán → Kết nối và định tuyến thống nhất → Quyền hạn, đo lường và quản trị → Tích hợp hệ thống doanh nghiệp → Vận hành bảo trì và dịch vụ liên tục**

Sản phẩm thực sự phải giúp khách hàng biết: năng lực đến từ đâu, chi phí phát sinh thế nào, dữ liệu đi qua đâu, khi xảy ra sự cố ai xử lý, và lần di chuyển tiếp theo còn lựa chọn hay không. Năng lực cụ thể, khu vực khả dụng, gói dịch vụ, phạm vi tuân thủ và cam kết dịch vụ phải căn cứ vào mô tả chính thức và thỏa thuận bằng văn bản của [token.love](https://token.love/).

## V. Thử nghiệm doanh nghiệp: trước tiên giải quyết một vấn đề có thể nghiệm thu

### 5.1 Giai đoạn khám phá

Trong lần trao đổi đầu tiên, đừng vội trình diễn mô hình. Trước tiên hãy hỏi:

- Quy trình hiện tại là gì, bước nào chậm nhất hoặc dễ xảy ra lỗi nhất;
- Ai đang gánh chi phí này, xảy ra bao lâu một lần, lỗi sẽ gây ảnh hưởng gì;
- Dữ liệu nào có thể sử dụng, dữ liệu nào tuyệt đối không được rời khỏi ranh giới tổ chức;
- Khách hàng đã có tài khoản, hợp đồng, mạng, quyền hạn và yêu cầu an toàn nào;
- Nếu thử nghiệm thành công, ai sẽ tiếp tục sử dụng, phê duyệt và trả phí;
- Kết quả nào sẽ khiến khách hàng nói rõ “tiếp tục”, kết quả nào sẽ khiến hai bên dừng lại.

Đầu ra là một trang tóm tắt vấn đề, không phải một trang tuyên ngôn chung chung về giá trị AI.

### 5.2 Giai đoạn thử nghiệm

Một thử nghiệm đạt yêu cầu phải có: phạm vi, mẫu, mục tiêu ngoài phạm vi, ranh giới dữ liệu, người phụ trách, thời gian, tiêu chuẩn nghiệm thu, điều kiện rút lui khi thất bại và giới hạn chi phí. Trước thử nghiệm, hãy lưu đường cơ sở của quy trình cũ: thời gian thủ công, tỷ lệ lỗi, thời gian chờ, số lần làm lại, chi phí hiện tại và mức độ hài lòng của người dùng.

Trong thời gian thử nghiệm, đồng thời ghi lại quy trình mới: lần gọi mô hình, định tuyến, độ trễ, lỗi, việc tiếp quản thủ công, giờ hỗ trợ, bất thường dữ liệu, công việc làm lại và phản hồi người dùng. Chỉ ghi lại “đã tạo ra bao nhiêu nội dung” thì không thể chứng minh hoạt động kinh doanh được cải thiện.

Dùng [phiếu chấm điểm dự án AI](../../templates/ai-project-scorecard.md) để đăng ký điều kiện kiểm thử, chi phí, hiệu quả độc lập và cổng kiểm soát đưa vào vận hành theo từng phiên bản, tránh tình trạng sau khi thử nghiệm kết thúc chỉ còn lại một buổi trình diễn.

### 5.3 Nghiệm thu và bàn giao

Trước khi bàn giao, hãy chia nghiệm thu thành bốn tầng:

1. **Chức năng**: Quy trình có thể hoàn thành hay không, lỗi có hiển thị rõ hay không;
2. **Chất lượng**: Đầu ra có đạt tiêu chuẩn nghiệp vụ hay không, khi bất thường có thể do con người tiếp quản hay không;
3. **An toàn**: Quyền hạn, nhật ký, lưu giữ dữ liệu, xóa dữ liệu và kiểm toán có được thông qua hay không;
4. **Vận hành**: Ai chịu trách nhiệm nâng cấp, sự cố, chi phí, chuyển đổi nhà cung cấp và hỗ trợ người dùng.

Gói bàn giao nên bao gồm sơ đồ kiến trúc, sơ đồ luồng dữ liệu, ma trận quyền hạn, mô tả biến môi trường, các bước triển khai, bảng điều khiển giám sát, lịch trực và đường dẫn nâng cấp, phương thức khôi phục, các vấn đề đã biết và ngày tổng kết tiếp theo.

## VI. Logic kiếm tiền: đảm nhận công việc có thể tính phí cho khách hàng

Kiếm tiền không phải là thay lớp vỏ cho tên mô hình rồi tăng giá, mà là đảm nhận cho khách hàng một phần công việc vốn đắt đỏ, phân tán hoặc khó quản lý. Những hình thức trao đổi giá trị có thể bao gồm:

- **Dịch vụ quản lý tài nguyên**: quản lý kết nối mô hình, hạn ngạch và chi phí theo lượt gọi, đội nhóm, dự án hoặc cấp độ dịch vụ;
- **Dịch vụ tích hợp và bàn giao**: kết nối với hệ thống hiện có của khách hàng, hoàn thành triển khai, quyền hạn, nhật ký và nghiệm thu;
- **Dịch vụ vận hành liên tục**: xử lý nâng cấp, sự cố, biến động chất lượng, chuyển đổi nhà cung cấp và hỗ trợ hằng ngày;
- **Dịch vụ quản trị và an toàn**: xây dựng quy trình về ranh giới dữ liệu, phê duyệt, kiểm toán, lưu vết và xử lý rủi ro;
- **Dự án tùy chỉnh và đào tạo**: hoàn thành phương án, nguyên mẫu, đưa vào vận hành và bàn giao đội nhóm xoay quanh vấn đề kinh doanh thực tế.

Đây không phải cam kết doanh thu, mà là các giao diện thu phí có thể kiểm chứng từng bước. Mỗi hạng mục đều phải trả lời: vì sao khách hàng sẵn sàng trả phí, kết quả được nghiệm thu thế nào, chi phí dịch vụ có thể được bù đắp lâu dài hay không.

### 6.1 Phương thức thu phí và bối cảnh áp dụng

| Giao diện thu phí | Phù hợp để giải quyết | Rủi ro chính | Bắt buộc ghi lại |
| --- | --- | --- | --- |
| Phí chẩn đoán/phương án một lần | Giúp khách hàng làm rõ quy trình, ranh giới và thử nghiệm | Sau khi bàn giao phương án không còn giá trị tiếp theo | Sản phẩm bàn giao, giờ công, tín hiệu chuyển đổi tiếp theo |
| Phí triển khai dự án | Tích hợp, triển khai, quyền hạn và nghiệm thu | Mỗi khách hàng đều phải tùy chỉnh lại, không thể sao chép | Phạm vi, thay đổi, công việc làm lại và dư địa lợi nhuận gộp |
| Phí sử dụng hoặc quản lý tài nguyên | Quản lý liên tục theo lượt gọi, dự án hoặc đội nhóm | Giá nhà cung cấp và mức sử dụng biến động | Lượt gọi, định tuyến, chi phí, đối soát và giới hạn |
| Phí thuê bao/cấp độ dịch vụ | Vận hành, hỗ trợ và quản trị liên tục | Cam kết dịch vụ vượt quá năng lực đội nhóm | Thời gian phản hồi, mức độ khả dụng, giờ hỗ trợ và ngoại lệ |
| Phí đào tạo và tư vấn | Giúp đội nhóm xây dựng năng lực sử dụng và quản trị | Học xong không sử dụng, khó quy kết hiệu quả | Mục tiêu khóa học, bài tập, chuyển giao và kiểm tra lại |

Hợp đồng thực tế phải căn cứ vào thỏa thuận chính thức giữa hai bên. Bài viết công khai chỉ thảo luận logic kinh doanh, không bịa đặt giá cả, lợi nhuận, số lượng khách hàng hay kết quả thu nhập.

### 6.2 Sổ chi phí

Khởi nghiệp ở tầng tài nguyên dễ chỉ nhìn vào nhu cầu mà không nhìn vào chi phí. Ít nhất phải ghi lại: mô hình và năng lực tính toán, mạng và lưu trữ, phát triển kỹ thuật, hỗ trợ khách hàng, bán hàng và thu hút khách hàng, tuân thủ và an toàn, bồi thường do sự cố, việc nhà cung cấp tăng giá, di chuyển, thuế phí và thời gian quản lý.

```text
贡献空间 = 客户收入
          - 模型与基础设施
          - 工程与支持
          - 获客与合规
          - 故障、返工与退款
```

Mỗi dự án phải tách riêng chi phí một lần và chi phí liên tục. Với dự án một lần, hãy xem xét hiệu suất bàn giao; với dịch vụ liên tục, hãy xem xét tỷ lệ duy trì, cường độ hỗ trợ, chi phí đơn vị và tín hiệu tiếp tục sử dụng. Nếu mỗi khách hàng mới chỉ làm tăng chi phí gọi, nhân lực và rủi ro, quy mô càng lớn thì thua lỗ có thể càng nhanh.

## VII. Vận hành: Không có sổ tay vận hành thì không có dịch vụ doanh nghiệp

### 7.1 Bảng điều khiển giám sát tối thiểu

- Số lượng yêu cầu, tỷ lệ thành công, loại lỗi và số lần thử lại;
- Phân bố độ trễ, thay vì chỉ xem giá trị trung bình;
- Chi phí theo mô hình, đội nhóm, dự án và nhiệm vụ;
- Vượt hạn ngạch, dữ liệu bất thường, từ chối quyền hạn và tiếp quản thủ công;
- Trạng thái nhà cung cấp, thay đổi định tuyến và thay đổi phiên bản;
- Phản hồi người dùng, giờ hỗ trợ và các vấn đề lặp lại.

Đây là các chỉ số vận hành được đề xuất, không có nghĩa là `token.love` hiện đã cung cấp đầy đủ mọi năng lực. Trước khi đưa vào vận hành, cần ghi chỉ số, người phụ trách, ngưỡng cảnh báo và chu kỳ lưu giữ vào hợp đồng dự án hoặc sổ tay vận hành nội bộ.

### 7.2 Phân cấp và xử lý sự cố

```text
发现 → 判断影响范围 → 暂停危险变更 → 降级/切换/人工接管
     → 通知受影响的人 → 保存日志与时间线 → 修复并验证
     → 复盘根因、成本和预防措施 → 更新运行手册
```

Sự cố nghiêm trọng ít nhất phải ghi lại: thời điểm phát hiện, dự án bị ảnh hưởng, thay đổi gần nhất, rủi ro dữ liệu, biện pháp tạm thời, trạng thái nhà cung cấp, thời điểm khôi phục, trao đổi với khách hàng, giả thuyết nguyên nhân gốc và bằng chứng khắc phục lâu dài. AI có thể hỗ trợ sắp xếp dòng thời gian, nhưng không thể thay thế người phụ trách sự cố.

### 7.3 Diễn tập chuyển đổi nhà cung cấp

Mỗi nhà cung cấp quan trọng ít nhất phải chuẩn bị: định tuyến dự phòng, mô hình hạ cấp, chiến lược giới hạn lưu lượng, bộ nhớ đệm hoặc quy trình thủ công, phương án di chuyển dữ liệu, đầu mối liên hệ theo hợp đồng và kiểm thử khôi phục. Mỗi quý thực hiện một lần diễn tập với một mẫu rủi ro thấp, để xác minh “có thể chuyển đổi” chứ không chỉ viết điều đó trong tài liệu.

## VIII. Ranh giới dữ liệu, an toàn và tuân thủ

| Mức độ dữ liệu | Ví dụ | Cách làm mặc định |
| --- | --- | --- |
| Công khai | Tài liệu đã phát hành, mã nguồn và dữ liệu công khai | Có thể sử dụng, kiểm tra nguồn và giấy phép |
| Nội bộ | Kế hoạch chưa phát hành, quy trình, nhật ký không nhạy cảm | Chỉ sử dụng công cụ được tổ chức phê duyệt, giới hạn thành viên và thời hạn lưu giữ |
| Mật | Thông tin khách hàng, hợp đồng, chiến lược kinh doanh, lỗ hổng chưa công bố | Không tải lên nếu chưa được phê duyệt rõ ràng, ưu tiên xử lý cục bộ hoặc khử nhận dạng |
| Hạn chế | Khóa bí mật, dữ liệu định danh/y tế, dữ liệu trẻ em, quyền riêng tư của bên thứ ba | Không đưa vào mô hình dùng chung, xử lý theo chính sách tổ chức và pháp luật áp dụng |

Dịch vụ tầng tài nguyên phải có khả năng trả lời: dữ liệu đi vào từ đâu, đi qua những nhà cung cấp nào, nhật ký nào sẽ được lưu, ai có thể xem, bao lâu thì xóa và chứng minh việc xóa như thế nào. Xóa một tệp không đồng nghĩa với xóa toàn bộ lịch sử, bộ nhớ đệm, bản xuất và bản sao lưu.

## IX. Lộ trình kiểm chứng trong mười hai tuần

| Thời gian | Vấn đề trọng tâm | Hành động | Bằng chứng bắt buộc phải lưu lại |
| --- | --- | --- | --- |
| Tuần 1–2 | Loại tổ chức nào có vấn đề cấp bách và cụ thể nhất? | Phỏng vấn, xem quy trình cũ, vẽ luồng dữ liệu | Biên bản phỏng vấn, đường cơ sở, ranh giới, điều kiện dừng |
| Tuần 3–5 | Sản phẩm tối thiểu có thể giảm chi phí tích hợp hoặc quản lý không? | Thiết lập sandbox, kết nối một nhiệm vụ, chạy kiểm thử đối chứng | Nguyên mẫu có thể chạy, kiểm thử, nhật ký thất bại, chi phí |
| Tuần 6–8 | Khách hàng có sẵn sàng tiếp tục sử dụng trong quy trình thực tế không? | Thử nghiệm phạm vi nhỏ, tiếp quản thủ công, tổng kết hằng tuần | Dấu vết sử dụng, sự cố, giờ hỗ trợ, hồ sơ an toàn |
| Tuần 9–10 | Việc bàn giao có thể được người khác sao chép không? | Diễn tập bàn giao, triển khai và khôi phục | Sổ tay vận hành, bảng quyền hạn, nghiệm thu bàn giao |
| Tuần 11–12 | Chi phí, chất lượng và thu phí có hình thành một tổ hợp hay không? | Tổng kết, thử nghiệm báo giá, thảo luận tiếp tục sử dụng | Sổ chi phí, báo giá, tín hiệu tiếp tục sử dụng, quyết định tiếp theo |

Khi bằng chứng không ủng hộ việc tiếp tục, hãy thu hẹp vấn đề, thay đổi khách hàng hoặc dừng phương án; khi bằng chứng ủng hộ việc tiếp tục, cũng phải bổ sung an toàn, hợp đồng, quyền hạn, giám sát và bàn giao trước khi nói đến mở rộng.

## X. Hai lát cắt thực hành từ các bài viết trên tài khoản công chúng: từ “trừu tượng” đến “từng khung hình”

Trên WeChat có hai bài viết liên quan đến tôi, lần lượt viết về AI từ góc độ quan sát nhân vật và tranh luận trên mạng. Chúng không phải là kiểm toán kỹ thuật, trường hợp khách hàng hay bằng chứng doanh thu; tôi xem chúng là tài liệu tường thuật công khai, mượn những hành động và ý thức về vấn đề trong đó để bổ sung cho lộ trình thực hành này.

### 10.1 Từ chối câu trả lời “có khả năng nhất” đầu tiên

Ngày 11 tháng 8 năm 2026, TokenMany đăng [《Han Xiankai: Con người “trừu tượng” nhất trong giới AI》](https://mp.weixin.qq.com/s?src=11&timestamp=1787503349&ver=6922&signature=hsfWcee*q*Okq4gsJ5TpMaWV4vZTwLean6SKtOxCC-EyAf9jWD6l1LQYDny29FqXVImHZFNFDPt*EVH*hVMN2pa91kZtuYfzI81wtV7yahnqVBsKS*c7Ls1uf9QqiEIF&new=1). Bài viết giải thích “trừu tượng” là không vội chấp nhận câu trả lời có sẵn, sẵn sàng để công nghệ, kinh doanh, bản tính con người và đời sống thường ngày soi chiếu lẫn nhau. Đây là quan sát mang tính văn học của tác giả về hình tượng nhân vật, không phải phép đo độc lập về năng lực.

Tôi chuyển phần có thể chuyển giao trong đó thành các hành động phát triển:

1. Trước tiên viết ra giả định mặc định, sau đó liệt kê ít nhất một cách giải thích ngược lại;
2. Nén liên tưởng liên ngành thành một thử nghiệm nhỏ có thể kiểm chứng trong 1–2 giờ;
3. Ghi lại quan sát nào xuất phát từ sự thật, quan sát nào chỉ là phép loại suy, trực giác hoặc giả thuyết chờ kiểm chứng;
4. Cho phép thử nghiệm bác bỏ ý tưởng đẹp đẽ của chính mình, đồng thời giữ lại các mẫu thất bại trong hồ sơ dự án.

Như vậy, “ý tưởng táo bạo” sẽ không dừng lại ở phong cách biểu đạt, mà trải qua định nghĩa vấn đề, nguyên mẫu tối thiểu, kiểm thử và tổng kết để biến thành bằng chứng có thể được người khác kiểm tra.

### 10.2 Biến sự huyên náo trở lại thành những vấn đề có thể trả lời

Ngày 21 tháng 8 năm 2026, Wanli Center thuộc Guận Tuyết Holdings đăng [《Han Xiankai và AI: Tách sự huyên náo thành cảm xúc từng khung hình》](https://mp.weixin.qq.com/s?src=11&timestamp=1787503349&ver=6922&signature=k7g1j*QF9lLWMGUlkAu65EFOmvokb8FoM51LNr4hgn4Q4Cc7q3t3O8Mkac7YnWTJbIVdvX-PXYdZXVHEohJieTOPR*Q2-TVAHuIg2ljgp2BMn8m7STrvovnpW01j817Y&new=1). Bài viết kể theo lối tường thuật rằng: giao từng bình luận cho AI phân loại, bên cạnh ghi lại “quan điểm, bằng chứng, cường độ cảm xúc, cách diễn đạt, mức độ có thể phản hồi”, đồng thời trước tiên xem “những lời chửi mắng” như “mẫu cảm xúc”. Đoạn văn này không thể chứng minh đã bàn giao một sản phẩm phân tích dư luận, cũng không thể chứng minh việc phân tích đã cải thiện kết quả thực tế; nó cung cấp một khung xử lý phản hồi đáng để thử nghiệm thận trọng.

Trong dự án thực tế, tôi sẽ thu hẹp khung này thành một quy trình có ranh giới:

| Bước | AI có thể hỗ trợ | Con người phải chịu trách nhiệm |
| --- | --- | --- |
| Thu thập | Loại trùng, phân cụm, đánh dấu chủ đề lặp lại | Xác nhận nguồn, quyền cấp phép, dữ liệu tối thiểu cần thiết và thời hạn xóa |
| Phân tách | Phân biệt phát biểu sự thật, suy đoán, từ ngữ cảm xúc và chiến lược biểu đạt | Phán đoán sự thật có bằng chứng hay không, tránh coi nhãn là kết luận |
| Sắp xếp | Tạo hàng đợi theo mức độ ảnh hưởng, khẩn cấp và khả năng phản hồi | Xác nhận mức ưu tiên, rủi ro và có cần chuyển sang xử lý thủ công hay không |
| Phản hồi | Tạo nhiều bản nháp có giọng điệu kiềm chế, hướng đến vấn đề cụ thể | Kiểm tra sự thật, quyền riêng tư, trách nhiệm và phạm vi công khai |
| Tổng kết | Tổng hợp thay đổi, hiểu lầm lặp lại và vấn đề chưa giải quyết | Quyết định có sửa sản phẩm, bổ sung giải thích, tạm dừng phản hồi hay dừng thử nghiệm |

Bình luận, phiếu hỗ trợ và phản hồi khách hàng đều có thể chứa thông tin cá nhân. Nếu chưa được cấp phép, không nên tải nguyên đoạn hội thoại, tên, thông tin liên hệ hoặc chi tiết có thể nhận dạng trực tiếp lên mô hình dùng chung; ngay cả khi dữ liệu là công khai, vẫn phải khử nhận dạng trước, hạn chế quyền truy cập và đặt thời hạn lưu giữ. AI có thể giúp xếp hàng tiếng ồn, nhưng không thể thay con người phán đoán ai đúng ai sai, càng không thể thay con người gánh trách nhiệm phản hồi công khai.

Điểm nhắc nhở chung mà hai bài viết này mang lại cho tôi là: sự sáng tạo chịu trách nhiệm đưa ra những lối vào khác nhau, còn bằng chứng quyết định có tiếp tục hay không; cảm xúc đáng được nhìn thấy, nhưng phải đi qua bộ lọc của sự thật, quyền riêng tư và trách nhiệm trước khi bước vào quy trình sản phẩm và doanh nghiệp.

## XI. Những nơi dễ mất kiểm soát nhất

- Coi đầu ra của mô hình là sự thật, coi hiệu quả trình diễn là chất lượng sản phẩm;
- Coi doanh thu từ một dự án một lần là một hoạt động kinh doanh bền vững;
- Chỉ tính chi phí API mà không tính thời gian hỗ trợ, làm lại, tuân thủ, bán hàng và quản lý;
- Tải dữ liệu khách hàng, bí mật công ty hoặc quyền riêng tư của bên thứ ba lên công cụ chưa được phê duyệt;
- Bị khóa vào một mô hình hoặc nhà cung cấp duy nhất nhưng không có phương án di chuyển, hạ cấp và xử lý sự cố;
- Cam kết thời gian phản hồi, mức độ khả dụng hoặc năng lực tuân thủ mà đội nhóm không thể cung cấp ổn định;
- Viết sản phẩm liên quan thành đánh giá độc lập, hoặc che giấu quan hệ thương mại đằng sau lời giới thiệu;
- Dùng thêm nhiều lời nhắc để che giấu vấn đề không có người dùng thật, chi phí thật và nghiệm thu thật.

Vì vậy, dự án này sẽ坚持 một số nguyên tắc đơn giản: nguồn có thể truy xuất, quan hệ lợi ích được công khai, kết quả có thể kiểm tra lại, rủi ro không được tô hồng, điều chưa biết phải được đánh dấu là chưa biết.

## 十二、Tôi muốn để lại điều gì

Nếu con đường này cuối cùng không trở thành một hoạt động kinh doanh đủ lớn, nó vẫn nên để lại ba loại điều:

1. Một phương pháp giúp tôi và đội ngũ học hỏi, phát triển nhanh hơn và vững vàng hơn;
2. Một loạt sản phẩm để người dùng thực sự có thể sử dụng, thử nghiệm và phê bình;
3. Một hồ sơ kinh doanh không xóa bỏ thất bại, để những người đến sau biết phán đoán nào từng phát huy tác dụng, còn phán đoán nào chỉ là kỳ vọng vào thời điểm đó.

Tôi vẫn muốn kiếm tiền, vì doanh thu là một bằng chứng cho thấy việc trao đổi giá trị có thể được duy trì; nhưng doanh thu không phải là giá trị duy nhất, cũng không phải kết cục có thể tuyên bố trước. Mục tiêu thành thật hơn lúc này là kết nối năng lực của AI với con người thực, tổ chức thực và trách nhiệm thực, rồi xem liệu nó có đáng để tiếp tục hay không.

## Nguồn và thuyết minh kiểm chứng

- **Kinh nghiệm cá nhân**: Dòng thời gian công ty phần mềm thất bại năm 2022, phục hồi năm 2023 và quay lại với AI năm 2026 được nêu trong[Câu chuyện của tôi](../part-2/my-story.md)và[Phần khởi nghiệp](../part-2/entrepreneurship.md).
- **Liên quan đến dự án**: Từ nguyên tiếng Trung, `token.love`, `ku0.com` và các bài viết trên tài khoản WeChat chính thức được nêu trong[Các dự án của tác giả và thực tiễn thực tế](../../projects.md), có mối liên hệ với tác giả, không phải đánh giá độc lập.
- **Kết luận kinh doanh**: Phương thức thu phí, sổ sách chi phí và lộ trình 12 tuần là những phương pháp đang chờ được kiểm chứng, không phải bằng chứng về doanh thu, số lượng khách hàng, lợi nhuận hay lợi tức đầu tư.
- **Kiểm chứng trang chính thức**: 2026-10-16. Trang chủ của `token.love` và `ku0.com` cùng các liên kết đến bài viết bên ngoài trong chương này đều có thể truy cập; năng lực sản phẩm cụ thể, phạm vi dịch vụ, khu vực, chính sách và cam kết trong hợp đồng vẫn cần được xác nhận lại trong dự án thực tế.

## Đưa phương pháp trở lại đời thường

Chương này không nên để độc giả mắc kẹt giữa tên sản phẩm, sơ đồ kiến trúc và giao diện thu phí. Điều thực sự nên được giữ lại là một tư thế làm việc chậm hơn nhưng thành thật hơn: nói rõ vấn đề, ghi rõ ranh giới, đưa từng lần chạy, từng khoản chi phí và từng thất bại trở lại vị trí có thể được kiểm tra.

Liệu dự án có thể tiếp tục hay không, cuối cùng vẫn phải do người dùng, đội ngũ, hợp đồng, thời gian và trách nhiệm cùng trả lời. Độc giả có thể trước tiên đến[Các dự án của tác giả và thực tiễn thực tế](../../projects.md)để đối chiếu mối liên hệ, trạng thái và ranh giới bằng chứng; cũng có thể trực tiếp chuyển đến[Phần IV: Thực hành và phục hồi](../part-4/practice-and-recovery.md), đưa những phán đoán ở đây trở lại một nhiệm vụ nhỏ, nhịp độ một tuần và một hành động có thể giúp bắt đầu lại.

Công nghệ giúp mở đường nhanh hơn không có nghĩa là con người đã đi đến đó. Thứ thực sự có thể đưa bạn qua chặng đường tiếp theo không phải là một màn trình diễn đẹp mắt, mà là chút năng lực giúp bạn sẵn lòng tiếp tục học hỏi, tiếp tục bàn giao trong điều kiện thực tế, đồng thời tiếp tục điều chỉnh.