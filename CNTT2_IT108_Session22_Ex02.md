# Bài 2: Xử lý lỗi thư viện mã nguồn mở bằng GitHub Issues

## 1. Bình luận nào mình đọc trước?

Mình sẽ ưu tiên đọc những bình luận có:

- **Nhiều Reactions** như 👍 (Thumbs Up), ❤️ (Hearts), 🎉: nghĩa là nhiều người cũng gặp lỗi và thấy cách này hiệu quả.
- Bình luận của **Maintainer / Owner / Member** (người trong nhóm phát triển, có nhãn bên cạnh tên): họ hiểu rõ code nên đáng tin hơn.
- Bình luận được **gắn link tới Pull Request / commit sửa lỗi**, hoặc có ghi rõ phiên bản, hệ điều hành giống máy mình (ví dụ Linux, macOS, v0.15.2).
- Những bình luận bị người khác phản bác hoặc không có ai ủng hộ thì mình đọc sau.

## 2. Workaround là gì?

**Workaround** là cách xử lý *tạm thời* để phần mềm vẫn chạy được trong lúc lỗi gốc chưa được sửa. Nó không sửa nguyên nhân thật sự của lỗi.

Ví dụ trong bài: cài lại bản `v0.14.0` (bản cũ chưa bị lỗi) thay vì dùng `v0.15.2`.

## 3. Vì sao không nên chờ bản cập nhật chính thức?

- Lỗi xảy ra ở **môi trường sản xuất** (production), nếu chờ thì hệ thống bị dừng, người dùng bị ảnh hưởng.
- Không ai biết bao giờ nhóm tác giả mới phát hành bản vá (có thể vài ngày hoặc vài tuần).
- Có workaround thì dự án vẫn chạy tiếp, đến khi có bản sửa chính thức thì mình cập nhật lại.

**Lưu ý:** workaround chỉ là giải pháp tạm, cần ghi chú lại để sau này gỡ bỏ và thử trước trên máy test, không áp dụng thẳng lên hệ thống thật.
