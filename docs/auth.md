# 身分驗證說明 (Authentication)

本系統使用 JWT (JSON Web Token) 進行身份驗證。

## 登入流程
1. 用戶發送 POST `https://api.test.com/v1/login`。
2. 後端回傳 `access_token` 與 `refresh_token`。
3. 後續請求須在 Header 帶入 `Authorization: Bearer <token>`。

## 權限等級
- Admin: 全權限。
- User: 僅讀寫個人資料。
