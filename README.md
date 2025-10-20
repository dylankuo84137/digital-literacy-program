# 七、八年級資訊基礎能力與素養融入式學習方案

## 專案簡介

本網站為「七、八年級資訊基礎能力與素養融入式學習方案」的說明網站，採用靜態網頁設計，適合部署於 GitHub Pages。

### 核心理念
在有意義的情境中，自然地學習

## 網站結構

```
/
├── index.html          # 首頁
├── grade7.html         # 七年級實施方案
├── grade8.html         # 八年級實施方案
├── admin.html          # 行政與設備配套建議
├── 404.html           # 錯誤頁面
├── _config.yml        # Jekyll 設定檔
├── README.md          # 本說明文件
└── assets/
    ├── images/        # 圖片資源（如需要）
    └── styles.css     # 網站樣式表
```

## 部署至 GitHub Pages

### 方法一：直接透過 GitHub 網頁介面

1. **建立 GitHub Repository**
   - 登入 GitHub
   - 點擊右上角 "+" → "New repository"
   - 輸入 Repository 名稱（例如：digital-literacy-program）
   - 選擇 "Public"
   - 點擊 "Create repository"

2. **上傳檔案**
   - 在 Repository 頁面點擊 "uploading an existing file"
   - 將所有檔案（包含 assets 資料夾）拖曳上傳
   - 輸入 Commit message：「Initial commit: Upload website files」
   - 點擊 "Commit changes"

3. **啟用 GitHub Pages**
   - 進入 Repository 的 "Settings"
   - 點擊左側選單的 "Pages"
   - 在 "Source" 下拉選單選擇 "main" 分支
   - 點擊 "Save"
   - 等待 1-2 分鐘，頁面上方會顯示網站網址

4. **訪問網站**
   - 網址格式：`https://[你的GitHub使用者名稱].github.io/[repository名稱]/`

### 方法二：使用 Git 指令（進階）

```bash
# 1. 初始化本地 Git repository
git init

# 2. 加入所有檔案
git add .

# 3. 建立第一次 commit
git commit -m "Initial commit: Digital literacy learning program website"

# 4. 連結到 GitHub repository
git remote add origin https://github.com/[你的使用者名稱]/[repository名稱].git

# 5. 推送到 GitHub
git branch -M main
git push -u origin main
```

## 檔案說明

### HTML 頁面
- **index.html**：首頁，介紹方案背景、目標與整體架構
- **grade7.html**：七年級三階段實施方案（暖身週、主題任務、技能護照）
- **grade8.html**：八年級專題深化內容（資料搜尋、媒體素養）
- **admin.html**：行政配套建議（教師共備、設備管理、家長溝通）
- **404.html**：自訂錯誤頁面

### 設定檔
- **_config.yml**：Jekyll 設定檔，定義網站標題、語言等基本資訊
- **assets/styles.css**：統一樣式表，包含響應式設計與無障礙設計

## 特色功能

### 響應式設計
- 支援桌面、平板、手機等各種裝置
- 行動裝置下導覽列自動調整為垂直排列
- 文字大小與間距針對小螢幕優化

### 無障礙設計
- 所有頁面設定 `lang="zh-Hant"` 語言標記
- 採用 UTF-8 編碼
- 連結具備焦點樣式（focus outline）
- 圖片需添加 alt 屬性（如有使用）
- 語意化 HTML 結構

### 使用者體驗
- 統一的導覽列，快速切換頁面
- 返回頂部按鈕（固定於右下角）
- 卡片式設計，內容結構清晰
- 漸層色彩，視覺舒適

## 維護與更新

### 修改內容
1. 直接編輯對應的 `.html` 檔案
2. 若要修改樣式，編輯 `assets/styles.css`
3. 上傳更新後的檔案到 GitHub（或使用 `git push`）

### 新增頁面
1. 建立新的 `.html` 檔案
2. 複製現有頁面的導覽列與頁首/頁尾結構
3. 在所有頁面的導覽列中加入新頁面連結
4. 更新首頁的說明與連結

### 新增圖片
1. 將圖片放入 `assets/images/` 資料夾
2. 在 HTML 中使用相對路徑引用：
   ```html
   <img src="assets/images/filename.jpg" alt="圖片說明文字">
   ```
3. 記得添加 `alt` 屬性描述圖片內容

## 技術規格

- **編碼**：UTF-8
- **語言**：繁體中文（zh-Hant）
- **相容性**：支援現代瀏覽器（Chrome、Firefox、Safari、Edge）
- **框架**：原生 HTML + CSS（無需 JavaScript）
- **部署平台**：GitHub Pages（Jekyll）

## 授權說明

本專案為教育用途，內容版權歸專案建立者所有。如需使用或修改，請註明來源。

## 聯絡資訊

如有問題或建議，請透過以下方式聯絡：
- GitHub Issues：在 Repository 中建立 Issue
- Email：it@waldorf.ilc.edu.tw

---

**最後更新：2025年10月**