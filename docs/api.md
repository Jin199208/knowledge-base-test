# API 介面定義 (API Specification)

## Authentication
- **POST** `/v1/login`: 使用者登入並取得 Token。
- **POST** `/v1/logout`: 登出並註銷當前 Token。
- **POST** `/v1/refresh`: 重新整理 Access Token。

## User Profile
- **GET** `/v1/me`: 取得當前登入用戶資訊。
- **PATCH** `/v1/me`: 更新用戶設定。
- **GET** `/v1/users/{id}`: 取得特定用戶的公開資訊。

## Documents
- **POST** `/v1/docs/upload`: 上傳新的 MD 檔案。
- **GET** `/v1/docs/list`: 列出已上傳的文件清單。
- **GET** `/v1/docs/{id}`: 取得特定文件的詳細內容。
- **PUT** `/v1/docs/{id}`: 更新特定文件的內容。
- **DELETE** `/v1/docs/{id}`: 刪除指定的檔案。
- **GET** `/v1/docs/search`: 根據關鍵字搜尋文件。

## Admin
- **GET** `/v1/admin/stats`: 取得系統運行統計數據。
- **GET** `/v1/admin/users`: (管理員) 列出所有系統用戶。
