# 伴奏製作室（GitHub Pages）

## 建立公開網站

1. 在 GitHub 建立一個新的 **Public** repository（例如 `yolo-karaoke`）。不要使用 `timcsy/demucs-web` 原始碼庫。
2. 把此資料夾內的所有檔案上傳到 repository 根目錄（包含 `.nojekyll`）。
3. 前往 **Settings → Pages**，將 **Build and deployment** 設為 **Deploy from a branch**、分支 `main`、資料夾 `/(root)`，然後儲存。
4. 等待 GitHub Pages 部署完成，網站網址會是 `https://<GitHub 使用者名稱>.github.io/<repository 名稱>/`。

## 使用注意

此為純前端處理。音訊留在瀏覽器，首次使用會從 Hugging Face 下載約 172 MB 的模型。GitHub Pages 無法設定所需的跨來源隔離標頭，所以此版本強制使用單執行緒 WASM；分離會比本機多執行緒版本慢。分離結果是 WAV 伴奏，沒有影片畫面輸出。