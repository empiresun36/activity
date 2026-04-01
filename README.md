# 太陽帝國社區兒童節「認識我的家」活動網站

## 📁 檔案結構
```
activity/
├── index.html          ← 主網站（活動首頁、集章、憑證）
└── loc/
    ├── 1.html          ← 地點1 QR Code 掃描頁
    ├── 2.html          ← 地點2
    ├── ...
    └── 10.html         ← 地點10
```

## 🚀 上架步驟（GitHub Pages 免費託管）

### 步驟1：申請 GitHub 帳號
1. 前往 https://github.com
2. 點「Sign up」，填入 Email、密碼、帳號名稱

### 步驟2：建立 Repository
1. 登入後點右上角「+」→「New repository」
2. Repository name 填：`sun-empire-activity`
3. 選「Public」
4. 點「Create repository」

### 步驟3：上傳檔案
1. 點「uploading an existing file」
2. 將 index.html 拖曳上傳
3. 點「Commit changes」
4. 再建立 loc 資料夾：點「Add file」→ 建立 `loc/1.html`，重複上傳10個

### 步驟4：開啟 GitHub Pages
1. 進入 Repository → 點「Settings」
2. 左側「Pages」
3. Source 選「main」→ 點「Save」
4. 等1-2分鐘，會顯示網址：
   `https://你的帳號.github.io/sun-empire-activity/`

## 🔗 QR Code 對應網址
將以下網址分別製作成 QR Code（用 qr-code-generator.com 等免費網站）：

地點1 社區大門：    https://你的帳號.github.io/sun-empire-activity/loc/1.html
地點2 中庭花園：    https://你的帳號.github.io/sun-empire-activity/loc/2.html
地點3 游泳池：      https://你的帳號.github.io/sun-empire-activity/loc/3.html
地點4 兒童遊樂場：  https://你的帳號.github.io/sun-empire-activity/loc/4.html
地點5 社區信箱：    https://你的帳號.github.io/sun-empire-activity/loc/5.html
地點6 健身房：      https://你的帳號.github.io/sun-empire-activity/loc/6.html
地點7 停車場：      https://你的帳號.github.io/sun-empire-activity/loc/7.html
地點8 垃圾資源回收站：https://你的帳號.github.io/sun-empire-activity/loc/8.html
地點9 管理室：      https://你的帳號.github.io/sun-empire-activity/loc/9.html
地點10 社區布告欄：  https://你的帳號.github.io/sun-empire-activity/loc/10.html

## 🎨 客製化地點名稱
打開 index.html，找到以下這段（約第 220 行），修改地點名稱和 emoji：

const LOCATIONS = [
  { id: 1, name: '社區大門', emoji: '🏠' },
  { id: 2, name: '中庭花園', emoji: '🌸' },
  ...
];

## 📱 使用說明（給參加者）
1. 掃描社區各處的 QR Code 立牌
2. 手機自動開啟網頁並記錄
3. 集滿10個後點「領取完成憑證」
4. 填入戶號+電話，截圖憑證
5. 至服務台換禮物

## ⚠️ 注意事項
- 印章記錄儲存在手機瀏覽器（localStorage）
- 換瀏覽器或清除快取會遺失，請直接截圖憑證
- 完成憑證防偽碼含日期+電話尾碼，可供核對
