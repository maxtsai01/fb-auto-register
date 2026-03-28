# 📱 FB Auto Register — AdsPower 自動註冊 FB 帳號

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=3,8,15&height=180&section=header&text=📱%20FB%20Auto%20Register&fontSize=40&fontColor=fff&animation=fadeIn&fontAlignY=35&desc=AdsPower%20×%20龍蝦%20自動養號&descSize=18&descAlignY=55" width="100%"/>
</p>

<p align="center">
  🧑‍💻 Created by <a href="https://instagram.com/10000allison">Allison (@10000allison)</a> | CTMaxs 龍蝦自動化團隊
</p>

---

## 🔥 一句話說完

**龍蝦 + AdsPower = 批量註冊 FB 帳號，每個帳號獨立指紋、獨立 IP，像真人一樣。**

---

## ❌ 手動養號的痛

- 一個一個註冊，要填資料、驗證、等待
- 用同一台電腦註冊多個帳號 → 被 FB 關聯封號
- 瀏覽器指紋相同 → FB 秒偵測
- 沒有代理 IP → 同一個 IP 多帳號 = 全滅
- 養到 50 個帳號要花幾天

## ✅ 用這個模組之後

- AdsPower 每個帳號獨立瀏覽器指紋
- 龍蝦用 CDP 自動操作每個瀏覽器
- 代理 IP 自動分配（每 6 帳號一個 IP）
- 註冊流程全自動：填資料 → 驗證 → 完善個資
- 18 個帳號 = 18 個「真人」

---

## 🎯 適合誰？

| 身份 | 痛點 | 解法 |
|------|------|------|
| 社群行銷 | 需要大量帳號互動 | 批量自動註冊 |
| 電商老闆 | 廣告帳號被封要備用 | 養一批備用帳號 |
| 社團經營 | 需要多帳號按讚留言 | 配合 FollowBunny 使用 |
| 代操公司 | 客戶多需要多帳號 | 規模化管理 |

---

## 🏗️ 技術架構

```
🦞 龍蝦（OpenClaw）
  ↓ API 呼叫
🌐 AdsPower（port 50325）
  ├── 帳號 1（獨立指紋 + IP-A）
  ├── 帳號 2（獨立指紋 + IP-A）
  ├── ...
  ├── 帳號 6（獨立指紋 + IP-A）
  ├── 帳號 7（獨立指紋 + IP-B）
  └── ...
  ↓ CDP 控制每個瀏覽器
📱 FB 註冊流程
  ├── 填寫個人資料
  ├── 手機/Email 驗證
  ├── 完善個資（頭像、背景）
  └── 養號行為模擬
```

---

## 🔧 包含什麼？

### Public（你現在看到的）
- ✅ AdsPower + OpenClaw 整合架構說明
- ✅ 帳號管理最佳實踐
- ✅ IP 分配策略
- ✅ 養號注意事項

### Private Core（付費版）
- 🔒 完整自動註冊腳本（Node.js）
- 🔒 AdsPower API 整合 Skill
- 🔒 自動養號行為模擬（每日登入、瀏覽、互動）
- 🔒 批量管理 Dashboard
- 🔒 封號應對 SOP
- 🔒 代理 IP 設定教學（IPFoxy/Oxylabs）

---

## ⚠️ 免責聲明

> 本工具僅供合法行銷用途。使用者需遵守 Facebook 服務條款。CTMaxs 不對因違反平台規則導致的帳號封禁負責。

---


---

## 💰 定價

| 方案 | 價格 | 內容 |
|------|------|------|
| 免費試用 | NT$0 | Public README + 架構說明 |
| 完整版 | 洽詢 | Private Core + 自動化腳本 |

👉 [立即免費領取](https://lumaint.1shop-app.com/lobster-store)

---

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=3,8,15&height=100&section=footer" width="100%"/>
</p>

<p align="center">
  Created by <a href="https://instagram.com/10000allison">Allison</a> | CTMaxs 龍蝦自動化團隊
</p>

---

## 🦞 龍蝦模組商店 Lobster Store

**💎 $100 USD/月 — 全部模組通用，訂閱即開通**

| Skill | 功能 |
|-------|------|
| 🎬 **[video-analyzer](https://github.com/maxtsai01/video-analyzer)** | AI 影片情報分析引擎 |
| 🤝 **[lobster-manus](https://github.com/maxtsai01/lobster-manus)** | AI 雙引擎協作（龍蝦×Manus） |
| 🛒 **[lobster-1shop](https://github.com/maxtsai01/lobster-1shop)** | 1Shop 電商自動化 |
| 🎯 **[lobster-adspower](https://github.com/maxtsai01/lobster-adspower)** | AdsPower 多帳號自動化 |
| 🤖 **[agent-orchestrator](https://github.com/maxtsai01/agent-orchestrator)** | 多代理協作引擎 |
| 📱 **[fb-auto-register](https://github.com/maxtsai01/fb-auto-register)** | AdsPower FB 自動註冊 |
| 🐰 **[followbunny](https://github.com/maxtsai01/followbunny-public)** | FB 社團自動互動 |
| 🌈 **[rainbow-life](https://github.com/maxtsai01/rainbow-life)** | AI 彩虹人生性格測驗 |
| 🖼️ **[ai-image-studio](https://github.com/maxtsai01/ai-image-studio)** | AI 智能圖片處理 |
| 🦞 **[lobster-ai-warbook](https://github.com/maxtsai01/lobster-ai-warbook)** | 龍蝦兵法訓練手冊 |

> 📸 私訊 [@10000allison](https://www.instagram.com/10000allison/) 訂閱 → 付款 → 全部模組即刻開通

