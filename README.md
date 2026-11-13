# LANDORA 曜域數位｜AURELIA STUDIO

此儲存庫專供曜域數位網站及「曜域 AI 助手」，與 LANDORA 房地產平台分開管理。

## 預定架構
- Cloudflare Workers Static Assets：公開網站
- Cloudflare Workers AI：生成式客服
- 真人客服：後端郵件通知；無自有寄件網域時須驗證 FormSubmit 收件信箱
- 免購買自有網域，使用 workers.dev 網址

## 上線條件
1. 匯入完整網站與 Worker 原始碼
2. 設定 wrangler.jsonc 的 AI binding 及 static assets
3. 在 Cloudflare Workers 連接此 GitHub 儲存庫並部署
4. 測試 /api/health 與 /api/chat
5. 驗證 Landora.platform@gmail.com 並實際收取真人客服測試信
6. 檢查濫用防護、隱私告知、跨裝置與八個示範頁

注意：本 README 並不表示已部署或 AI 已啟用。