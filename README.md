# 🎨 30 Theme Switcher — Smith Theme OPT

一個具備 30 種完整視覺主題、即時切換、附客戶留言功能的響應式網站。

## ✨ 功能特色
- ✅ 30 種獨特主題（不同 Layout、背景、字型、按鈕）
- ✅ RWD 響應式設計（手機、平板、桌機）
- ✅ 即時主題切換（無需重新載入）
- ✅ 客戶留言功能（選擇主題 + 填寫資料）
- ✅ 自動寄信至 rueishian.chen@gmail.com（Formspree）
- ✅ 自動發送 Telegram 通知

---

## 📧 Email 設定（Formspree — 必做）

> Formspree 是免費的表單服務，免後端即可收信。

1. 前往 [formspree.io](https://formspree.io) 註冊帳號
2. 點 **+ New Form**，Email 填入 `rueishian.chen@gmail.com`
3. 建立後，複製你的 **Form ID**（格式如 `xabcdefg`）
4. 開啟 `index.html`，搜尋：
   ```
   https://formspree.io/f/xvgaogqv
   ```
   將 `xvgaogqv` 替換成你自己的 Form ID
5. 完成後部署即可收信

---

## 🚀 部署至 GitHub + Render

### Step 1：推送至 GitHub
```bash
git init
git add .
git commit -m "Smith Theme OPT — 30 themes with contact form"
git remote add origin https://github.com/你的帳號/theme-switcher.git
git push -u origin main
```

### Step 2：部署至 Render
1. 登入 [render.com](https://render.com) → **New → Web Service**
2. 連結你的 GitHub Repository
3. 設定：
   - **Environment**: Node
   - **Build Command**: `npm install`
   - **Start Command**: `npm start`
4. 點 **Create Web Service** — 幾分鐘後即有公開網址

---

## 📱 Telegram 通知
Token 和 Chat ID 已內建於 `index.html`，部署後即自動生效，無需額外設定。

## 🗂 檔案說明
| 檔案 | 用途 |
|------|------|
| `index.html` | 主頁面（30主題 + 留言功能） |
| `server.js` | Express 靜態伺服器 |
| `package.json` | Node 設定 |
| `README.md` | 本說明文件 |
