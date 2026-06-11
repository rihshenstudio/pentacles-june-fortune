# 六月星運・命運試煉 ✦ PENTACLES STUDIO

五芒星航的免費互動占卜遊戲。玩家通過三道試煉（啟動星盤 → 凝聚星能量 → 命運抽牌），
解鎖自己的 2026 六月運勢「搶先看」，完整版報告導購至官方賣場。

- 純靜態網頁（單一 `index.html`），無需後端、無需 build
- 完整版購買連結：https://portaly.cc/pentacles.studiotw

## 如何修改內容

打開 `index.html`，找到 `<script>` 區塊：

| 要改的東西 | 位置 |
|---|---|
| 12 星座運勢文案 | `SIGNS` 陣列（`theme` 主題、`kw` 關鍵字、`read` 總體運勢） |
| 塔羅指引牌訊息 | `CARDS` 陣列 |
| 鎖定章節的標題與預覽 | `showResult()` 內的 `locks` 陣列 |
| 價格 / 購買連結 | 搜尋 `NT.` 與 `portaly.cc` |

## 部署到 Vercel

1. 將本資料夾推上 GitHub（Public 或 Private 皆可）
2. 到 [vercel.com](https://vercel.com) 用 GitHub 帳號登入
3. **Add New… → Project → Import** 此 repo
4. Framework Preset 保持 **Other**，其餘設定不動，按 **Deploy**
5. 約 30 秒後取得 `https://你的專案名.vercel.app` 網址

之後只要更新 GitHub 上的檔案，Vercel 會自動重新部署。
