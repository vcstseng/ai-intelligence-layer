# AI Intelligence Layer — Bilingual Edition

可直接在瀏覽器開啟的決策支援產品殼層。包含電商、餐飲、專案管理三個領域，以及每個領域四個可探索的管理案例。

## 使用方式

直接以現代瀏覽器開啟 `index.html`。不需要後端、資料庫、API key 或外部服務。右上角可即時切換台灣繁體中文與英文；目前所在頁面、案例、選項與人員設定參數會保留。

## 範圍

- 共用 Golden Path：總覽 → 洞察 → 證據 → 決策 → 行動 → 回顧
- 12 個 deterministic mock-data 案例
- 每個案例具有 Attention signal、指標、洞察、支持／保留條件證據、可重現計算、來源資料與選項
- 三個 Primary Golden Cases 另具人類決策、行動護欄、結果回顧、組織學習與相關決策記憶

## 資料與責任界線

所有顯示的資料為本機固定 mock data。每一張 Evidence 卡片均可展開「查看計算」及「查看來源資料」。AI 的角色是綜合證據與脈絡；程式負責 deterministic calculation；人類負責決策。歷史先例與結果判讀均不應被視為因果證明。

## Controlled Extension — Product Architecture & Growth Technical Proof

本版在既有產品殼層中新增「產品架構」頁，使用非技術語言說明五項相連能力：商業脈絡與資料、分析與智慧、AI 工具與知識、決策與執行、回顧與學習。Security、Governance、Observability、Evaluation 被標示為跨層設計考量，並未假裝已完成企業級實作。

電商的 **Growth Without Profit** 案例在 Insight 與 Evidence 頁提供「這個 AI 洞察如何運作」modal。它將既有 $50 → $65 的人員決策，連結至可檢視的 fixture、interpret contract 與 grounding rules：

- `examples/ecommerce/growth-without-profit/growth_fixture.json`
- `core/interpret/growth_contract.json`
- `core/ground/growth_validation_rules.md`
- `docs/growth-technical-proof.md`

### Demonstration status

- **Implemented:** static source records, deterministic calculations, evidence traceability, the human parameter and guardrail interactions.
- **Simulated:** AI structured interpretation, context selection, and option generation.
- **Planned:** live tool calling, retrieval, LLM structured output, and production-grade evaluation/observability.

本 prototype 沒有後端、API key、LLM、RAG pipeline 或外部資料呼叫；可直接以靜態網站方式開啟 `index.html`。
