# 今天換你上班｜數感實驗室跨部門工作體驗遊戲（對外版）

九個部門，九種上班日。單機網頁遊戲，不需要後端，打開 `index.html` 就能玩。

## 資料夾內容

| 檔案 | 說明 |
| --- | --- |
| `index.html` | 遊戲本體（所有程式和樣式都在這個檔案裡） |
| `chars/` | 19 張人物圖片：九個部門的半身圖與頭像、首頁的五人合照 |
| `.nojekyll` | 告訴 GitHub Pages 不要用 Jekyll 處理，請保留 |

## 放上 GitHub Pages

1. 在 GitHub 建立一個新的 repository（例如 `workday-game`），設為 Public。
2. 把這個資料夾裡的所有檔案（包含 `chars` 資料夾和 `.nojekyll`）上傳到 repository 的根目錄。
   - 網頁上傳：在 repository 頁面按「Add file → Upload files」，把檔案拖進去，再按「Commit changes」。
   - `.nojekyll` 是隱藏檔，用網頁上傳時若看不到，可以在 GitHub 上「Add file → Create new file」建立一個空白的 `.nojekyll`。
3. 到 repository 的「Settings → Pages」：
   - Source 選「Deploy from a branch」
   - Branch 選 `main`、資料夾選 `/ (root)`，按 Save。
4. 等 1～2 分鐘，頁面上方會出現網址，例如 `https://你的帳號.github.io/workday-game/`。

## 和 claude.ai 版本的差別

- 沒有「同事留言板」：留言板需要 claude.ai 的資料庫，對外版已移除首頁和結果頁的留言板按鈕。
- 其他內容（九個部門、限時事件、結果頁）與 claude.ai 版本相同。

## 注意

- 遊戲會從網路載入 React、htm（cdnjs、unpkg）和 Google Fonts 字型，玩家需要連網。
- 遊戲不會儲存或上傳任何玩家資料；重新整理頁面就會回到首頁。
