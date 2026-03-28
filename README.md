# 🤖 FB Auto Register — OpenClaw + AdsPower 自動註冊 Facebook 帳號

> AI Agent 自動完成 85% 的 FB 註冊流程，55 秒搞定（手動要 10-15 分鐘）

---

## 這是什麼？

一套基於 **OpenClaw（AI Agent）+ AdsPower（指紋瀏覽器）** 的自動化 Facebook 帳號註冊工具。

AI 負責思考和操作，AdsPower 負責提供獨立的瀏覽器環境，讓每個帳號看起來都像來自不同裝置的真人。

## 🎯 功能

- ✅ 自動填寫註冊表單（姓名、Email、密碼）
- ✅ 自動選擇生日和性別（處理 Facebook 的特殊 ARIA UI）
- ✅ 自動完成 Email 驗證
- ✅ 自動處理安全檢查點
- ✅ 模擬真人打字速度（delay 50ms）
- ✅ 每個帳號獨立指紋環境（Canvas、WebGL、AudioContext）
- ⚠️ 影片自拍驗證需人工介入（觸發率 5-15%）

## 🏗️ 架構

```
OpenClaw AI Agent
    │
    ▼
AdsPower Local API (port 50325)
    │
    ▼
啟動 Browser Profile（獨立指紋）
    │
    ▼
Puppeteer CDP 控制
    │
    ▼
Facebook 註冊流程
```

## 📋 前提需求

| 工具 | 用途 | 必要 |
|------|------|------|
| [AdsPower](https://www.adspower.net/share/Qd0snp) | 指紋瀏覽器 + 帳號隔離 | ✅ |
| [OpenClaw](https://openclaw.ai) | AI Agent 框架 | ✅ |
| Node.js 18+ | 執行腳本 | ✅ |
| 住宅 IP 代理 | 降低驗證觸發率 | 🔶 強烈建議 |
| Gmail 帳號 | 接收驗證碼 | ✅ |

## 🚀 快速開始

```bash
# 1. Clone
git clone https://github.com/maxtsai01/fb-auto-register.git
cd fb-auto-register

# 2. 安裝依賴
npm install

# 3. 設定帳號資料
cp config.example.json config.json
# 編輯 config.json 填入你的資料

# 4. 確保 AdsPower 已啟動
# AdsPower API 預設 port: 50325

# 5. 執行
node register.js
```

## ⚙️ 設定檔說明

```json
{
  "adspower": {
    "apiBase": "http://localhost:50325",
    "apiKey": "你的 AdsPower API Key"
  },
  "accounts": [
    {
      "profileId": "AdsPower Profile ID",
      "firstName": "John",
      "lastName": "Doe",
      "email": "john@gmail.com",
      "password": "安全密碼",
      "birthday": { "month": "Apr", "day": "15", "year": "1990" },
      "gender": "male"
    }
  ],
  "options": {
    "typingDelay": 50,
    "proxy": "socks5://IP:PORT"
  }
}
```

## 📊 成功率

| 環境 | 影片驗證觸發率 | 整體成功率 |
|------|--------------|-----------|
| 數據中心 IP + 普通瀏覽器 | 60-80% | 低 |
| 住宅 IP + AdsPower | 5-15% | 高 |
| 住宅 IP + AdsPower + 養號 | <5% | 極高 |

## ⚠️ 免責聲明

> 本工具僅供學習和研究目的。
> - 使用者需自行遵守 Facebook 服務條款
> - 帳號被封屬於第三方平台行為，非本工具責任
> - 不包含一對一技術支援
> - 需要客製化？用 OpenClaw 自己改，或付費委託

## 🔗 相關資源

- [AdsPower Agentic Browser 官方介紹](https://www.adspower.com/blog/adspower-ai-agentic-browser)
- [OpenClaw + AdsPower 自動註冊實測](https://www.adspower.com/blog/can-ai-agents-register-facebook-accounts-automatically)
- [OpenClaw + AdsPower 自動登入 Google](https://www.adspower.com/blog/use-openclaw-ai-agent-to-login-google-account-with-adspower)

---

## 💰 完整版

這個 Public 版本是架構說明和概念展示。

**完整版包含：**
- 可直接執行的註冊腳本
- Email 驗證碼自動擷取
- 安全檢查點自動處理
- 批量註冊支援
- 失敗重試機制

👉 私訊 [@10000allison](https://www.instagram.com/10000allison/) 取得完整版

---

*Built with 🦞 OpenClaw + 🔒 AdsPower*
