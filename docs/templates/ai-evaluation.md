---
title: "Mẫu ghi chép đánh giá AI"
description: "Ghi lại phạm vi nhiệm vụ, mẫu được giữ lại, phiên bản, điều kiện bắt buộc, các lỗi và toàn bộ chi phí, nhằm hỗ trợ quyết định áp dụng, khắc phục hoặc rút lại quy trình AI."
updated: 2026-10-16
---

# Mẫu ghi chép đánh giá AI

Được sử dụng cùng với [Đánh giá và độ tin cậy của AI](../threads/practice/ai-evaluation.md). Trước tiên hãy điền các tiêu chuẩn, sau đó chạy các trường hợp. Bảng trống dùng để ghi chép việc so sánh một phiên bản; các con số minh họa không đại diện cho hiệu suất của mô hình hoặc ngưỡng triển khai chung.

## Bản ghi có thể sao chép

```markdown
# Đánh giá AI — Ngày / Nhiệm vụ

## Phạm vi
- Người dùng và hành động cần thực hiện:
- Tài liệu đầu vào, quyền truy cập và cách loại bỏ thông tin nhận dạng:
- Phương án thực hiện thủ công làm mốc so sánh và tổng thời gian:
- Các nhiệm vụ không được hỗ trợ:

## Thiết lập kiểm thử (cố định trước khi chạy)
- Phiên bản hiện tại / phiên bản đề xuất:
- Mô hình, prompt, tài liệu truy xuất, phiên bản công cụ:
- Ngày chạy, khu vực, thiết lập bộ nhớ; phiên bản dịch vụ không thể cố định:
- Trong vòng này chỉ thay đổi:
- Mẫu phát triển / mẫu giữ lại không dùng để tinh chỉnh:
- Số lần chạy mỗi trường hợp và giới hạn thời gian, số lượt gọi, chi phí:
- Các điều kiện bắt buộc phải đạt:
- Chất lượng có thể so sánh và hướng dẫn chấm điểm thủ công:
- Người chấm điểm / cách giải quyết bất đồng:
- Các tình huống thất bại liên quan: thiếu nguồn / prompt injection / vượt quyền / thử lại mất kiểm soát hoặc gây tác dụng phụ lặp lại / lỗi phiên âm hoặc nhận diện hình ảnh:
- Trường dành cho tác vụ dài: mã nhiệm vụ / mã lượt chạy, điểm kiểm tra, thời gian thực tế trôi qua, thời gian chờ, số lần thử lại tối đa, mã định danh chống xử lý trùng lặp, điểm chuyển giao cho con người:
- Trường về môi trường cô lập: môi trường sạch, danh sách cho phép kết nối mạng ra ngoài, phạm vi quyền của thông tin xác thực, giải thích về đầu vào không đáng tin cậy từ trình duyệt / trang web:
- Trường về chính sách: tên chính sách của nhà cung cấp, phiên bản, ngày có hiệu lực, khu vực, yêu cầu con người xem xét đối với trường hợp rủi ro cao:

## Ghi chép từng trường hợp (sao chép phần này riêng cho mỗi phiên bản)
- Phiên bản trong phần này:
- ID dùng định dạng “mã trường hợp / số thứ tự lần thử”, ví dụ 07 / 2; đầu vào tham chiếu đến tài liệu đã được cố định cho trường hợp đó.

### Trường hợp (sao chép một bản cho mỗi lần thử)
- Mã trường hợp / số thứ tự lần thử:
- Loại và vị trí tài liệu đầu vào cố định:
- Hành vi mong đợi / căn cứ đánh giá:
- Vị trí trích đoạn gốc / khoảng thời gian trong âm thanh hoặc video / vùng hình ảnh làm bằng chứng cho kết luận:
- Hành vi thực tế / vị trí sản phẩm đầu ra:
- Vị trí bản ghi quá trình / lượt gọi công cụ / bản ghi cấp quyền:
- Điểm kiểm tra / mã khôi phục / bản ghi thử lại và chống xử lý trùng lặp:
- Kết nối mạng ra ngoài, bằng chứng từ trang web hoặc ảnh chụp màn hình, phạm vi quyền của thông tin xác thực:
- Kết quả cuối cùng trong môi trường (tệp, cơ sở dữ liệu hoặc trạng thái người dùng nhìn thấy):
- Lần đầu có đạt yêu cầu không / điều kiện bắt buộc không đạt:
- Số phút chỉnh sửa thủ công / nội dung chỉnh sửa:
- Trạng thái cuối cùng (giữ lại cả thất bại và hết thời gian chờ):

## Tổng hợp (tính riêng cho từng phiên bản, giữ các lần thất bại và hết thời gian chờ trong mẫu số)
- Số lần đạt yêu cầu ngay lần đầu / tổng số lần thử:
- Các điều kiện bắt buộc không đạt và trường hợp cụ thể:
- Số lần đạt yêu cầu sau khi chỉnh sửa thủ công / tổng số lần thử:
- Tổng số phút chuẩn bị, chạy, kiểm chứng và làm lại:
- Chi phí công cụ và phương pháp quy đổi chi phí nhân công:
- Tổng chi phí của cả quá trình trong đợt này / số lượng kết quả cuối cùng đạt yêu cầu:
- Giới hạn của bằng chứng và các suy luận không được bằng chứng hỗ trợ:

## Quyết định và bước tiếp theo
- Áp dụng / giữ nguyên hiện trạng / sửa và kiểm thử lại / dừng:
- Các trường hợp làm căn cứ cho quyết định:
- Các trường hợp kiểm thử hồi quy mới và phạm vi chạy lại:
- Điều kiện kích hoạt kiểm thử lại khi mô hình, tài liệu, công cụ hoặc bộ nhớ thay đổi; phiên bản gần nhất đạt yêu cầu:
- Phạm vi được phép sử dụng / thời điểm chuyển giao cho con người / điều kiện thu hồi:
- Kết quả diễn tập phương án rút lui khi đổi nhà cung cấp, tắt bộ nhớ hoặc ngắt kết nối công cụ:
- Người phụ trách, ngày xem xét lại, vị trí lưu bản ghi:
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