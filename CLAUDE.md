## Development Scripts

| 用途 | 指令 | 說明 |
| --- | --- | --- |
| 啟動開發伺服器 | `npm run dev` | localhost:5173 預覽 |
| 建置正式版本 | `npm run build` | 輸出至 dist/ |
| 預覽正式版本 | `npm run preview` | localhost:4173 預覽 dist/ |

## Code Style Guidelines

- UI 文字須使用繁體中文
- 程式碼註解須使用繁體中文
- 變數與函式命名須使用 camelCase

## 命名慣例

- JavaScript/TypeScript 檔案：使用 camelCase 或 PascalCase（元件使用）。
  - 正確：utils.js、UserProfile.jsx、apiClient.ts
  - 錯誤：utils_cool.js、userprofile.jsx
- CSS/SCSS 檔案：使用 kebab-case（例如：main-styles.css）。
