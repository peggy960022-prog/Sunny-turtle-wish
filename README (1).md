# 晴天烏龜祈願所

畫一顆太陽，陪 66 隻小烏龜一起迎接好天氣。

以臺灣民間祈晴習俗為靈感的春日祈願小遊戲：選擇日期與地點、畫出太陽、召集 66 隻小烏龜、寫下心願，最後完成數位祈願儀式並下載專屬祝福卡（PNG）。

🌐 線上遊玩：https://peggy960022-prog.github.io/Sunny-turtle-wish/

> 遊戲內容僅供文化體驗與娛樂，不代表宗教儀式，也不具天氣預測或改變天氣的功能；實際天氣請以氣象預報為準。

## 遊戲流程

1. **春日準備**：填寫祈願日期、地點、時段與活動類型
2. **繪製太陽**：選一種太陽，點擊畫紙放上去，可拖曳微調
3. **烏龜大集合**：一隻隻呼叫或一次呼叫全部，共 66 隻（每輪有 3～6 隻特殊造型）
4. **寫下心願**：可自訂或使用預設祈願詞
5. **誠心祈願**：Canvas 燃燒動畫（純數位象徵，不會真的燃燒任何東西）
6. **晴天祝福卡**：下載 PNG 保存

## 專案結構

```
.
├── index.html              遊戲本體（單一檔案，HTML + CSS + JS，無外部相依）
├── icon.jpg                圖示原始檔（1024×1024）
├── favicon.ico             瀏覽器分頁圖示
├── icon-32.png             32×32 圖示
├── icon-192.png            Android / PWA 圖示
├── icon-512.png            PWA 大圖示
├── apple-touch-icon.png    iOS 加到主畫面圖示（180×180）
├── og-image.png            分享預覽圖（1200×630）
├── manifest.webmanifest    PWA 設定
├── 404.html                找不到頁面時顯示
├── .nojekyll               告訴 GitHub Pages 不要用 Jekyll 處理
└── README.md
```

## 本機預覽

直接雙擊 `index.html` 即可；若要模擬網站環境：

```bash
python3 -m http.server 8000
# 開啟 http://localhost:8000
```

## 部署到 GitHub Pages

1. 把專案推送到 GitHub 的 `main` 分支
2. Repo → **Settings → Pages**
3. **Source** 選 *Deploy from a branch*，Branch 選 `main`、資料夾選 `/ (root)`，按 Save
4. 約 1～2 分鐘後，網址為 `https://<帳號>.github.io/<repo 名稱>/`

`index.html` 裡的分享預覽網址（`og:url`、`og:image`、`twitter:image`）需要是完整網址；若 repo 名稱或帳號變更，請一併修改。

## 相容性

支援近年版本的 Chrome、Safari、Edge、Firefox（手機與桌機）。已支援鍵盤操作、`prefers-reduced-motion`（減少動態效果）與安全區域（瀏海螢幕）。
