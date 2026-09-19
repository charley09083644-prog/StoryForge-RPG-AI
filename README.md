# StoryForge RPG AI v3 — Android App

這是「AI 互動英文小說 × RPG × 單字學習 × 作家模擬器」的原生 Android v3 專案。

## v3 大型更新內容
- 原生 Android App 架構，不再依賴 Node 網站伺服器
- App 內 OpenAI API Key / 文字模型 / 圖片模型設定
- API 連線測試與錯誤診斷
- 中文創作需求 → 英文小說
- 完整繁體中文對照翻譯
- 3 條分支選項 + 自訂中文劇情方向
- AI 每章示意圖
- RPG 等級 / EXP / Gold / Lexicon
- Focus / Creativity / Courage / Insight 屬性
- 任務 / 地點 / 背包
- 點英文單字查詢 + 收藏
- 中英對照 / 只看英文 / 只看中文
- 本機保存故事與進度

## API 設定
第一次開啟 App：
1. 點底部「設定」
2. 輸入你自己的 OpenAI API Key
3. 設定文字模型與圖片模型
4. 按「測試 AI 連線」

> 個人原型版會將 Key 儲存在 Android App 本機資料中。若未來公開上架，應改成自己的安全後端代理。

## Android
- Package: `com.storyforge.rpg`
- minSdk: 26
- targetSdk / compileSdk: 35
- versionName: 3.0.0

## GitHub Actions
Push 到 `main` 後，`.github/workflows/build-apk.yml` 會自動編譯 debug APK，並上傳為 Actions artifact。
