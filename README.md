# Agentic AI Insurance Claim Automation & Policy Retrieval Assistant
An intelligent, multi-agent automated system designed to streamline complex insurance policy inquiries and claim processing workflows using localized workflow automation (**n8n**), **Agentic AI architecture**, and cloud-ready vector datasets.

---

## System Architecture & Multi-Agent Design
The system implements a **Multi-Agent Collaborative Architecture** to handle heterogeneous and multi-step insurance workflows:

1. **Multi-Agent Orchestrator (多代理協作中樞 Agent):** 
   * Acts as the central decision-making hub. Handles user authentication (ID + Birthday verification) and dynamically routes intents.
2. **Data Query Agent (資料查詢 Agent):** 
   * Handles general Q&A regarding insurance terms, and executes personalized queries against user policies and vector databases.
3. **Claim Application Agent (申請理賠 Agent):** 
   * Guides users through claim procedures, parses uploaded documents, and performs preliminary eligibility checks and payout estimations.

## Tech Stack
* **Workflow Automation & Orchestration:** n8n (Local Environment)[cite: 1]
* **AI & LLM Framework:** Ollama Chat Models, Custom Prompt Engineering, Structured Output Parsers[cite: 1]
* **Vector Search & Data:** Python, Pandas, GitHub Releases (Vector Datasets)[cite: 1]
* **Domain:** InsurTech, Agentic AI, Retrieval-Augmented Generation (RAG)[cite: 1]

## n8n Workflow Templates
To ensure transparency and reproducibility, the core n8n low-code workflow templates are provided in this repository:
* `workflows/insurance_main_workflow.json`: The multi-agent orchestration and routing logic.
* You can easily import these JSON files into your local n8n instance to review or replicate the automation pipeline.

## Dataset & Releases (Vector Embeddings)
This project provides a dedicated RAG dataset for the insurance domain (using Cathay Life Insurance policies as an example), containing pre-processed chunks and their corresponding embeddings.

Dataset Download
Due to the large data volume and to ensure version stability, the files are hosted in GitHub Releases:
insurance_rag_data.csv (Full Version) - link：https://github.com/111306047/insurance/releases/download/v1.0.0/insurance_rag_data.csv
