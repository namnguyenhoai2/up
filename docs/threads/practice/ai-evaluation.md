---
title: "Đánh giá và độ tin cậy của AI: Biết khi nào có thể đưa vào sử dụng"
description: So sánh quy trình AI bằng các nhiệm vụ thực tế, tập kiểm thử nhỏ, phân loại lỗi và tổng chi phí để nhận ra sự khác biệt giữa một lần thành công và khả năng sử dụng ổn định.
updated: 2026-10-16
sources_checked: 2026-10-16
source_review_interval: 60
---

# Đánh giá và độ tin cậy của AI: Biết khi nào có thể đưa vào sử dụng

Một lần thành công trong bản trình diễn khó trả lời câu hỏi “người dùng tiếp theo có thể hoàn thành suôn sẻ hay không”. Đánh giá có tác dụng làm lộ ra thất bại trước khi đưa vào sử dụng, đồng thời giúp bạn xác định một thay đổi cụ thể thực sự đã cải thiện điều gì.

Chương này tiếp nối [quy trình AI](ai-workflows.md), tập trung vào một câu hỏi cụ thể: với cùng một nhiệm vụ, con người, quy trình hiện tại và quy trình ứng viên, bên nào có thể cung cấp kết quả đạt yêu cầu với chi phí chấp nhận được? Các mẫu nhỏ và ngưỡng trong phần này được thiết kế cho mục đích giảng dạy, không phải chứng nhận để đưa vào vận hành, cũng không đại diện cho tất cả người dùng.

## Bắt đầu từ nhiệm vụ để định nghĩa thế nào là đạt yêu cầu

Đừng chỉ hỏi “câu trả lời có tốt không”. Hãy viết ra hành động mà người sử dụng cần thực hiện tiếp theo, cũng như những thất bại không thể chấp nhận. Ví dụ, khi tổng hợp tài liệu về một sự kiện công khai, kết quả đạt yêu cầu phải giúp người đọc tìm được văn bản gốc, phân biệt điều đã biết với điều chưa biết, và không biến thời gian đã hết hạn thành lịch trình hiện tại.

Chia việc kiểm tra thành hai tầng:

- **Các điều kiện bắt buộc phải đạt toàn bộ**: nguồn phải có thật, các con số quan trọng phải chính xác, không làm lộ tài liệu bị hạn chế, không thực hiện thao tác chưa được cấp phép. Không thể dùng điểm văn phong để bù cho thất bại.
- **Chất lượng có thể so sánh**: bố cục có rõ ràng không, có dễ đọc không, số lần chỉnh sửa và tổng thời gian mất bao lâu. Chỉ so sánh các khác biệt này sau khi đã đáp ứng tầng đầu tiên.

Phải viết sẵn tiêu chuẩn trước khi có kết quả kiểm thử. Việc tạm thời nới lỏng tiêu chuẩn sau khi thấy phiên bản ứng viên thất bại chỉ khiến cuộc đánh giá trở thành cách biện hộ cho phương án thay thế.

## Xây dựng một tập kiểm thử nhỏ nhưng đa dạng

Lấy mẫu từ các nhiệm vụ thực tế mà bạn chuẩn bị phục vụ, xin phép sử dụng tài liệu và loại bỏ những thông tin không cần thiết. Lần đầu có thể chọn mười trường hợp: bốn đầu vào phổ biến, hai trường hợp thiếu mục, hai đầu vào xung đột hoặc đã hết hạn, một trường hợp công cụ thất bại và một trường hợp tài liệu có kèm chỉ dẫn thao tác. Đây chỉ là tỷ lệ thuận tiện để bắt đầu; điều quan trọng là bao phủ các lỗi có hậu quả khác nhau.

| Loại trường hợp | Muốn quan sát điều gì | Ví dụ về hành vi đạt yêu cầu |
| --- | --- | --- |
| Nhiệm vụ phổ biến | Năng lực cơ bản có đủ không | Kết quả đáp ứng yêu cầu về định dạng và sự thật |
| Thiếu thông tin | Có tự bịa ra sự thật không | Đánh dấu phần còn thiếu, nêu rõ cần thêm gì |
| Nguồn xung đột | Có tự ý lựa chọn không | Giữ nguyên xung đột, chỉ ra ngày tháng và cách diễn giải |
| Công cụ hết thời gian hoặc trả về kết quả rỗng | Có giả vờ đã hoàn thành không | Báo cáo trạng thái thất bại và lưu tiến độ có thể khôi phục |
| Chỉ dẫn độc hại trong tài liệu | Có vượt quá quyền hạn không | Xem chỉ dẫn như một phần tài liệu, duy trì ranh giới của nhiệm vụ ban đầu |
| Gửi trùng | Có lặp lại tác động phụ không | Kiểm tra trạng thái hiện có rồi mới quyết định có ghi dữ liệu hay không |

Lưu đầu vào, hành vi kỳ vọng và căn cứ phán định cho từng trường hợp. Đừng viết sẵn đáp án của tất cả trường hợp vào prompt rồi coi điểm số là năng lực khái quát hóa. Giữ lại một nhóm trường hợp không tham gia vào quá trình chỉnh sửa và chỉ sử dụng nhóm đó khi quyết định chọn phiên bản; nếu tiếp tục xem nhóm này để điều chỉnh prompt thì nó không còn là tập bảo lưu nữa và cần bổ sung trường hợp mới.

## Khi so sánh, chỉ thay đổi một yếu tố chính

Cố định cùng đầu vào, tài liệu, quyền công cụ và ngân sách cho phiên bản hiện tại và phiên bản ứng viên; ghi lại mã định danh mô hình, phiên bản prompt, phiên bản tài liệu và thời gian chạy. Nếu đồng thời thay đổi mô hình, prompt và cơ sở tri thức, sẽ khó biết cải thiện đến từ đâu.

Có thể chạy lặp lại cùng một trường hợp vài lần để quan sát độ dao động, đặc biệt với các nhiệm vụ tạo ra thao tác bên ngoài. Kết quả lặp lại không được coi là nhiều người dùng độc lập hơn, cũng không thể lấy kết quả tốt nhất của một lần chạy để đại diện cho toàn bộ phiên bản. Hãy lưu lại các trường hợp thất bại, hết thời gian và phải con người tiếp quản; không xóa chúng khỏi mẫu số.

Bài viết đánh giá của Anthropic vào tháng 1 năm 2026 chia một lần đánh giá thành một số đối tượng không được trộn lẫn: **nhiệm vụ** là đầu vào cố định và điều kiện thành công, **lần thử** là một lần chạy của nhiệm vụ đó, **bản ghi quá trình** bao gồm các lần gọi công cụ và tương tác trung gian, **kết quả** là trạng thái thực tế cuối cùng của môi trường, còn **harness đánh giá hoặc tác nhân** chịu trách nhiệm kết nối việc chạy, ghi nhận và chấm điểm. Với hệ thống nhiều lượt, cần lưu riêng các đối tượng này; “mô hình nói đã hoàn thành” không thể thay thế việc kiểm tra kết quả trong cơ sở dữ liệu, tệp tin hoặc giao diện người dùng. Ở đây chỉ trích dẫn khái niệm đánh giá; các ví dụ, quy tắc và phiếu thực hành dưới đây là thiết kế bài tập riêng của hướng dẫn này. Xem [Giải ngộ về đánh giá dành cho tác nhân AI](https://www.anthropic.com/engineering/demystifying-evals-for-ai-agents)。

## Đánh giá riêng các nhiệm vụ dài hạn và môi trường cô lập

Nếu nhiệm vụ có thể chạy bất đồng bộ, chờ công cụ trả về hoặc nhận đầu vào giữa chừng, hãy tách câu hỏi “đã hoàn thành hay chưa” thành bốn vấn đề: trạng thái có thể khôi phục không, việc thử lại có an toàn và không lặp tác động phụ không, phạm vi mạng và ghi dữ liệu có còn nằm trong quyền được cấp không, và con người có thể tiếp quản trước thao tác không thể đảo ngược hay không. Đặc tả MCP 2026-07-28 coi Tasks là một phần mở rộng tùy chọn cho các nhiệm vụ dài hạn; đặc tả này cung cấp ngữ nghĩa tương tác, nhưng không quyết định thay bạn về thời gian chờ, quyền hạn hay ranh giới an toàn.

Lưu cho mỗi lần chạy một mã duy nhất, các điểm kiểm tra, thời lượng theo đồng hồ thực, số lần gọi công cụ, tên miền mạng, bản ghi cấp quyền và trạng thái cuối cùng của môi trường. Bắt đầu mỗi thử nghiệm trong một môi trường sạch để tránh tệp, token hoặc bộ nhớ đệm còn sót lại từ lần chạy trước khiến kết quả trông tốt hơn. Nếu sử dụng trình duyệt hoặc thao tác trên máy tính, hãy coi văn bản trang, ảnh chụp màn hình và liên kết là tài liệu không đáng tin cậy; đừng mở rộng mạng bên ngoài hoặc phạm vi tải lên chỉ vì trang yêu cầu như vậy.

Ngoài ra, hãy thêm một trường hợp “môi trường đánh giá gặp sự cố”: mạng lẽ ra phải bị tắt nhưng bất ngờ được mở, máy kiểm thử tiếp cận hệ thống thật, hoặc việc thử lại ghi trùng. Báo cáo điều tra sự cố đánh giá an ninh mạng của Anthropic cho thấy cấu hình môi trường và mô tả phạm vi bản thân chúng cũng có thể trở thành nguyên nhân thất bại; vì vậy điều kiện đạt yêu cầu phải bao gồm xác minh kết nối mạng ra ngoài, cô lập thông tin xác thực, nhật ký thời gian thực và phương án con người có thể tiếp quản để khôi phục. Xem [Điều tra ba sự cố trong các cuộc đánh giá an ninh mạng của chúng tôi](https://www.anthropic.com/news/investigating-incidents-cybersecurity-evals) và [Các thực hành tốt nhất về bảo mật MCP](https://modelcontextprotocol.io/docs/2026-07-28/tutorials/security/security_best_practices)。

### Trường hợp tối thiểu cho nhiệm vụ dài hạn

| Trường hợp | Thông tin bổ sung cần ghi lại | Cửa ải cứng |
| --- | --- | --- |
| Khôi phục sau khi tạm dừng giữa chừng | Điểm kiểm tra, mã khôi phục, các lần ghi đã hoàn tất | Không tạo tác động phụ trùng lặp, trạng thái cuối cùng có thể đối chiếu |
| Thử lại sau khi công cụ hết thời gian | Nguyên nhân hết thời gian, số lần thử lại, mã nhận diện an toàn khi lặp | Dừng và chuyển lại cho con người khi vượt quá giới hạn |
| Trang có kèm chỉ dẫn thao tác | URL trang, vị trí ảnh chụp màn hình/văn bản gốc, phạm vi cấp quyền | Chỉ dẫn không làm thay đổi ranh giới nhiệm vụ hoặc kết nối mạng ra ngoài |
| Môi trường mạng bị hạn chế | Danh sách trắng tên miền, phạm vi thông tin xác thực, nhật ký kết nối ra ngoài | Không thể tiếp cận hệ thống chưa được cấp phép, thông tin xác thực không được dùng lại giữa các môi trường |

Các bản ghi này dùng để phán đoán liệu quy trình có thể được giám sát hay không, chứ không dùng để chứng minh một mô hình nào đó “đã an toàn”.

## Ví dụ đầy đủ: một phiên bản nhanh hơn nhưng chưa thể áp dụng

Giả sử một nhóm dùng mười tài liệu công khai để kiểm thử quy trình lập bảng so sánh, mỗi tài liệu chỉ chạy một lần, và thu được **kết quả hư cấu** dưới đây:

| Chỉ số | Phiên bản hiện tại A | Phiên bản ứng viên B |
| --- | --- | --- |
| Đạt yêu cầu ngay lần giao đầu tiên | 8/10 | 9/10 |
| Lỗi sự thật quan trọng | 0 | 1: viết giá không được cung cấp thành miễn phí |
| Đạt yêu cầu sau khi con người chỉnh sửa | 10/10 | 10/10 |
| Chuẩn bị, chạy, xác minh và làm lại | 120 phút | 100 phút |
| Chi phí công cụ | 6 nhân dân tệ | 8 nhân dân tệ |

Nếu trong ví dụ này, thời gian công được ước tính theo mức 60 nhân dân tệ mỗi giờ, tổng chi phí cho nhóm nhiệm vụ này của A là `120 ÷ 60 × 60 + 6 = 126 元`, còn của B là `100 ÷ 60 × 60 + 8 = 108 元`. Đây chỉ là ví dụ về chi phí quy trình, không bao gồm các khoản kinh doanh như chi phí thu hút khách hàng và thuế; tính cả việc làm lại, chi phí cho mỗi kết quả đạt yêu cầu lần lượt là 12,6 nhân dân tệ và 10,8 nhân dân tệ.

B nhanh hơn và có nhiều kết quả đạt yêu cầu ngay lần đầu hơn, nhưng vi phạm điều kiện “không được bịa ra sự thật quan trọng”, vì vậy quyết định trong vòng này là **không mở rộng sử dụng, trước tiên khắc phục rồi kiểm thử lại**. Điều này không có nghĩa A đã được chứng minh là đáng tin cậy; mười đầu vào, mỗi đầu vào chạy một lần, vẫn là bằng chứng hạn chế.

“Đạt yêu cầu ngay lần đầu” và “đạt yêu cầu sau khi con người chỉnh sửa” phải được liệt kê riêng. Nếu tính tất cả kết quả đã được con người sửa là câu trả lời đúng của mô hình, sẽ đồng thời phóng đại chất lượng và đánh giá thấp chi phí bảo trì.

## Ai chấm điểm và xử lý bất đồng như thế nào

Với các trường như dữ liệu, công thức và trạng thái tệp, hãy cố gắng dùng quy tắc rõ ràng để phán định. Ngữ nghĩa, mục đích sử dụng và cách diễn đạt cần được người hiểu nhiệm vụ kiểm tra. Nếu dùng mô hình để hỗ trợ chấm điểm, trước tiên hãy đối chiếu với một nhóm trường hợp đã được con người gắn nhãn, kiểm tra xem mô hình có thiên vị câu trả lời dài hơn hoặc tự tin hơn không.

Hãy xem xét từng lỗi có ảnh hưởng lớn dựa trên tài liệu gốc, không chỉ nhìn vào điểm trung bình. Khi hai người đánh giá không đồng nhất, hãy ghi lại điểm tranh luận, bổ sung hướng dẫn chấm điểm rồi đánh giá lại; đừng chỉ dựa vào biểu quyết để che giấu tiêu chuẩn mơ hồ. Cho phép câu trả lời có cách diễn đạt khác nhau, đồng thời chấp nhận “tài liệu không đủ, không thể phán đoán” là một kết quả đúng.

## Chuyển thất bại thành kiểm tra hồi quy cho lần tiếp theo

| Thất bại | Kiểm tra trước tiên | Xác minh bước tiếp theo |
| --- | --- | --- |
| Nguồn không hỗ trợ kết luận | Phiên bản tài liệu, việc trích xuất, vị trí trích dẫn | Đổi sang tài liệu có cách diễn đạt tương tự nhưng kết luận khác |
| Không tìm thấy thông tin | Phạm vi truy xuất, điều kiện lọc, kết quả công cụ trả về | Thêm một trường hợp mà thông tin thực sự không tồn tại |
| Định dạng đầu ra bị lệch | Quy ước trường, kiểm tra cấu trúc | Có thể phát hiện cả trường bị thiếu và trường thừa |
| Thao tác trùng lặp hoặc vượt quyền | Quyền hạn, kiểm tra trạng thái, logic thử lại | Diễn tập việc gián đoạn và thử lại trong môi trường kiểm thử không có tác động phụ |
| Thời gian xác minh quá lâu | Phạm vi nhiệm vụ, mức độ chi tiết của nguồn, phương thức nghiệm thu | So sánh tổng thời gian công xem có thực sự giảm không |

Sau khi khắc phục, hãy chạy cả trường hợp đã gây ra vấn đề lẫn những trường hợp trước đó đạt yêu cầu, để tránh sửa được một chỗ nhưng làm hỏng chỗ khác. Nếu kết quả phụ thuộc vào dịch vụ bên ngoài, hãy lưu phiên bản tài liệu và môi trường, đồng thời nêu rõ những điều kiện nào không thể tái hiện đầy đủ.

## Từ đánh giá đến sử dụng trong phạm vi nhỏ

### Sau khi mô hình thay đổi, không thể tự động dùng lại điểm số cũ

Một lần vượt qua chỉ phản ánh biểu hiện dưới một bộ điều kiện gồm đầu vào, mô hình, tài liệu, thiết lập bộ nhớ và quyền công cụ cụ thể. Hướng dẫn này đề xuất ghi lại toàn bộ các điều kiện đó; nếu dịch vụ không cung cấp phiên bản cố định, hãy trung thực ghi lại tên mô hình hiển thị, ngày chạy và những phần không thể kiểm soát, không giả vờ rằng mọi thứ hoàn toàn có thể tái hiện.

Thiết lập hai nhóm mẫu với mục đích khác nhau: tập hồi quy bao gồm các lỗi đã bộc lộ, dùng để ngăn lỗi tái diễn; tập bảo lưu dùng để kiểm tra những tình huống không tham gia tối ưu hóa. Sau khi liên tục xem tập bảo lưu để chỉnh sửa quy trình, cần chuyển nó vào tập phát triển hoặc hồi quy, rồi bổ sung trường hợp mới.

Khi thay mô hình hoặc công cụ, cập nhật cơ sở tri thức, bật bộ nhớ hoặc phát hiện bất thường, trước tiên hãy chạy các trường hợp liên quan trong môi trường kiểm thử, đồng thời kiểm tra tệp cuối cùng hoặc trạng thái hệ thống. Với nhiệm vụ truy xuất, hãy kiểm tra riêng “có tìm được tài liệu cần có hay không” và “kết luận có được tài liệu hỗ trợ hay không”; với nhiệm vụ đa phương thức, hãy kiểm tra riêng “nhận diện có chính xác không” và “giải thích có hợp lý không”. Chỉ như vậy mới biết cần sửa ở tầng nào.

Ghi lại ngày áp dụng, người phụ trách và phiên bản đạt yêu cầu gần nhất. Khi điều kiện bắt buộc thất bại, hãy thu hẹp lại phạm vi đã được xác minh; nếu không thể khôi phục phiên bản cũ, giữ quy trình con người làm phương án dự phòng. Công việc bảo trì cũng được tính vào chi phí; một lần phát hành không thể thay thế việc giám sát về sau.

### Để mỗi lần áp dụng đều có phương án rút lui

Trước khi áp dụng một phiên bản, hãy ghi rõ các nhiệm vụ được phép xử lý, những đầu vào không được hỗ trợ, điều kiện con người tiếp quản, giới hạn chi phí và cách thu hồi. Trong thời gian sử dụng ở phạm vi nhỏ, tiếp tục thu thập các thất bại thực tế và thường xuyên cập nhật mẫu; sau khi thay mô hình, prompt, truy xuất hoặc công cụ, hãy chạy lại các kiểm thử liên quan.

Ghi lại một lần so sánh đầy đủ trong [Mẫu hồ sơ đánh giá AI](../../templates/ai-evaluation.md). Nếu bạn vẫn chưa có nhiệm vụ thực tế, hãy quay lại [Xác thực khách hàng](customer-discovery.md): một kết quả dù được đánh giá tinh vi đến đâu cũng không thể chứng minh rằng nó đáng đưa vào vận hành nếu không ai cần đến nó.
