# 生成式 AI 應用系統與工程

**Generative AI Application Systems and Engineering**

## 基本資訊

| 項目 | 內容 |
|------|------|
| 開課系所 | 資訊工程研究所 |
| 開課學年／學期 | 114 學年度 第 2 學期 |
| 學分數 | 3 |
| 授課教師 | 莊坤達 |
| E-mail | ktchuang@mail.ncku.edu.tw |

## 課程概述

本課程以「生成式 AI 應用系統」開發為核心，帶領學生從需求分析、系統設計，到實作與部署，完成一個生成式 AI Web 服務。內容涵蓋軟體工程 SDLC、前後端技術、資料流程與工作流、開源 CI/CD 與 MLOps/LLMOps 工具、AWS 雲端環境、分散式 AI Infra、LLM 微調與 local LLM 評測、Agent 工作流與 MCP/ADK/agent-to-agent 架構、LiteLLM/OpenRouter 等模型代理工具，以及 token 經濟學、Prompt 優化、多輪對話設計、幻覺減少與 LLM 資安議題。學生將透過至少六次程式作業與期末專題，實作一個具完整工程思維的生成式 AI 應用系統。

## 教學目標

修課學生預期能達成：

1. 理解生成式 AI 應用系統的整體架構，包括前端、後端、LLM 層、Agent 工作流與資料流。
2. 熟悉 SDLC 在生成式 AI 專案中的實務流程，能撰寫系統需求與高階架構設計。
3. 能運用 Web 架構、AWS 平台、資料庫與向量檢索技術，可建構具 RAG 能力的應用系統。
4. 了解並整合 MLOps/LLMOps toolchain，包括 CI/CD、模型部署、評估與觀測。
5. 掌握 Agent workflow、MCP、ADK 與 agent-to-agent 等概念，並透過 callbacks 實作安全與審計邏輯。
6. 理解 token 經濟學、多輪對話設計與幻覺減少策略，並融入系統設計中。
7. 能設計與實作基本的 LLM 資安防護，包括 prompt injection 防禦與 response auditing。
8. 完成一項可展示的生成式 AI 應用系統期末專題。

## 課程進度表

| 週次 | 主題 | 時數 | 內容 |
|:----:|------|:----:|------|
| 1 | 課程介紹、修課要求與評分方式 | 3h | 生成式 AI 應用系統典型架構：前端、後端、LLM 層、Agent workflow、資料流、系統觀測機制等介紹 |
| 2 | SDLC、需求分析與系統架構設計概念 | 3h | 生成式 AI 專案的 SDLC 設計、撰寫 System Requirement / Use Case、Microservice 高階架構圖規劃、服務邊界與模組切分 |
| 3 | 前端 Web 技術與生成式介面設計 | 3h | Next.js / React / Tailwind、gen-AI UI patterns、SSE / WebSocket streaming |
| 4 | 後端架構、微服務設計與 LLM Proxy Gateway | 3h | API Server（FastAPI / Node.js）、REST / WebSocket / SSE 實作、Microservice 架構核心、GenAI 微服務拆分、LLM Gateway 核心微服務（Routing、Token Logging） |
| 5–6 | 事件驅動資料流架構 | 6h | ETL / background tasks、Airflow DAG / Task / Scheduler、Kafka → Airflow → Iceberg 典型資料處理流程、Iceberg Data Lake、Microservice 與 Background Worker 整合 |
| 7 | CI/CD、MLOps、LLMOps | 3h | GitHub Actions / GitLab CI、Docker 化與環境建置、MLflow / promptfoo、模型行為監控與 Regression Test、Microservice deployment pipeline |
| 8 | AWS 開發與部署、AWS Kiro 介紹 | 3h | AWS EC2 / ECS / Lambda、IAM / S3 / RDS、Kiro 環境、成本估算與 auto scaling、CDN / Cache |
| 9 | 資料庫系統與向量資料庫 | 3h | Embedding / HNSW / Retrieval、RAG pipeline（chunking → index → rerank）、Retrieval microservice |
| 10 | 模型微調、Local LLM、行為檢測 | 3h | Fine-tuning、vLLM / Ollama 本地部署、promptfoo / eval harness 模型行為檢測、Model Service as Microservice |
| 11–12 | 分散式 AI Infra 與工作流程 | 6h | Ray tasks / actors、Ray Serve + scaling、多檔案多任務平行 LLM pipeline、Ray Worker microservice |
| 13 | Agent Workflow、MCP、ADK、Agent-to-Agent 協作 | 3h | Agent 架構（Planner / Tool / Critic）、MCP 工具抽象層與資源管理、ADK / Vertex AI Agent Builder、agent-to-agent workflow |
| 14 | ADK Callbacks 與 Sanitize / Policy Check / Audit Middleware | 3h | ADK Agent 生命周期與 callback 流程、使用 ADK callbacks 做安全防護與審計 |
| 15 | LLM Security、Jailbreak 與 Response Auditing | 3h | Prompt Injection、Jailbreak 防禦、ADK-based Policy Engine、API key 保護與最小權限原則 |
| 16 | Observability | 3h | LLM UX / error recovery、延遲優化 / Queue、logs / metrics / distributed tracing、token 成本與效能指標、Online A/B testing |
| 17–18 | Project Demo | 6h | 期末專題展示 |

## 評量方式

| 項目 | 比重 |
|------|:----:|
| HW 1 | 10% |
| HW 2 | 10% |
| HW 3 | 10% |
| HW 4 | 10% |
| HW 5 | 10% |
| HW 6 | 10% |
| **Final Project** | **40%** |

### Final Project 評分面向

- 系統架構圖（含微服務拆分、Agent workflow）
- 服務流程圖與 API 設計
- Demo Presentation and Slides
- GitHub Source and Technical Report

## 課程要求

- 具備基本程式設計能力
- 具備基本 Web 技術（HTML / CSS / JS）與 GitHub 使用經驗
- 對雲端服務有初步認識者佳（非必要條件）

## 參考資料

- 講義、程式碼示例、AWS 教材
- MCP、LLMOps、Ray 等官方文件