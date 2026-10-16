# FCMS 靜境大草原 · FCMS Quiet Safari

郭怡雅神父紀念學校（FCMS）課堂噪音監測工具。全班保持安靜時，草原上的小動物會一隻隻現身；太嘈就會全部走。**聲音只在本機量度音量，不錄音、不上載、無帳號。**

A classroom noise monitor for Father Cucchiara Memorial School (FCMS). Animals come out when the class is quiet and flee when it gets loud. Audio levels are measured locally only — nothing is recorded or uploaded.

## 使用 Use

1. 開啟網頁 → 允許麥克風 → 選擇目標模式（靜默／自習／小組）
2. 投影到課室大螢幕或電子白板
3. 安靜時間累積 → 動物現身；持續超過「嘈」門檻約 1 秒 → 全部走

## 功能 Features

- 三種目標模式，各自有「靜」及「嘈」門檻
- 麥克風選擇、靈敏度調整、班別名稱（存於本機 localStorage）
- 全螢幕模式（適合白板）、空格鍵開／停
- 純靜態單檔 HTML，無依賴、無後端

## 私隱 Privacy

- 音訊經 Web Audio API 在瀏覽器內計算 RMS 音量，**不產生錄音、不傳送任何數據**
- 設定及班別名稱只存於瀏覽器 localStorage

## 部署 Deploy

GitHub Pages：`main` branch 根目錄。本地測試：

```bash
python3 -m http.server 8080
# 或直接以 file:// 開啟（部分瀏覽器限制麥克風權限，建議經 http）
```

## 致謝 Acknowledgement

概念受 [Shy Safari](https://www.shysafari.com/)（teacher.dev）啟發。本專案為獨立原創實作，未使用其代碼、素材或商標。
