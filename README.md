# 矯正諮詢模擬演練 · 回饋單

專為矯正諮詢模擬器設計的演練回饋表單。純靜態 HTML，無需後端，可直接部署至 GitHub Pages。

---

## 使用方式

### 線上使用（GitHub Pages）

直接開啟部署後的網址即可使用，無需安裝任何軟體。

### 本地使用

下載 `feedback-form.html`，用瀏覽器（Chrome / Edge / Safari）開啟即可。

---

## 功能說明

| 區塊 | 內容 |
|------|------|
| A 結果摘要 | 日期、組別、輪次、難度、患者情境、信任分數與狀態 |
| B 本次總評 | 一句話總評、做得好的地方、需修正的地方、卡住核心原因 |
| C 核心能力評估 | 關係建立、需求挖掘、說明能力、推進能力（佳／可加強／不足）|
| D 信任建立指標 | 七項行為逐一勾選（有做到／部分做到／未做到）|
| E 失分風險檢核 | 七項常見失分行為點選標記，加上最明顯失分習慣填寫 |
| F 關鍵對話截點 | 最多三個回合，每回合含患者原話、學員回應、效果、改法 |
| G 患者推進判讀 | 四個狀態選一，避免誤把「沒生氣」當成功 |
| H 下次行動 | 保留、停止、刻意練習三格，收斂成可執行動作 |

**匯出 PDF**：填寫完畢後點右上角「匯出 PDF」，瀏覽器自動下載，檔名含日期。

---

## 部署至 GitHub Pages

1. 將 `feedback-form.html` 上傳至你的 GitHub repo
2. 進入 repo 的 **Settings → Pages**
3. Source 選擇 `Deploy from a branch`，Branch 選 `main`，資料夾選 `/ (root)`
4. 儲存後約 1 分鐘，網址格式如下：

```
https://<你的帳號>.github.io/<repo名稱>/feedback-form.html
```

---

## 技術說明

- 純 HTML / CSS / JavaScript，單一檔案，無框架依賴
- PDF 匯出使用 [jsPDF](https://github.com/parallax/jsPDF) + [html2canvas](https://github.com/niklasvh/html2canvas)，透過 CDN 載入，不需本地安裝
- 所有資料僅存在瀏覽器當前頁面，不會上傳至任何伺服器

---

## 檔案結構

```
repo/
└── feedback-form.html   # 回饋單主檔（唯一需要的檔案）
└── README.md
```
