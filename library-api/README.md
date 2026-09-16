# Library Management Project

## 1. Backend Server Setup
- **Port running:** `http://localhost:3000`
- **Database:** MongoDB (`aptech_library`)

## 2. API Endpoints cho ReactJS Client
| Method | Endpoint | Description | Query/Params/Body |
| :--- | :--- | :--- | :--- |
| `GET` | `/books` | Lấy tất cả sách | None |
| `GET` | `/books/:id` | Lấy chi tiết sách theo ID | Param: `id` |
| `GET` | `/books/category/:category` | Lấy danh sách sách theo thể loại | Param: `category` |
| `POST` | `/books` | Thêm sách mới | Body: `{ title, author, category, available }` |
| `PUT` | `/books/:id` | Cập nhật sách | Param: `id`, Body: các trường cần cập nhật |
| `DELETE` | `/books/:id` | Xóa sách | Param: `id` |

## 3. Cấu trúc dữ liệu JSON (Book Schema)
```json
{
  "_id": "66b1f0b8e3c9a7d1a1234567",
  "title": "Node.js Basics",
  "author": "Aptech",
  "category": "Programming",
  "available": true
}