# 🎓 Student Management App (Laravel)

Ứng dụng quản lý sinh viên đơn giản được xây dựng bằng Laravel, cho phép thêm và hiển thị danh sách sinh viên.

---

## 🚀 Tính năng chính

- 📋 Hiển thị danh sách sinh viên
- ➕ Thêm sinh viên mới
- 💾 Lưu dữ liệu vào database
- 🎨 Giao diện UI/UX hiện đại (Bootstrap + custom CSS)

---

## 🛠️ Công nghệ sử dụng

- Laravel
- PHP
- MySQL
- Blade Template
- Bootstrap 5

---

## ⚙️ Cài đặt & chạy project

### 1. Clone project

```bash
git clone https://github.com/your-username/student-app.git
cd student-app
```

### 2. Cài dependencies

```bash
composer install
```

### 3. Cấu hình môi trường

Tạo file `.env`:

```bash
cp .env.example .env
```

Sửa thông tin database:

```env
DB_DATABASE=student_db
DB_USERNAME=root
DB_PASSWORD=
```

### 4. Generate key

```bash
php artisan key:generate
```

### 5. Chạy migration

```bash
php artisan migrate
```

### 6. Chạy server

```bash
php artisan serve
```

👉 Truy cập: http://127.0.0.1:8000

---

## 📁 Cấu trúc chính

```
app/
 ├── Models/Student.php
 ├── Http/Controllers/StudentController.php

resources/views/students/
 ├── index.blade.php
 ├── create.blade.php

routes/
 ├── web.php
```

---

## 🔄 Luồng hoạt động

```
User → Route → Controller → Model → Database → View
```

---

## 📌 Các route chính

| Route            | Chức năng          |
| ---------------- | ------------------ |
| /students        | Hiển thị danh sách |
| /students/create | Form thêm          |
| /students/store  | Lưu dữ liệu        |

---

## 🗄️ Database

**Bảng: students**

| Field      | Type     |
| ---------- | -------- |
| id         | bigint   |
| name       | string   |
| major      | string   |
| timestamps | datetime |

---

## ✨ Nâng cấp (đề xuất)

- ✔ Validation dữ liệu
- ✔ CRUD đầy đủ (Edit/Delete)
- ✔ Tìm kiếm sinh viên
- ✔ Phân trang
- ✔ Dark/Light mode

---

## 📸 Demo giao diện

- Trang danh sách sinh viên
- Trang thêm sinh viên

_(Bạn có thể thêm screenshot vào đây)_

---

## 📚 Kiến thức áp dụng

- Mô hình MVC trong Laravel
- Routing & Controller
- Migration & Database
- Blade Template

---

## 👨‍💻 Tác giả

- Sinh viên CNTT
- Bài tập môn Laravel

---

## 📄 License

Dự án phục vụ mục đích học tập.
