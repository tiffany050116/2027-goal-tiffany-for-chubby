# 2027 創新行銷部業績規劃

可直接部署的靜態網站，包含 KEYLM 開發、Ronnie 工作安排、綠川工作安排、NEXT STEP 與參考資料。

## 檔案結構

- `index.html`：完整首頁，內含 HTML、CSS 與 JavaScript。
- `.nojekyll`：讓 GitHub Pages 直接提供靜態檔案。
- `.gitignore`：排除電腦與編輯器的暫存設定。
- `README.md`：專案與發布說明。

不需要安裝套件、執行建置或設定 API 金鑰。沒有外部 CSS 或 JavaScript 相依套件；參考資料與原始文件連結需要網路才能開啟。

## 本機開啟

直接用瀏覽器開啟 `index.html`。

亦可在專案資料夾啟動本機靜態伺服器：

```bash
python3 -m http.server 8000
```

然後開啟 `http://localhost:8000`。

## 上傳 GitHub

1. 建立 GitHub repository。
2. 解壓縮本專案，將資料夾內的檔案上傳至 repository 根目錄，確保根目錄有 `index.html`。請上傳解壓後的檔案，而非只上傳 ZIP。
3. 提交變更。

如果使用 Git 指令，請在本專案資料夾執行，並把最後一行的網址替換為自己的 repository：

```bash
git init
git add .
git commit -m "Add 2027 marketing plan website"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

## GitHub Pages 發布

在 repository 的 Pages 設定中，選擇從分支發布，來源設為 `main` 分支的根目錄。部署完成後，使用 GitHub 提供的網站網址開啟。

本專案為純靜態網頁，本身沒有登入或存取控管。是否開放網站瀏覽，請依 repository 與網站發布設定管理。

## 修改內容與樣式

用文字編輯器開啟 `index.html`：

- `<style>`：顏色、字級、段落卡片、桌機／手機版與列印版排版。
- `<body>`：完整內容、側邊目錄及參考資料。
- `<script>`：頁內導覽狀態及列印按鈕。

使用 UTF-8 編碼儲存。原始文件連結維持原有位置，可自行替換。
