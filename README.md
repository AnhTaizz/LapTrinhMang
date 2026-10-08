# Lập trình mạng — 72 bài Java / NetBeans

Project Java Ant, JDK 17 trở lên. Mỗi bài có một file Java riêng, 9 package theo dạng bài.

## Mở và chạy trong NetBeans

1. Giải nén ZIP. Chọn **File → Open Project**, chọn thư mục `LapTrinhMang_NetBeans` chứa `build.xml` và `nbproject`.
2. Nếu IDE yêu cầu nền tảng Java, chọn JDK 17 trở lên trong **Project Properties → Libraries → Java Platform**.
3. Chọn **Clean and Build Project**. Không cần thư viện ngoài.
4. Mở **Source Packages**, chọn package dạng bài, mở file cần làm.
5. Kiểm tra mã câu hỏi và cổng theo đề đang được giao. Mã sinh viên trong code đã đặt thành **B23DCCN730**.
6. Chuột phải file bài → **Run File (Shift+F6)**. **Run Project (F6)** chỉ in hướng dẫn, không tự gửi bài lên server.

Đề bài nằm trong comment đầu mỗi file Java. [Mục lục](MUC_LUC.md) dẫn tới đủ 72 bài.
Thư mục `de_bai` giữ toàn bộ từng mục nguồn (đề, code gốc, ghi chú) để đối chiếu.

## Các package

- `TCP.byte_stream`: 11 bài
- `TCP.data_stream`: 7 bài
- `TCP.character_stream`: 19 bài
- `TCP.object_stream`: 6 bài
- `TCP.gzip_stream`: 2 bài
- `TCP.nio_stream`: 2 bài
- `UDP.data_type`: 9 bài
- `UDP.string_type`: 11 bài
- `UDP.object_type`: 5 bài
- `TCP`, `UDP`: các lớp dữ liệu dùng khi serialize; giữ nguyên tên đầy đủ, kiểu thuộc tính và serialVersionUID.

## Phạm vi

Nguồn bài: 5 file Word đã cung cấp. Repo tham khảo cấu trúc: https://github.com/datnt-numenor/Lap-trinh-mang
Đã đổi tên class Main/tam theo từng bài, tách package và model để toàn bộ project cùng biên dịch được.
Không lấy trạng thái AC trong tài liệu làm kết quả kiểm thử của project này. Chưa kết nối server để chấm lại thuật toán/giao thức.
Các mã còn thiếu hoặc placeholder trong nguồn phải được thay bằng qCode của bạn; không suy ra mã bài từ ảnh.

`nbproject/build-impl.xml` được sinh từ stylesheet Apache NetBeans (Apache License 2.0), với thông báo bản quyền giữ trong file.

## Kiểm tra đã thực hiện

- Biên dịch đồng thời 83 file Java bằng JDK 17: thành công.
- Ant `clean jar run`: BUILD SUCCESSFUL.
- Ant `run-single` với file hướng dẫn: thành công.
- Chưa mở giao diện NetBeans và chưa chạy các bài với máy chủ chấm.

## Các bài có mã câu hỏi chưa hoàn chỉnh trong nguồn

- [BÀI 3: Tổng Số Nguyên Tố](src/TCP1/byte_stream/Bai03_TongSoNguyenTo.java)
- [BÀI 3: Đảo Ngược Chuỗi](src/TCP1/character_stream/Bai03_DaoNguocChuoi.java)
- [BÀI B10. LỌC KÝ TỰ + LOẠI TRÙNG (BÀI MỚI TỪ HỆ THỐNG)  [qCode: cập nhật sau]](src/UDP/string_type/Bai10_LocKyTuLoaiTrung.java)
- [BÀI B11. MASK LOG + ĐẾM ERROR/INFO/WARN (BÀI MỚI TỪ HỆ THỐNG)  [qCode: cập nhật sau]](src/UDP/string_type/Bai11_MaskLogDemErrorInfoWarn.java)

Đối chiếu đề của bạn trước khi chạy. Một số bài còn thiếu mã ở tiêu đề vẫn có mã mẫu trong code; không coi mã mẫu là mã được cấp cho tài khoản của bạn.
