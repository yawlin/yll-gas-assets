# Google Apps Script (GAS) Assets Repository

這個倉庫專門用於託管 **Google Apps Script** 專案所需的靜態資源（如圖示、Logo 與圖片）。透過 GitHub 的 CDN 機制，為 GAS 的 `manifest` 檔案提供穩定的 `logoUrl` 連結。

## 🚀 快速獲取圖片連結 (Direct Link)

為了在 `appsscript.json` 中正確顯示圖示，請務必使用 **Raw** 原始檔案連結：

1. 點擊下表中的檔案路徑。
2. 在 GitHub 介面點擊 **"Download raw file"** 或 **"Raw"** 按鈕。
3. 複製瀏覽器網址列的 URL（應以 `raw.githubusercontent.com` 開頭）。

| 資產名稱 | 用途 | 解析度 | 原始連結 (範例) |
| :--- | :--- | :--- | :--- |
| `book_4.png` | Add-on 主要 Logo | 128x128 | [點此獲取](https://raw.githubusercontent.com/yawlin/gas-assets/main/book_4.png) |

## 🛠 配置說明 (Configuration)

在您的 `appsscript.json` 檔案中，請依照以下方式設定：

```json
{
  "addOns": {
    "common": {
      "name": "您的外掛名稱",
      "logoUrl": "[https://raw.githubusercontent.com/你的用戶名/gas-assets/main/book_4.png](https://raw.githubusercontent.com/你的用戶名/gas-assets/main/book_4.png)"
    }
  }
}
