# La Piccola Costa｜小海岸 PWA

資料夾內容
- index.html：整個 App（圖片已內嵌）
- manifest.json：App 名稱、圖示、主題色
- sw.js：讓它離線也能打開
- icon-192.png、icon-512.png、maskable-512.png、apple-touch-icon.png、favicon-32.png：各尺寸圖示（全部放在同一層，方便用手機上傳）

## 放到網路上（任選一種，都免費）

### A. Netlify Drop（最簡單，不用註冊 Git）
1. 先解壓縮這個 zip。
2. 用電腦開啟 app.netlify.com/drop。
3. 把資料夾裡的所有檔案拖進去。
4. 幾秒後會得到一個 https 網址，這就是你的 App 網址。

### B. GitHub Pages
1. 在 GitHub 建立新的 repository（公開）。
2. 點「uploading an existing file」，一次選取全部 9 個檔案上傳，index.html 要在最外層。
3. Settings → Pages → Branch 選 main，資料夾選 /(root)，按 Save。
4. 約一分鐘後會得到 https://你的帳號.github.io/repository名稱/

## 在 Samsung 手機安裝
1. 用 Chrome 或 Samsung Internet 開啟你的網址。
2. Chrome：右上角選單 → 「安裝應用程式」或「加到主畫面」。
   Samsung Internet：選單 → 「新增頁面至」→「主螢幕」。
3. 桌面會出現小海岸圖示，點開就是全螢幕。
4. 打開一次之後，關掉網路也能使用。

## 之後更新內容
改完 index.html 後，把 sw.js 第一行的 'lpc-v1' 改成 'lpc-v2'（每次加一），再重新上傳。
這樣已安裝的手機下次打開就會拿到新版。

## 注意
- PWA 一定要 https 才能安裝，Netlify 和 GitHub Pages 都已經是 https。
- 直接在電腦上雙擊 index.html 可以看畫面，但不會有安裝與離線功能。
