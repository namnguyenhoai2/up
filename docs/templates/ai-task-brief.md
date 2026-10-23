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

Bối cảnh thực tế:
Người dùng/đối tượng tiếp nhận:
Quyết định hoặc hành động cần hoàn thành:
Vì sao thực hiện ngay bây giờ:
Hạn chót và mốc không thể bỏ lỡ:
Người chịu trách nhiệm cuối cùng và người rà soát thủ công:
Ai sẽ bị ảnh hưởng nếu không làm hoặc trì hoãn:
```

Hãy chuyển “học AI” hoặc “làm một trợ lý thông minh” thành các hành động có thể quan sát được, chẳng hạn như “người dùng có thể nhập một tệp trong vòng 10 phút và xem một báo cáo có thể giải thích nguồn gốc và lỗi”.

## 2. Dữ liệu đầu vào, nguồn và ranh giới dữ liệu

| Đầu vào/khẳng định | Loại | Nguồn, phiên bản và vị trí | Có thể cung cấp cho mô hình không | Người xác minh | Điều kiện mất hiệu lực |
| --- | --- | --- | --- | --- | --- |
| | Sự thật / suy luận / kinh nghiệm cá nhân / dữ liệu người dùng / nội dung bên thứ ba | | Công khai / đã ẩn danh / được tổ chức phê duyệt / cấm | | |

```markdown
Tệp và trường được phép sử dụng:
Tài liệu xác định không cung cấp:
Mức độ nhạy cảm dữ liệu: công khai / nội bộ / mật / hạn chế
Thời hạn thu thập, truyền, lưu giữ và xóa:
Đã có sự đồng ý cần thiết chưa:
Yêu cầu về bản quyền, giấy phép, trích dẫn và ghi công:
Phạm vi dữ liệu tối thiểu mô hình có thể tiếp cận:
```

Nguồn không đồng nghĩa với sự thật. Mỗi khẳng định quan trọng phải có thể truy về văn bản gốc, phiên bản, phạm vi dữ liệu hoặc quan sát trực tiếp; các liên kết, con số và trích dẫn do mô hình đưa ra vẫn cần được con người xác minh.

## 3. Kết quả đầu ra và tập đánh giá

```markdown
Sản phẩm bàn giao cuối cùng:
Định dạng, độ dài và đối tượng tiếp nhận:
Tiêu chí hoàn thành có thể quan sát:
Cổng cứng bắt buộc phải vượt qua:
Các biến thể chấp nhận được:
Nội dung tuyệt đối không được xuất hiện:
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
AI có thể làm: đặt câu hỏi / phân loại / giải thích phương án / phản ví dụ / chép lại / bản nháp / gợi ý kiểm thử
AI không được làm: phán đoán sự thật cuối cùng / bịa nguồn / thay người chịu trách nhiệm phê duyệt / vượt quyền
                    / hoàn thành kỳ thi hoặc đơn đăng ký cấm hỗ trợ bên ngoài / tự động xuất bản
Chế độ sử dụng: chẩn đoán / hỗ trợ / tạo phương án / xử lý hàng loạt / khác
Mô hình, phiên bản, khu vực và ngày gọi:
Công cụ bên ngoài, máy chủ MCP hoặc giao thức khác cùng phiên bản:
Phạm vi đọc/ghi, người cấp quyền và cách thu hồi của từng công cụ:
Vị trí phiên bản lời nhắc, chỉ dẫn hệ thống hoặc quy trình:
```

Nếu nhiệm vụ sẽ chạy trong thời gian dài hoặc gọi các công cụ bên ngoài, cũng cần ghi lại:

```markdown
Mã lần chạy/nhiệm vụ và mã nhiệm vụ cha:
Đồng bộ hay bất đồng bộ; thời gian dự kiến và tối đa theo đồng hồ thực:
Vị trí điểm kiểm tra và các bước khôi phục:
Số lần thử lại tối đa, hết hạn và mã an toàn chống lặp:
Trang trình duyệt, ảnh chụp màn hình và chỉ dẫn bên ngoài đều được xem là đầu vào không đáng tin cậy:
Danh sách cho phép đầu ra mạng và phạm vi thông tin xác thực:
Ghi ra bên ngoài, biên nhận và trạng thái môi trường cuối:
Điểm con người tiếp quản và cách dừng khẩn cấp:
Chính sách/phiên bản nhà cung cấp, ngày hiệu lực, khu vực và rà soát rủi ro cao:
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
Giới hạn ước tính về số lần gọi, thời gian và chi phí:
Ngân sách rà soát thủ công và làm lại:
Dữ liệu có đi vào huấn luyện, nhật ký hoặc lưu giữ bên thứ ba không:
Độ trễ có thể chấp nhận và phương án hạ cấp:
Có thể thu hồi, chạy lại hoặc khôi phục về phiên bản nào:
Phạm vi phát hành và đối tượng triển khai từng phần:
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
Trạng thái hiện tại: chưa bắt đầu / thử nghiệm / dùng thử nội bộ / triển khai từng phần / đã bàn giao / đã dừng
Phần đã hoàn thành và vị trí bằng chứng:
Vấn đề chưa giải quyết và rủi ro:
Nhiệm vụ nhỏ nhất tiếp theo:
Người phụ trách bàn giao, thời gian và quyền hạn:
Phạm vi tham gia của AI mà độc giả/người dùng cần biết:
Giải thích về nguồn, quyền riêng tư, bản quyền và lợi ích liên quan:
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
