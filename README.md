# Bài tập 02 - Lập trình Web
**Họ tên:** Nguyễn Xuân Bắc  
**Domain ảo:** http://nguyenxuanbac.com/  
**Thư mục web:** D:\Apache24\nguyenxuanbac  

---

## 1️⃣ Cài đặt Apache
- Giải nén Apache vào D:\Apache24  
- Sửa file cấu hình httpd.conf và httpd-vhosts.conf  
- Thêm domain ảo nguyenxuanbac.com
- <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/6129f63e-69d3-4955-800a-e6f802da87cd" />
- <img width="1782" height="938" alt="image" src="https://github.com/user-attachments/assets/6f1d96b9-0edf-4d26-8ea9-f316b45c8056" />
- <img width="1814" height="972" alt="image" src="https://github.com/user-attachments/assets/9255bec7-eb9b-4a9d-8575-fcb07040a102" />
- <img width="1809" height="974" alt="image" src="https://github.com/user-attachments/assets/ecdc5ed7-b550-4c74-8eb8-893825f91178" />
- <img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/0bb48102-b36d-4eb8-a4bc-56b38bddca92" />

## 2️⃣ CÀI NODE.JS & NODE-RED
- Cài Node-RED: npm install -g --unsafe-perm node-red --prefix "D:\nodejs\nodered"
- Tạo file chạy run-nodered.cmd:
@echo off
set PATH=D:\nodejs;%PATH%
node "D:\nodejs\nodered\node_modules\node-red\red.js" -u "D:\nodejs\nodered\work" %*
- Chạy Node-RED tại http://localhost:1880
- <img width="1566" height="836" alt="image" src="https://github.com/user-attachments/assets/08e54204-853c-460d-b770-a8d4304d496f" />
- <img width="1539" height="842" alt="image" src="https://github.com/user-attachments/assets/8f6ba38b-0950-473b-9e4c-209bdda07ce5" />
- <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2dff4e75-782a-4105-b835-6bcfe2e3204c" />

## 3️⃣ CẤU HÌNH SQL SERVER
- Tạo database: BTVN02 
- Bảng SinhVien:
- CREATE DATABASE BTVN02;
GO
USE BTVN02;
GO
CREATE TABLE SinhVien (
  Id INT PRIMARY KEY IDENTITY(1,1),
  HoTen NVARCHAR(100),
  Lop NVARCHAR(50)
);
GO
INSERT INTO SinhVien (HoTen, Lop) VALUES
(N'Nguyễn Thị Ánh', N'K16-HTTT'),
(N'Phạm Thị Thu', N'K16-HTTT'),
(N'Lê Thị Mai', N'K16-HTTT');
- <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/f503afdb-71a2-4189-a47e-0c85a0d93ed8" />
- <img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/86e0bb00-955a-4b5f-a5cb-4460ac6626eb" />

## 4️⃣ CÀI ĐẶT CÁC NODE CẦN THIẾT TRONG NODE-RED
- Install và cài:
node-red-contrib-mssql-plus
node-red-contrib-moment
node-red-contrib-cron-plus
node-red-contrib-telegrambot
<img width="1903" height="1068" alt="image" src="https://github.com/user-attachments/assets/633c9c2f-b37f-464a-9ea1-8e14b300d4f5" />

## 5️⃣ TẠO FLOW KẾT NỐI SQL SERVER
<img width="1914" height="1071" alt="image" src="https://github.com/user-attachments/assets/0f3db90d-8266-472d-8bf8-be5c025a0d2a" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/d3c7f6bc-9e53-4f03-9a55-bd15d5b6c705" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/2b618d0e-ac3b-4ebc-ab82-138959237b7d" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/91abd46a-766d-444e-9c3a-06bb06e85530" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/09220bf8-b405-4e64-90e8-00a03564b7b7" />
## Kết quả kiểm tra API
- Truy cập: http://localhost:1880/timkiem?q=thi
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/3ed9e978-99b6-46d2-b116-844f449de4e0" />




