# 伴奏製作室（GitHub Pages）

## 部署

此公開 repository 的網站檔案位於根目錄。前往 **Settings → Pages**，將 **Build and deployment** 設為 **Deploy from a branch**、分支 `main`、資料夾 `/(root)`，儲存後等待部署完成。網站網址：<https://310219-dev.github.io/yolo-accompaniment/>。

## 使用注意

這是純前端音訊處理，選取的音訊留在瀏覽器中。首次使用會從 Hugging Face 載入約 172 MB 模型。GitHub Pages 無法設定跨來源隔離標頭，因此此版本強制使用單執行緒 WASM；分離速度可能較慢。輸出為 WAV 伴奏音訊，不含影片畫面。
