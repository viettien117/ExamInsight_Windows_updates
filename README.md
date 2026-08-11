# ExamInsight

**Phần mềm thống kê kết quả thi trắc nghiệm** — đọc file kết quả do [ExamScan](https://github.com/viettien117/ExamScan_Windows_updates) chấm ra, tính điểm trung bình, tỷ lệ đạt, phân phối điểm và phân tích xem câu nào cả lớp sai nhiều nhất, rồi xuất báo cáo Excel/PDF.

Repo này host **bản cài đặt Windows mới nhất** và **kênh cập nhật tự động** cho ExamInsight.

---

## Tải xuống bản mới nhất

1. Vào trang [**Releases**](https://github.com/viettien117/ExamInsight_Windows_updates/releases/latest)
2. Trong mục **Assets**, tải file `ExamInsight-x.y.z-x64.msi`
3. Double-click file `.msi` → đi qua wizard cài đặt
4. Mở phần mềm từ **Start Menu** hoặc shortcut **Desktop** → "ExamInsight"

> Nếu Windows SmartScreen cảnh báo *"Windows protected your PC"*, bấm **More info** → **Run anyway** (file được ký bằng EdDSA của nhà phát triển).

## Yêu cầu hệ thống

- Windows 10 (64-bit) hoặc Windows 11
- Bản cài đặt **self-contained** đã kèm sẵn .NET runtime — **không cần cài .NET**

## Dùng thử ngay, chưa cần dữ liệu thật

Ở Bước 1 bấm **"Thử với file mẫu"** — chương trình tự điền cả ba file đầu vào lẫn thông tin bài kiểm tra, bạn chỉ việc bấm **NẠP & THỐNG KÊ**. Bộ file mẫu nằm sẵn bên trong chương trình nên không cần mạng.

## Ba file đầu vào

| File | Do đâu tạo ra | Bắt buộc |
|---|---|---|
| `KetQua.xlsx` | ExamScan tạo sau khi chấm | Có |
| `DapAn.xlsx` | [ExamMixer](https://github.com/viettien117/ExamMixer_Windows_updates) tạo cùng lúc với đề thi | Không — nhưng thiếu thì không phân tích được câu hỏi |
| `DanhSachSinhVien.xlsx` | Bạn tự soạn (cột A số thứ tự, cột B mã số, cột C họ tên) | Không — thiếu thì bảng chỉ hiện mã số |

## Cập nhật tự động

Sau khi cài bản đầu tiên, **bạn không cần truy cập trang này nữa**. Phần mềm sẽ:

- Tự động kiểm tra bản mới mỗi ngày khi mở app
- Hiển thị thông báo khi có version mới, tải về + cài đè với 1 click
- Kiểm tra thủ công: vào mục **"Cập nhật"** trong chương trình

## Bộ phần mềm Exam*

- [**ExamMixer**](https://github.com/viettien117/ExamMixer_Windows_updates) — trộn đề trắc nghiệm từ ngân hàng câu hỏi Word
- [**ExamScan**](https://github.com/viettien117/ExamScan_Windows_updates) — chấm phiếu trả lời bằng ảnh chụp (Windows, Android, iOS)
- **ExamInsight** — thống kê và phân tích kết quả chấm

## Lịch sử phiên bản

Xem changelog từng phiên bản tại [appcast.xml](appcast.xml) hoặc trang [Releases](https://github.com/viettien117/ExamInsight_Windows_updates/releases).

## Bản quyền

Copyright © 2026 RuBi. All rights reserved.
