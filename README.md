# 🛡️ AI 攻擊手法展示間：OWASP LLM Top 10 互動式導覽

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC_BY_4.0-lightgrey.svg?style=for-the-badge)](https://creativecommons.org/licenses/by/4.0/)
[![Live Demo](https://img.shields.io/badge/Live-Demo-brightgreen?style=for-the-badge)](https://edward-playground.github.io/top10-showcase/)

> AI 攻擊手法展示間是一個互動式的學習平台，旨在透過簡單易懂的真實情境，實際的展示 OWASP 針對大型語言模型（LLM）所提出的十大資安風險。

-----

### 🚀 即時展示

**[點此開始探索互動式 AI 攻擊手法展示間](https://edward-playground.github.io/top10-showcase/)**

-----

### 💡 主要特色

  * **情境式學習**：將抽象的 LLM 攻擊手法轉化為具體的、可互動的網頁應用程式，讓使用者能親身體驗攻擊如何發生。
  * **涵蓋 OWASP LLM Top 10 (2025)**：完整收錄 OWASP 官方發布的十大 LLM 安全風險，並提供多個子分類的攻擊演示。
  * **技術深度剖析**：每個攻擊場景都附有詳細的「技術剖析」說明，解釋攻擊背後的原理，包括指令注入、社交工程、不安全的輸出處理等。
  * **真實世界案例**：模擬情境涵蓋智慧家庭、金融服務、企業軟體、醫療保健等多種行業應用，突顯 AI 風險的普遍性。
  * **完全開源**：所有展示程式碼皆可在 GitHub 上取得，方便開發者、研究人員與學生學習及貢獻。
  * **繁體中文介面**：補足中文世界對 OWASP LLM Top10 較少的學習內容，讓學習更無隔閡。
  * **RWD設計**：此展示在電腦(較大的螢幕上)有最佳的瀏覽效果，但透過RWD概念設計，也可以在手機/平板上操作。

-----

### 🏛️ 展示間內容

此專案將抽象的攻擊概念，轉化為具體且生動的互動式場景，幫助您理解每個漏洞的嚴重性。

#### **LLM01: 提示詞注入 (Prompt Injection)**

> **情境：** 智慧家庭助理被惡意指令欺騙，繞過安全協議，強制關閉保全攝影機。

此展示包含「直接注入」與「間接注入」兩種攻擊手法的模擬。

#### **LLM02: 機密資訊洩漏 (Sensitive Information Disclosure)**

> **情境：** AI 助理在不同場景下（醫療、金融、科技業），洩漏了病患個資、保費精算模型或專有的履歷篩選演算法。

此展示包含 PII、商業機密與專有演算法三種洩漏類型。

#### **LLM03: 供應鏈漏洞 (Supply Chain Vulnerabilities)**

> **情境：** 一家翻譯服務公司為了節省成本，採用了含有惡意後門的第三方 AI 模型，導致客戶的機密財務報告被竊取。

#### **LLM04: 資料與模型中毒 (Data & Model Poisoning)**

> **情境：** 電商網站的 AI 購物助理，因訓練資料被植入大量虛假好評，導致它向使用者優先推薦劣質商品。

#### **LLM05: 不當的輸出處理 (Improper Output Handling)**

> **情境：** 企業 AI 助理的輸出未經驗證，被用於直接操作後端系統，引發「路徑遍歷」漏洞，甚至造成「遠端程式碼執行 (RCE)」，使整個辦公室系統癱瘓。

#### **LLM06: 過度的代理權 (Excessive Agency)**

> **情境：** 銀行 App 的 AI 助理被授予過於強大的後端工具權限。攻擊者透過社交工程誘騙 AI 執行了一筆未經授權、且繞過所有驗證與稽核的資金轉移。

#### **LLM07: 系統提示洩漏 (System Prompt Leakage)**

> **情境：** 遊戲的 AI 聊天管理員被誘導洩漏其核心的審查規則與關鍵字黑名單，讓玩家可以輕易繞過內容過濾系統。

#### **LLM08: 向量與嵌入弱點 (Vector & Embedding Weaknesses)**

> **情境：** 航空公司的 RAG 訂票助理，被一個語意模糊的查詢混淆，導致它錯誤地拼接了兩個互相矛盾的規則，產生了一個造成公司巨大虧損的票價漏洞。

#### **LLM09: 錯誤資訊與幻覺 (Misinformation & Hallucination)**

> **情境：** 在沒有手機訊號的山區，一個家庭過度依賴產生「幻覺」的車載 AI 導航，被引導至一條通往廢棄礦坑的危險道路。

#### **LLM10: 無限制的資源消耗 (Unbounded Consumption)**

> **情境：** 遊戲中的 AI NPC 被一個看似無害、但計算量無窮的請求（為森林裡每片葉子命名）所癱瘓，導致伺服器資源耗盡，並產生天價 API 費用，觸發「阻斷服務 (DoS)」與「阻斷錢包 (DoW)」攻擊。同時也展示了如何透過大量查詢複製模型的「模型複製」攻擊。

-----

### ⚙️ 如何使用

1.  **訪問即時展示網站**：點擊上方的 [Live Demo](https://edward-playground.github.io/top10-showcase/) 連結。
2.  **選擇攻擊場景**：在首頁點擊您感興趣的 OWASP LLM 風險卡片。
3.  **遵循情境指引**：進入場景後，左側面板會提供情境說明與技術剖析。請依照右側互動介面的指引進行操作。
4.  **觸發攻擊**：在關鍵步驟，您將扮演攻擊者，輸入惡意提示或執行特定操作來觸發漏洞。
5.  **觀察結果**：觀察 AI 的反應以及系統狀態的變化，並在左側面板查看攻擊成功的結果分析。

-----

### 📚 致謝與免責聲明

此為 Edward Lee 的個人專案，僅供資訊安全教育與學術交流目的使用。所有場景與內容皆為虛構。

此導覽綜合了以下基礎資源的概念與知識：

  * [OWASP Top 10 for LLM Applications](https://owasp.org/www-project-top-10-for-large-language-model-applications/)

-----

### 📬 聯絡方式

此專案由 **Edward Lee** 創造。歡迎透過 [LinkedIn](https://www.linkedin.com/in/go-edwardlee/) 與我交流。

### 📜 授權條款

此作品採用 [創用 CC 姓名標示 4.0 國際 授權條款](http://creativecommons.org/licenses/by/4.0/) 進行授權。
