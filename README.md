感謝您提供專案連結。我已檢視您的 GitHub 倉庫 [AlHIO/CloudNative\_2025Final](https://github.com/AlHIO/CloudNative_2025Final)，並注意到目前的 `README.md` 檔案可能與專案內容不完全一致。根據倉庫中的目錄結構與檔案，我為您重寫了一份更符合專案實際內容的 README。

---

# CloudNative\_2025Final

本專案為 2025 年雲原生課程的期末專案，旨在建構一個基於 Django 的餐廳點餐系統，並採用雲原生架構設計，結合容器化部署、RESTful API 與 PostgreSQL 資料庫，以實現高擴展性與可維護性。

## 專案功能

* **使用者管理**：提供註冊、登入、個人資料編輯等功能。
* **菜單管理**：支援新增、修改、刪除菜品資訊，並可上傳圖片與描述。
* **訂單處理**：使用者可建立與追蹤訂單狀態。
* **評論系統**：使用者可對菜品進行評分與留言。
* **管理介面**：透過 Django Admin 管理所有模型資料。

## 專案結構

```
CloudNative_2025Final/
├── CloudNative_final/       # 主應用程式目錄
│   ├── __init__.py
│   ├── settings.py          # 設定檔
│   ├── urls.py              # URL 路由設定
│   └── wsgi.py              # WSGI 入口點
├── common/                  # 共用模組
├── menu/                    # 菜單管理應用
├── orders/                  # 訂單處理應用
├── reviews/                 # 評論系統應用
├── users/                   # 使用者管理應用
├── static/                  # 靜態檔案
├── templates/               # HTML 模板
├── manage.py                # Django 管理指令
├── requirements.txt         # 相依套件清單
└── README.md                # 專案說明文件
```



## 安裝與執行

1. **建立虛擬環境**：

   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```



2. **安裝相依套件**：

   ```bash
   pip install -r requirements.txt
   ```



3. **資料庫遷移**：

   ```bash
   python manage.py migrate
   ```



4. **啟動開發伺服器**：

   ```bash
   python manage.py runserver
   ```



5. **存取應用程式**：在瀏覽器中開啟 `http://localhost:8000/`。

## 技術棧

* **後端框架**：Django
* **資料庫**：PostgreSQL
* **容器化**：Docker（可選）
* **API 設計**：RESTful

<-----未做----->
* **部署平台**：支援雲端平台（如 AWS、GCP、Azure）
