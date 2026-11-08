# AntiGravity 2 工具、技能與環境規範 (ANTIGRAVITY.md)

## 環境架構與工具規範
- **作業系統**：Windows 11
- **執行環境**：PowerShell (UTF-8 編碼確保中文無亂碼)
- **版本控制**：Git + GitHub CLI (`gh`)，預設遠端 repository 為 `juliahml-ux/chyi-pharmacy-slide`。
- **Python 工具**：
  - 本地簡報打包與修圖腳本（`pack_pptx.py`、`remove_bg.py` 等），依賴 Pillow, python-pptx 等套件。

## 簡報專案技能矩陣
1. **`soil-teaching-deck`**：SOIL 六顆引擎教學簡報（概念定位、脈絡定位、架構、認知編修、風格），產出可編輯 PPTX。
2. **`html-slide-builder`**：將教材或報告轉化為離線 Reveal.js 互動網頁簡報。
3. **`soil-html-deck`**：單檔 HTML 互動簡報，支援 Chart.js 數據視覺化與離線互動。
4. **`soil-image-deck`**：高視覺張力全版純圖片簡報。
5. **`startup` / `shutdown`**：標準化開工盤點與收工同步工作流。

## 驗證標準與品質要求
- **離線可用性檢驗**：產出之 HTML 簡報必須使用本地相對路徑引用 `libs/reveal`、`libs/chartjs` 與本地圖片，確保在無外網之院內電腦順暢放映。
- **視覺清晰與認知負擔控制**：遵循「30 原則」與 SOIL 架構，字體大小與色調對比需達醫療報告放映標準。
- **權限與外部服務**：
  - 未經確認不得主動建立新的外部遠端倉庫或推送未經審核的變更。
  - Obsidian 駕駛艙僅在使用者明確指定 vault 路徑後建立。
