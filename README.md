# Ocean Challenge 2025

在這份報告中，我們提出了一個AI生態保育追蹤系統，這個系統為一套結合行動裝置與生成式人工智慧（LLM）的生態保育與導覽解決方案，協助民眾及生態專員共同參與環境守護與自然教育。使用者可透過手機拍照並上傳附帶GPS與時間資訊的照片，系統將利用LLM分析圖片內容，自動產生說明與判斷處理等級，再上傳至雲端資料庫。生態保育人員可即時查看待處理事項，彷彿一份共用的待辦清單（To-do List），加速生態修復行動。而在生態導覽方面，使用者亦可上傳景點照片與描述，系統將擴充文字說明與內容，供未來遊客依據位置自動顯示導覽資訊，提升旅遊體驗與環境意識。本系統不僅促進社會參與，也建立了一套低門檻、可擴充的生態資料與多媒體導覽平台。

## 團隊基本資料

**隊名**: Tech Action

**隊員**: Tiffany Gau (隊長), Mira Gau, Megan Chang, Ethan Chang, Oliver Chen, Ryan Chen, Daniel Gau

呼應本次競賽的主題"Youth in Action"，我們取隊名"Tech Action"，"Take Action"的諧音，使用科技讓大家採取行動。

## 計畫概念

我們主要是從 todo list 發想，想要開發一個可以讓大家一起幫忙保護生態的服務，同樣的技術可以很容易的延伸成導覽系統，提升環境保護的意識。

## 系統運作流程

1. 使用者透過手機上傳照片，並寫下對該照片的描述。
2. 伺服器接收到照片之後，會做如下處理：
  1. 將照片送往LLM做分析，產生分析結果以及需處理的狀態。
  2. 伺服器程式會讀出GPS座標以及拍攝時間。
  3. 如果照片包含GPS訊息：
    1. 伺服器程式會將照片送往圖形空間儲存，並取得照片的URL。
    2. 伺服器程式會將照片的URL、使用者對照片的描述、AI分析結果、AI建議處理的狀態、GPS座標、拍攝時間等資料存在資料庫上。
3. 使用者透過Web介面可以看到目前各項工作的處理狀態。
4. 管理人員透過後台管理程式可以更新各項工作的狀態。



## 使用技術

在這個計畫中，我們正在使用及考慮使用的技術如下：

**LLM**

* [Google Gemini API](https://aistudio.google.com/)

**Image Hosting**

* [imgbb](https://imgbb.com/)

**Voice Hosting**

* [vocaroo](https://vocaroo.com/)

**Database**

* [firebase](https://firebase.google.com/)
* [supabase](https://supabase.com/)

