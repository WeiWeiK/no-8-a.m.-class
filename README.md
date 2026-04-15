> [!CAUTION]
> 因部分使用者長時間（24 小時）持續運行，造成資源浪費，已新增白名單機制。<br>
> 請聯繫作者取得金鑰，並填入下方紅框欄位。<br>
> 請於點名前幾分鐘開啟使用，避免長時間掛機。(不然我會封你)<br>
>（僅適用於 v1.1.5 版本的 Extension，若已過期請移除並重新安裝套件）<br>
<img width="1899" height="1025" alt="截圖 2026-04-15 下午6 17 23" src="https://github.com/user-attachments/assets/4bffaae4-07d4-4796-a013-c8baa1d0f2c0" />


> [!WARNING]
> 本工具純屬作者無聊產物，用來測試與娛樂。  
> 沒有保證能用，也沒有每間學校都試過。  
>  
> 目前只支援「電腦版瀏覽器」且為「數字點名」。  
>  
> ✅ 已成功：
> - 國立臺灣海洋大學 (數字)
> - 天主教輔仁大學 (數字)
> - 東海大學 (數字)
> - 大同大學 (數字)
> - 淡江大學 (數字)
> - 東吳大學 (數字)
> - 虎尾科技大學 (數字)
> - 弘光科技大學 (數字)
>
> ❓ 其他學校：祝你好運，自己試
>
> 如有其他功能需求，歡迎私訊討論。

> 早八不是課，是人體開機測試。  
>  
> 鬧鐘一響，我的靈魂先起床看我一眼，說：「你加油。」然後就下線了。  
>  
> 8 點的我根本不是我，是一個連情緒都還沒載入完成的 NPC。  
>  
> 所以我不是不去上課，我只是還在載入人生。


# Demo


https://github.com/user-attachments/assets/05cf412e-7bb0-4029-8280-b7cb14a32d44








# 拒絕早八 Tronclass版
此專案僅開源客戶端（browser extension）部分。<br>
核心功能需透過後端服務支援，extension 會與遠端 server 進行通訊。<br>
<br>

## HOW
後端使用高併發分散式搜尋引擎（Distributed High-Concurrency Search Engine），<br>
針對 Tronclass 的密碼空間進行極速枚舉。<br>
<sub>#自適應併發控制（Adaptive Concurrency Control）<br>
動態調整請求速率，根據回應延遲與錯誤率即時收斂，避免觸發風控機制。</sub>
<br><br>
<sub>#代理池分流（Distributed Proxy Pooling）<br>
將請求流量拆分至多節點來源，實現橫向擴展並降低單點風險。</sub>
<br><br>
<sub>#請求隨機化（Request Randomization Layer）<br>
包含順序打亂、時間抖動（jitter）、header 擬態，讓流量呈現自然分布。</sub>
<br><br>
<sub>#優先級搜尋策略（Heuristic Prioritization）<br>
對高機率候選（如 0000、1234、8888）進行前置探測，加速命中期望值。</sub>
<br><br>
<sub>#批次並行枚舉（Batch Parallel Enumeration）<br>
將 10,000 組候選切片分發至 worker，實現近似 O(1 round-trip) 的搜尋效率。</sub>
<br>
<br>
此工具會將 session 等 Cookie 傳至後端以利運作，會怕就不要裝。

## 如何安裝
**1. 載這個**
<img width="1443" height="962" alt="image" src="https://github.com/user-attachments/assets/482a5db4-d292-4815-b937-f682987b2750" />

<br>
<br>

**2. 下載後將此zip解壓縮 將會獲取 no-8-a.m.-class-1.1 資料夾**
<br>
<br>

**3. 前往瀏覽器擴充功能管理頁面 (找不到請自己問ai)<br>**

> [!WARNING]
> 請記得開啟 開發人員模式

<br>
<br>

**4. 點擊「載入未封裝項目」並選擇剛剛解壓出來的資料夾**
<img width="1568" height="754" alt="image" src="https://github.com/user-attachments/assets/cb3ce6af-54e0-40c6-b440-5d9fbc1c8706" />
<img width="1288" height="148" alt="image" src="https://github.com/user-attachments/assets/47f8634f-4bbe-45f9-a375-c22f7d0562a6" />
<br>
<br>

**5. 大功告成 開始使用🎉**
<img width="1567" height="414" alt="image" src="https://github.com/user-attachments/assets/deb6961b-18e5-4496-9a36-3d1f9743b828" />
<br>
<br>

## 如何使用
進入 Tronclass 首頁即可看到此控制列
<img width="1570" height="1027" alt="截圖 2026-04-09 下午6 12 35" src="https://github.com/user-attachments/assets/978e5c7c-26c6-4268-80a4-34565652454d" />

<br>
<br>
按下點名他就會自己每隔一段時間抓一次了，如果有點名資訊他破解完就會給你(最快5秒內)。<br>
把自動點名打開他就會幫你自動點名，一起告別早八吧
<br>

> [!WARNING]
> 請儘量在點名前3-5分鐘掛著用
> 在此期間請勿使用 Tronclass 做任何動作

### 瀏覽器支援摘要
- Chrome/Chromium：完整支援✅
- Firefox：還未測試 我懶
- Brave：完整支援✅
- Edge：還未測試 我懶
- Safari：還未測試 我懶
