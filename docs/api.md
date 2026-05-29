# API 介面定義 (API Specification)

## User Profile
- **GET** `/v1/me`: 取得當前登入用戶資訊。
- **PATCH** `/v1/me`: 更新用戶設定。

## Documents
- **POST** `/v1/docs/upload`: 上傳新的 MD 檔案。
- **GET** `/v1/docs/list`: 列出已上傳的文件。
