# Yun｜PR & MKT Freelancer 接案作品集

一個單頁式（Landing Page）接案作品集網站，展示里長 Yun 在媒體公關、社群經營、活動企劃等領域的服務項目與作品案例，並提供聯繫方式。

## 功能

- **導覽列**：置頂固定導覽列，含品牌 Logo、Instagram／Threads 社群連結與快速聯繫按鈕
- **首頁主視覺（Hero）**：全螢幕背景圖搭配標語、副標與行動呼籲按鈕（與我聯繫／觀看作品）
- **成績單區塊**：採訪報導數、籌辦活動場次、經營社群帳號數、累計追蹤人數等數字，滾動至畫面內時會有動態計數效果（支援 `prefers-reduced-motion`）
- **里民服務區**：採訪撰稿與文字企劃、社群經營與行銷、線上線下活動企劃與專案統籌三大服務說明
- **精選作品區**：三張作品卡片，分別介紹教育品牌社群經營、政府單位活動統籌、房仲品牌公關議題操作三個案例，含成效數據
- **聯繫區塊**：提供 Email、Instagram、Threads 等聯繫連結
- **RWD 響應式設計**：已針對手機版（480px 以下）優化，包含：
  - 成績單與作品卡片在手機版改為單欄／雙欄排列
  - 所有按鈕與圖示最小尺寸 44px，觸控友善
  - 大標題字體於手機版縮小為桌面版的 75%
  - `overflow-x: hidden` 確保頁面無橫向捲動
- **視覺效果**：漸層背景動畫、柔和光暈裝飾（blob）、卡片與元素淡入動畫（支援 `prefers-reduced-motion`）

## 使用技術

- **HTML5**：語意化標籤（`nav`、`header`、`section`、`article`、`footer`）
- **CSS3**：純 CSS 實作，無外部框架
  - CSS Grid（成績單、服務項目、作品卡片自適應排版）
  - Flexbox（導覽列、按鈕列、聯繫連結排版）
  - CSS 變數（`:root` 自訂色彩系統）
  - `@media` 響應式斷點與 `clamp()` 流體字級
  - CSS `@keyframes` 動畫（背景漸層流動、光暈飄浮、淡入效果）
- **JavaScript**：僅用於成績單數字的滾動計數動畫（`IntersectionObserver` + `requestAnimationFrame`），無其他依賴
- **字型**：Google Fonts（Inter）

不依賴任何前端框架或後端服務，純前端靜態頁面。

## 如何在瀏覽器開啟

**方法一：直接開啟檔案**

1. 下載或 clone 這個專案到本機
2. 在檔案總管／Finder 中找到 `index.html`
3. 直接雙擊該檔案，或將檔案拖曳到瀏覽器視窗中即可開啟

**方法二：使用終端機指令開啟**

```bash
# macOS
open index.html

# Windows
start index.html

# Linux
xdg-open index.html
```

**方法三：使用本機伺服器（建議，畫面效果更接近正式環境）**

```bash
# 使用 Python 內建伺服器
python3 -m http.server 8000

# 接著在瀏覽器開啟
http://localhost:8000
```

## 專案結構

```
.
├── index.html              # 主頁面（HTML + CSS + 少量 JS）
├── assets/
│   ├── Logo.png             # 品牌 Logo
│   ├── yilan.jpg             # 首頁主視覺背景圖
│   ├── n-viewpoint.jpg       # 作品案例：教育品牌社群經營
│   ├── hurc.jpg              # 作品案例：政府單位活動統籌
│   ├── yc-realestate.jpeg    # 作品案例：房仲品牌公關議題操作
│   ├── instagram-icon.webp   # Instagram 圖示
│   └── threads-icon.webp     # Threads 圖示
└── README.md
```
