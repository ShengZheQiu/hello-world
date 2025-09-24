# GeoBingAn v2 第三方元件清單報告

**報告日期**: 2025-09-24
**系統版本**: geoBingAn v2
**符合規範**: 資安法第三方軟體揭露要求

---

## 📋 執行摘要

根據資安法規範，涉及利用非受託者自行開發之系統或資源者，應標示非自行開發之內容與其來源及提供授權證明。本報告詳細列出 **geoBingAn v2** 系統中所有第三方軟體元件、開源授權條款、商用軟體廠商及使用之GenAI工具。

## 🏗️ 系統架構總覽

GeoBingAn v2 採用三層架構設計：

### 🖥️ **geoBingAn_v2_frontend** (前端系統)
- **技術棧**: React + TypeScript + Material-UI
- **地圖引擎**: Cesium (3D) + Mapbox (2D)
- **主要功能**: 地理空間資料視覺化、表單管理、報告檢視

### 🔬 **geoBingAn_v2_rag** (RAG 知識處理引擎)
- **技術棧**: Python + Flask + LangChain
- **AI模型**: Gemini 2.5 Pro
- **主要功能**: PDF文件解析、建築安全報告分析

### 🏗️ **geoBingAn_v2_backend** (後端系統)
- **技術棧**: Django + PostgreSQL + Redis
- **特殊功能**: 區塊鏈整合、MCP ChatGPT整合
- **主要功能**: API服務、資料管理、認證授權

---

## 📊 第三方元件詳細清單

### **1. Frontend 前端元件 (geoBingAn_v2_frontend)**

| 第三方軟體名稱 | 版本 | 開源授權條款 | 開源授權連結 | 商用軟體廠商 |
|---|---|---|---|---|
| React | 18.3.1 | MIT | https://github.com/facebook/react/blob/main/LICENSE | Meta/Facebook |
| Material-UI (MUI) | 6.4.0 | MIT | https://github.com/mui/material-ui/blob/master/LICENSE | MUI |
| Cesium | 1.125 | Apache-2.0 | https://github.com/CesiumGS/cesium/blob/main/LICENSE.md | Cesium GS Inc |
| Mapbox GL | 3.9.3 | BSD-3-Clause | https://github.com/mapbox/mapbox-gl-js/blob/main/LICENSE.txt | Mapbox Inc |
| Redux Toolkit | 2.5.0 | MIT | https://github.com/reduxjs/redux-toolkit/blob/master/LICENSE | - |
| React Router | 7.1.2 | MIT | https://github.com/remix-run/react-router/blob/main/LICENSE.md | - |
| Axios | 1.7.9 | MIT | https://github.com/axios/axios/blob/master/LICENSE | - |
| i18next | 25.4.2 | MIT | https://github.com/i18next/i18next/blob/master/LICENSE | - |
| React Beautiful DnD | 13.1.1 | Apache-2.0 | https://github.com/atlassian/react-beautiful-dnd/blob/master/LICENSE | Atlassian |
| Vite | 6.1.0 | MIT | https://github.com/vitejs/vite/blob/main/LICENSE | - |
| TypeScript | 5.6.2 | Apache-2.0 | https://github.com/Microsoft/TypeScript/blob/main/LICENSE.txt | Microsoft |
| Vitest | 3.2.4 | MIT | https://github.com/vitest-dev/vitest/blob/main/LICENSE | - |
| ESLint | 9.18.0 | MIT | https://github.com/eslint/eslint/blob/main/LICENSE | - |
| Tailwind CSS | 3.4.17 | MIT | https://github.com/tailwindlabs/tailwindcss/blob/master/LICENSE | - |

### **2. RAG Module RAG模組 (geoBingAn_v2_rag)**

| 第三方軟體名稱 | 版本 | 開源授權條款 | 開源授權連結 | 商用軟體廠商 |
|---|---|---|---|---|
| Python | 3.11 | PSF | https://docs.python.org/3/license.html | Python Software Foundation |
| Flask | 2.3.x | BSD-3-Clause | https://github.com/pallets/flask/blob/main/LICENSE.rst | - |
| LangChain | 0.1.0 | MIT | https://github.com/langchain-ai/langchain/blob/master/LICENSE | LangChain Inc |
| ChromaDB | 0.4.18 | Apache-2.0 | https://github.com/chroma-core/chroma/blob/main/LICENSE | - |
| Sentence Transformers | 2.2.2 | Apache-2.0 | https://github.com/UKPLab/sentence-transformers/blob/master/LICENSE | - |
| PyPDF2 | 3.0.1 | BSD-3-Clause | https://github.com/py-pdf/PyPDF2/blob/main/LICENSE | - |
| pdfplumber | 0.10.3 | MIT | https://github.com/jsvine/pdfplumber/blob/stable/LICENSE.txt | - |
| Google GenerativeAI | 0.3.2 | Apache-2.0 | https://github.com/google/generative-ai-python/blob/main/LICENSE | Google |
| FAISS | 1.7.4 | MIT | https://github.com/facebookresearch/faiss/blob/master/LICENSE | Meta/Facebook |
| Pandas | 2.1.3 | BSD-3-Clause | https://github.com/pandas-dev/pandas/blob/main/LICENSE | - |
| NumPy | 1.26.2 | BSD-3-Clause | https://github.com/numpy/numpy/blob/main/LICENSE.txt | - |
| OpenPyXL | 3.1.2 | MIT | https://github.com/theorchard/openpyxl/blob/master/LICENCE.rst | - |

### **3. Backend 後端系統 (geoBingAn_v2_backend)**

| 第三方軟體名稱 | 版本 | 開源授權條款 | 開源授權連結 | 商用軟體廠商 |
|---|---|---|---|---|
| Django | 4.2.7 | BSD-3-Clause | https://github.com/django/django/blob/main/LICENSE | Django Software Foundation |
| Django REST Framework | 3.14.0 | BSD-2-Clause | https://github.com/encode/django-rest-framework/blob/master/LICENSE.md | - |
| PostgreSQL | 15 | PostgreSQL License | https://www.postgresql.org/about/licence/ | PostgreSQL Global Development Group |
| PostGIS | 3.3 | GPL-2.0 | https://github.com/postgis/postgis/blob/master/COPYING | - |
| Redis | 5.0.1 | BSD-3-Clause | https://github.com/redis/redis/blob/unstable/COPYING | - |
| Celery | 5.3.4 | BSD-3-Clause | https://github.com/celery/celery/blob/master/LICENSE | - |
| Web3.py | 6.11.3 | MIT | https://github.com/ethereum/web3.py/blob/master/LICENSE | - |
| GDAL | 3.6.2 | MIT/X | https://gdal.org/license.html | OSGeo |
| Gunicorn | 21.2.0 | MIT | https://github.com/benoitc/gunicorn/blob/master/LICENSE | - |
| psycopg2-binary | 2.9.7 | LGPL-3.0 | https://github.com/psycopg/psycopg2/blob/master/LICENSE | - |
| Graphene Django | 3.2.3 | MIT | https://github.com/graphql-python/graphene-django/blob/master/LICENSE | - |
| Django OAuth Toolkit | 1.7.1 | BSD-2-Clause | https://github.com/jazzband/django-oauth-toolkit/blob/master/LICENSE | - |
| Boto3 | 1.34.0 | Apache-2.0 | https://github.com/boto/boto3/blob/develop/LICENSE | Amazon |
| Scikit-learn | 1.3.0 | BSD-3-Clause | https://github.com/scikit-learn/scikit-learn/blob/main/COPYING | - |
| Matplotlib | 3.7.2 | PSF | https://github.com/matplotlib/matplotlib/blob/main/LICENSE/LICENSE | - |
| SymPy | 1.12 | BSD-3-Clause | https://github.com/sympy/sympy/blob/master/LICENSE | - |
| MCP (Model Context Protocol) | 1.0.0 | MIT | https://github.com/modelcontextprotocol/python-sdk/blob/main/LICENSE | Anthropic |

### **4. 基礎設施與部署工具**

| 第三方軟體名稱 | 版本 | 開源授權條款 | 開源授權連結 | 商用軟體廠商 |
|---|---|---|---|---|
| Docker | 24.x | Apache-2.0 | https://github.com/moby/moby/blob/master/LICENSE | Docker Inc |
| Docker Compose | 2.x | Apache-2.0 | https://github.com/docker/compose/blob/v2/LICENSE | Docker Inc |
| Nginx | 1.24 | BSD-2-Clause | http://nginx.org/LICENSE | - |
| Node.js | 20.x | MIT | https://github.com/nodejs/node/blob/main/LICENSE | - |

---

## 🤖 使用之 GenAI 工具

| GenAI 工具名稱 | 用途 | 版本/API | 提供廠商 | 授權方式 |
|---|---|---|---|---|
| **Gemini 2.5 Pro** | PDF文件解析、建築安全報告分析、多模態資料處理 | API v1beta | Google | 商用API服務 |
| **ChatGPT (MCP整合)** | 智能查詢、資料分析輔助、自然語言處理 | MCP 1.0.0 | OpenAI | 商用API服務 |
| **Claude Code** | 程式碼開發輔助、架構設計諮詢 | claude.ai/code | Anthropic | 商用服務 |

### GenAI 使用範圍說明：
1. **Gemini 2.5 Pro**: 主要用於 RAG 模組中的PDF文件自動解析和建築安全報告結構化處理
2. **ChatGPT**: 透過 MCP 協議整合，提供智能查詢和資料分析功能
3. **Claude Code**: 僅用於開發階段的程式碼輔助，不涉及生產環境資料處理

---

## 📍 主要功能模組架構

### Frontend 模組結構：
```
src/components/
├── MapView/              # 2D地圖顯示 (Mapbox)
├── ThreeDMapView/        # 3D地圖顯示 (Cesium + Resium)
├── ChartView/            # 圖表分析
├── ListView/             # 列表檢視
├── BoardView/            # 看板檢視
├── FilterPanel/          # 篩選面板
├── Forms/                # 表單管理
├── Reports/              # 報告管理
├── DragDropFormBuilder/  # 拖拉表單建構器
└── AppLayout/            # 應用程式布局
```

### Backend 應用模組：
```
apps/
├── core/                 # 核心地理空間功能
├── reports/              # 報告管理系統
├── sensors/              # 感測器資料處理
├── authentication/       # OAuth2認證
├── blockchain/           # 區塊鏈整合 (Web3.py)
├── analytics/            # 資料分析
├── api_gateway/          # API閘道
├── mcp/                  # ChatGPT MCP整合
├── groups/               # 群組管理
├── views_system/         # 檢視系統
└── credit/               # 點數系統
```

### RAG 模組結構：
```
├── backend/app.py        # Flask API服務器
├── frontend/             # React操作界面
├── ontology/             # 建築安全本體論
├── data/                 # PDF文件處理
├── scripts/              # 資料處理腳本
└── src/                  # 核心處理邏輯
```

---

## 🔒 資安合規聲明

### 開源軟體合規：
- ✅ 所有開源元件均採用 **MIT、BSD、Apache-2.0** 等商業友好的寬鬆授權
- ✅ **GPL授權軟體** (PostGIS) 僅用於資料庫層面，不影響應用程式授權
- ✅ 所有授權條款均已詳細列出，符合揭露要求

### 商用服務授權：
- ✅ **Gemini API**: Google Cloud 商用API服務，按使用量計費
- ✅ **Mapbox**: 商用地圖服務，已取得適當授權
- ✅ **Cesium**: 開源版本 (Apache-2.0)，商用功能未使用

### GenAI 使用合規：
- ✅ **資料隔離**: GenAI工具僅處理非敏感的技術文件和範例資料
- ✅ **本地部署**: 核心業務資料均在本地處理，不傳送至外部AI服務
- ✅ **開發輔助**: Claude Code 僅用於開發階段，不接觸生產資料

### 資料安全措施：
- 🔐 **加密傳輸**: 所有API通信均使用 HTTPS/TLS
- 🔐 **認證機制**: OAuth2 + JWT Token 雙重認證
- 🔐 **資料庫安全**: PostgreSQL 連線加密 + Redis 密碼保護
- 🔐 **容器安全**: Docker 映像定期更新，移除已知漏洞

---

## 📈 版本管理與維護

### 依賴性管理：
- **Frontend**: package.json + yarn.lock 鎖定版本
- **Backend**: requirements.txt 指定確切版本
- **RAG**: requirements.txt 管理Python依賴

### 安全更新策略：
- 🔄 **定期掃描**: 使用 npm audit、pip-audit 檢查漏洞
- 🔄 **自動更新**: 非破壞性安全更新自動應用
- 🔄 **測試驗證**: 所有更新均經過完整測試套件驗證

---

## 📋 合規檢查清單

- ✅ **第三方軟體名稱**: 已完整列出所有元件
- ✅ **版本資訊**: 指定確切版本號
- ✅ **開源授權條款**: 詳細標示授權類型
- ✅ **授權連結**: 提供原始授權文件連結
- ✅ **商用軟體廠商**: 標示商用元件提供商
- ✅ **GenAI 工具揭露**: 完整說明使用範圍和目的
- ✅ **資安措施**: 說明資料保護和合規措施

---

**報告產生者**: geoBingAn v2 開發團隊
**最後更新**: 2025-09-24
**下次審查**: 建議每季度更新一次

---

*本報告符合資安法第三方軟體揭露要求，所有資訊均為實際使用情況之準確記錄。*