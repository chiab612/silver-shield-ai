# silver-shield-ai
AWS-powered AI scam prevention assistant for seniors, families, banks, and social welfare organizations.
# Silver Shield AI｜銀髮守門人
...
## Vision
真正的防詐，不只是辨識壞人，而是在人最脆弱、最緊張、最孤單的那一刻，給他一個可以停下來確認的理由。

...

題目名稱：
銀髮守門人：AI 高齡者防詐騙雲端預警系統

一句話：
用 AWS + AI 幫高齡者判斷可疑電話、簡訊、LINE 訊息與轉帳要求，並在高風險時通知家人或社福單位。

核心痛點：
高齡者常遇到假檢警、假投資、假親友、假客服、假交友、假中獎等詐騙。
很多人不是不聰明，而是在緊張、孤單、被催促時，來不及判斷。

解法：
建立一個簡單的防詐助手。
高齡者只要把可疑訊息貼上，或把電話內容簡單說出來，AI 就會判斷風險等級、指出可疑話術，並用白話提醒下一步。

AWS 可用服務：
Amazon Bedrock：判斷詐騙風險與生成白話提醒
Amazon Transcribe：把可疑電話語音轉文字
Amazon Comprehend：分析關鍵詞與情緒壓力
AWS Lambda：處理判斷流程
Amazon DynamoDB：儲存案例與風險紀錄
Amazon S3：儲存語音與截圖
Amazon SNS：通知家人、社工或照護者
Amazon API Gateway：串接前端或 LINE Bot
Amazon Cognito：登入與權限管理

MVP 功能：
1. 貼上可疑訊息，AI 判斷是否可能詐騙
2. 上傳電話錄音，轉文字後分析
3. 顯示風險等級：低／中／高
4. 列出可疑關鍵句，例如「不要告訴家人」「立刻匯款」「帳戶被凍結」
5. 產生高齡者看得懂的提醒
6. 高風險時通知家人或照護者

Demo 情境：
阿姨收到 LINE：
「媽，我手機壞了，先匯 3 萬到這個帳戶，拜託不要跟爸說。」

系統分析：
風險等級：高
可疑點：
- 冒充親友
- 要求立即匯款
- 要求不要告訴家人
- 使用情緒勒索語氣

白話提醒：
「這很可能是詐騙。請先不要匯款，打原本熟悉的電話確認，或請家人陪你一起判斷。」

商業價值：
可提供給銀行、保險公司、電信業者、長照機構、地方政府、社福單位使用。
銀行可降低臨櫃詐騙匯款風險。
電信商可結合可疑簡訊提醒。
地方政府可用於銀髮族防詐教育。

你的角色定位：
我不一定要扮演純工程師，而是扮演產品企劃、風險情境設計、使用者體驗設計與 Demo 故事設計者。
我能把高齡者、家人、銀行、社福單位、政府與 AWS 技術串成一個能落地的解決方案。

黑客松 Pitch 金句：
真正的防詐，不只是辨識壞人，而是在人最脆弱、最孤單、最緊張的那一刻，給他一個可以停下來確認的理由。

英文題名：
Silver Shield AI: Cloud-Based Scam Prevention for Seniors

英文一句話：
An AWS-powered AI assistant that helps seniors detect scam messages, suspicious calls, and urgent money-transfer requests before harm happens.

...

Repository 名稱：
silver-shield-ai

專案名稱：
Silver Shield AI｜銀髮守門人

一句話：
AWS + AI 高齡者防詐騙雲端預警系統

標語：
在人最緊張、最孤單、最容易被騙的那一刻，給他一個停下來確認的理由。

...

# Silver Shield AI｜銀髮守門人

Silver Shield AI 是一個面向高齡者、家人、銀行、社福單位與地方政府的 AI 防詐騙雲端預警系統。

本專案希望透過 AWS 與 AI 技術，協助高齡者判斷可疑電話、簡訊、LINE 訊息與轉帳要求，並在高風險時提醒家人或照護者介入。

## Problem

高齡者常遇到：

- 假親友借錢
- 假檢警
- 假投資
- 假客服
- 假中獎
- 假交友
- 要求立刻匯款
- 要求不要告訴家人

很多受害者不是沒有判斷力，而是在緊張、孤單、害怕、被催促時，來不及停下來確認。

## Solution

使用者可以輸入可疑訊息或上傳可疑電話錄音，系統會：

1. 分析詐騙風險
2. 標示可疑話術
3. 產生高齡者看得懂的白話提醒
4. 高風險時通知家人、照護者或社福窗口

## AWS Architecture

預計使用：

- Amazon Bedrock：詐騙風險分析與提醒生成
- Amazon Transcribe：電話語音轉文字
- AWS Lambda：後端邏輯處理
- Amazon DynamoDB：案例與風險紀錄
- Amazon S3：儲存錄音與截圖
- Amazon SNS：高風險通知
- Amazon API Gateway：串接前端或 LINE Bot
- Amazon Cognito：登入與權限管理

## MVP Features

- 文字訊息詐騙風險判斷
- 電話錄音轉文字分析
- 低／中／高風險分級
- 可疑關鍵句標示
- 白話防詐提醒
- 高風險通知家人或照護者

## Demo Scenario

高齡者收到訊息：

> 媽，我手機壞了，先匯 3 萬到這個帳戶，拜託不要跟爸說。

系統判斷：

- 風險等級：高
- 可疑點：冒充親友、要求立即匯款、要求不要告訴家人
- 建議：請先不要匯款，改用原本熟悉的電話號碼確認。

## Target Users

- 高齡者
- 家人與照護者
- 銀行
- 電信業者
- 長照機構
- 地方政府
- 社福單位

## Hackathon Role

本專案適合 AWS、AI、資安、金融科技與社會影響力相關黑客松。

我在專案中可負責：

- 產品企劃
- 使用者情境設計
- Demo 流程設計
- Pitch Deck
- 防詐內容設計
- AI Prompt 設計
- 跨領域應用整合

## Vision

真正的防詐，不只是辨識壞人，而是在人最脆弱、最緊張、最孤單的那一刻，給他一個可以停下來確認的理由。

...

資料夾結構建議：

silver-shield-ai/
├── README.md
├── docs/
│   ├── problem.md
│   ├── solution.md
│   ├── user-scenarios.md
│   ├── aws-architecture.md
│   └── pitch-script.md
├── prompts/
│   └── scam-detection-prompt.md
├── sample-data/
│   ├── fake-family-message.txt
│   ├── fake-bank-message.txt
│   └── fake-investment-message.txt
├── frontend/
├── backend/
└── LICENSE

...
