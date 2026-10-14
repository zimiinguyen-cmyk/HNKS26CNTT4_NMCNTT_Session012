# BÀI LÀM – HACKATHON GIỮA MÔN 01

- **Họ tên: Nguyễn Ngọc Tuấn Anh**
- **Lớp: CNTT04** 
- **Link repository:** 
- **Hệ điều hành (Windows/macOS): Windows** 

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng
PS D:\OnTap\demo-on-tap\cafe-website> ls
PS D:\OnTap\demo-on-tap\cafe-website> mv "Ghi Chu.txt" docs
PS D:\OnTap\demo-on-tap\cafe-website> Copy-Item media backup -Recurse
PS D:\OnTap\demo-on-tap\cafe-website> Remove-Item temp_001.tmp
PS D:\OnTap\demo-on-tap\cafe-website> Get-ChildItem .\logs

```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
# Ghi lệnh vào đây (xoá dòng này)
PS D:\OnTap\demo-on-tap\cafe-website> Select-String "ERROR" .\logs\server.log
PS D:\OnTap\demo-on-tap\cafe-website>

```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [ ] Heading 1: tên dự án
- [ ] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [ ] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [ ] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
- [ ] Task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [ ] Blockquote nhắc không upload `.env`

## 4.5. Nâng cao – Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Ghi lệnh vào đây (xoá dòng này)
# Script: auto_report.ps1
# Tac gia: Nguyễn Ngọc Tuấn Anh
# Ngay tao: 13/10/2026
 
Write-Host "Dang loc log..."
 
"=== BAO CAO LOI ===" > .\logs\auto_report.txt
Get-Content .\logs\server.log | Select-String "ERROR" >> logs/auto_report.txt

Write-Host "Hoan thanh!"

```

### Kết quả hiển thị

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.6. Nâng cao – Đếm số dòng lỗi

### Lệnh

```shell
# Ghi lệnh vào đây (xoá dòng này)
PS D:\OnTap\demo-on-tap\cafe-website> (Select-String "ERROR" .\logs\server.log).Count

```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.7. Nâng cao – Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng (xoá dòng này)
PS D:\OnTap\demo-on-tap\cafe-website> "=== TONG HOP LOG ===" > .\logs\tong_hop.txt
PS D:\OnTap\demo-on-tap\cafe-website> Get-Content .\logs\server.log | Select-String "WARNING" >> .\logs\tong_hop.txt
PS D:\OnTap\demo-on-tap\cafe-website> (Select-String 'ERROR' .\logs\server.log).Count

```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.8. Nâng cao – Excel

> Phần Excel được chấm trực tiếp trên file `data/orders_thang_9.xlsx`, không cần ghi vào đây.
