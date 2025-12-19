# Vibe Coding 課程文件

## Lovable 與後端的開發模式

按照模組順序一步一步做~

確保流程順利，不要嘗試修改每一個發現的問題，因為額度沒了，就沒辦法進行下去

前置作業：
1. supabase 帳號
2. github 帳號
3. 2 個 google 帳號
4. lovable 帳號 (使用邀請碼) > 關聯 github 帳號
5. ngrok

安裝軟體：
1. python、uv
2. antigravity
3. git
4. node.js
5. ngrok

模組4.5：

    Q: 如何設定管理員權限?

    A: 在資料庫中，將 user 的 role 設定為 admin 即可。

    Q: 如何設定超級管理員權限?

    A: 在資料庫中，將 user 的 role 設定為 super_admin 即可。

    Q: 如何設定一般使用者權限?

    A: 在資料庫中，將 user 的 role 設定為 customer 即可。

    Q: 如何設定客戶經理權限?

    A: 在資料庫中，將 user 的 role 設定為 manager 即可。


模組5

    https://console.cloud.google.com/

    建立新專案 > API和服務 > Google Sheets API > 啟用

    API和服務 > 建立憑證 > 服務帳戶

    服務帳戶 > 建立金鑰 > JSON > 下載 > 放入專案config資料夾中，更改檔名

    打開 JSON 檔案，找到client_email，複製到Google Sheets的共用者，給編輯權限

    建立試算表 > 複製連結中 `d/` 和 `/edit` 之間的 ID 複製到 .env 的 SPREADSHEET_ID

模組7

    Q: 遇到CORS錯誤
    
    A: 
        1. 前端設定allowedHosts，路徑包含ngrok網址
        2. 前端設定proxy，將'/auth' 轉換成 'http://localhost:8000',

