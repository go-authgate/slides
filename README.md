# AuthGate × DevOps Day Slides

本專案是「**AuthGate**」的簡報投影片，介紹如何以一座輕量的 **Identity Gateway** 統一管理 OAuth / OIDC 認證與 JWT 簽發。

## 🔗 線上瀏覽

**https://go-authgate.github.io/slides/**

## 📑 內容簡介

投影片涵蓋以下主題：

- **三大痛點** — 為什麼需要一座統一的身分閘道
- **What is AuthGate** — 一個輕量的 Identity Gateway
- **三種 OAuth 流程** — Auth Code + PKCE、以及覆蓋瀏覽器、CLI/IoT 與服務間的三類用戶端
- **Which Flow When** — Web / SPA / Mobile 的標準流程選擇
- **Token 設計** — access 與 refresh 同表儲存、`token_category`、撤銷機制
- **Resource Server 驗證** — `aud` audience 綁定、多 API 隔離（api-a.corp / api-b.corp）
- **可觀測性** — `auth_login_total`、`http_request_duration` 等指標與稽核事件

講者：**appleboy**

## 🚀 本機預覽

投影片是單一檔案 `index.html`（已內嵌所有資源），直接用瀏覽器開啟即可：

```bash
open index.html
```

或啟動一個本機伺服器：

```bash
python3 -m http.server 8080
# 開啟 http://localhost:8080
```

## 📦 部署

本投影片透過 **GitHub Pages** 部署，來源為 `main` 分支根目錄。
更新內容後只要推送到 `main`，GitHub Pages 會自動重新部署：

```bash
git add index.html
git commit -m "Update slides"
git push origin main
```
