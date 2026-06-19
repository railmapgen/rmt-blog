---
title: 遇見地鐵線路圖繪製器 5.5！
date: 2026-06-16 00:00:00
lang: zh-HK
tags:
  - RMP
  - 更新
---

地鐵線路圖繪製器 5.5 來了！本次更新圍繞更自由的線路繪製、更靈活的樣式組合、常用工具管理、屬性複用，以及一批線路標識和地區樣式補充展開，讓複雜線路圖的製作過程更順手。

---

## 🧭 任意角度線段

新增「任意角度線段」，可以分別設定起點和終點的角度，並調整起終點偏移與圓角因子。它適合繪製不局限於 45°、90° 或固定方向的折線，讓線路走向更貼近真實圖面需求。

<video src="/rmt-blog/images/rmp-5-5/ray-guided-line.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🧱 通用線段樣式

新增「通用樣式」，支援把多層線條疊加成一個線路樣式。每一層都可以設定顏色、寬度、透明度、線帽、虛線長度和間隔，也可以複製、排序或刪除，用來製作特殊線路、圖例線或臨時視覺方案都更方便。

<video src="/rmt-blog/images/rmp-5-5/generic-line-style.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## ⭐ 收藏常用工具

左側工具面板新增收藏功能。常用的線路樣式、車站和雜項節點可以加入收藏，並透過「僅顯示收藏」快速過濾，減少在長列表中反覆尋找工具的時間。

<video src="/rmt-blog/images/rmp-5-5/favorite-tools.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🎛️ 線路樣式預覽圖標

線路樣式列表現在會顯示實際樣式預覽圖標。選擇樣式前就能看到大致視覺效果，尤其在倫敦、JR East、MTR、城際鐵路等樣式較多的場景下更直觀。

![線路樣式預覽圖標](/rmt-blog/images/rmp-5-5/line-style-icons.png)

---

## 📋 複製與貼上獨特屬性

右鍵選單新增「複製獨特屬性」和「貼上獨特屬性」。同類型車站、同類型雜項節點或同樣式線段之間，可以只複用獨特屬性，而不影響名稱、位置或其他基礎資訊。

<video src="/rmt-blog/images/rmp-5-5/copy-paste-specific-attrs.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🔗 一鍵選中相連同樣式線段

雙擊線段即可選中所有相連且樣式相同的線段。需要批量調整同一段線路的樣式、層級或屬性時，不再需要逐段多選。

<video src="/rmt-blog/images/rmp-5-5/select-connected-lines.mp4" autoplay loop muted playsinline style="max-width: 100%;"></video>

---

## 🚅 新幹線樣式

新增 JR East 新幹線線路樣式，可繪製帶方向箭頭質感的線路。它支援常見線段類型，並可配合終端裝飾一起使用。

![新幹線樣式](/rmt-blog/images/rmp-5-5/shinkansen.png)

---

## 🚉 JR East 終端裝飾

JR East 單色樣式和網狀圖案樣式新增終端裝飾設定，可選擇「終點」或「其他線區」等顯示方式，並指定裝飾顯示在線段起點或終點。

![JR East 終端裝飾 1](/rmt-blog/images/rmp-5-5/jr-east-terminal-decoration-1.png)

![JR East 終端裝飾 2](/rmt-blog/images/rmp-5-5/jr-east-terminal-decoration-2.png)

---

## 🚇 倫敦地鐵線路標牌

新增倫敦地鐵線路標牌節點，支援普通線路標牌與步行標牌。標牌可填寫線路名、步行目標和距離，也可以疊加多個項目，適合製作更接近倫敦圖面風格的說明與換乘資訊。

![倫敦地鐵線路標牌](/rmt-blog/images/rmp-5-5/london-tube-line-badge.png)

---

## 🏙️ 武漢軌道交通標識

新增武漢軌道交通線路標識節點，同時武漢換乘站支援 3 線及以上換乘圖標和換乘資訊編輯。製作武漢風格線路圖時，線路編號和換乘圖形可以更完整地呈現。

![武漢軌道交通標識](/rmt-blog/images/rmp-5-5/wuhan-rt-badges.png)

---

## 🚏 深圳設施圖標

新增深圳火車站、城際鐵路、輪渡、有軌電車和機場設施圖標，便於在深圳相關線路圖中標註更多交通接駁資訊。

![深圳設施圖標](/rmt-blog/images/rmp-5-5/shenzhen-facilities.png)

---

## ✨ 其他改進

- 重構了線段路徑的資料結構與計算方式，現在能更穩定地參與偏移、描邊、輪廓和圓角處理。
- 創建車站時可直接使用空白站名，適合後續統一補名或製作無站名草圖。
- 車站名稱支援直接拖動到自訂位置。
- 節點座標輸入更穩健，非法值不會直接寫入項目。
- 更新上海 2024 設施圖標。
- 廣東城際鐵路樣式新增灰色選項。
- 廣州地鐵線路標識支援 APM 樣式線框。
- 北京地鐵換乘圖標更新並修正位置。
- 長沙換乘站新增顏色翻轉選項，並修正站名位置。
- 優化畫布拖拽、縮放、節點拖動、網格線與選中高亮等體驗，觸控板和移動端操作也更順手。
- 改進圖片和 SVG 匯出清理與 Safari 相容性，並修復空畫布、署名選項和特殊 SVG path 的匯出問題。
