# 資料庫結構 (Database Schema)

## 表格設計

### Users
- `id`: UUID (PK)
- `email`: String (Unique)
- `password_hash`: String

### Documents
- `id`: UUID (PK)
- `owner_id`: UUID (FK -> Users.id)
- `content_path`: String
- `created_at`: Timestamp
