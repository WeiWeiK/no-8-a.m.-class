> 早八不是課，是人體開機測試。  
>  
> 鬧鐘一響，我的靈魂先起床看我一眼，說：「你加油。」然後就下線了。  
>  
> 8 點的我根本不是我，是一個連情緒都還沒載入完成的 NPC。  
>  
> 所以我不是不去上課，我只是還在載入人生。

# Tronclass 點名神器
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


## 如何使用


### 瀏覽器支援摘要
- Chrome/Chromium：完整支援✅
- Firefox：還未測試 我懶
- Brave：還未測試 我懶
- Edge：還未測試 我懶
- Safari：還未測試 我懶
