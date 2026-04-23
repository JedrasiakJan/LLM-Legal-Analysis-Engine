# ⚖️ Legal Domain AI Agent (Advanced RAG Architecture)

> ⚠️ **Note:** The core logic and Python source code are currently kept in a private, closed-source repository due to upcoming commercialization. This repository serves as an architectural overview and technical showcase of my AI-native engineering capabilities.

An end-to-end, agentic Retrieval-Augmented Generation (RAG) system built for the Polish legal domain. It autonomously processes scraped legal documents (Supreme and Administrative Courts) to provide precise, context-aware answers while strictly mitigating LLM hallucinations through self-reflection.

### 🛠️ Tech Stack & Infrastructure


Frontend & UI

<p align="left">
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white" alt="Streamlit" />
<img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
<img src="https://img.shields.io/badge/Markdown_Parsing-000000?style=for-the-badge&logo=markdown&logoColor=white" alt="Markdown" />
<img src="https://img.shields.io/badge/YAML_Config-CB171E?style=for-the-badge&logo=yaml&logoColor=white" alt="YAML" />
</p>

Data Engineering & Intelligent Chunking

<p align="left">
<img src="https://img.shields.io/badge/Docling-0066FF?style=for-the-badge&logo=ibm&logoColor=white" alt="Docling" />
<img src="https://img.shields.io/badge/LangChain_Splitters-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white" alt="LangChain Splitters" />
<img src="https://img.shields.io/badge/PyMuPDF-FF6600?style=for-the-badge&logo=adobeacrobatreader&logoColor=white" alt="PyMuPDF" />
<img src="https://img.shields.io/badge/Microsoft_Word-2B579A?style=for-the-badge&logo=microsoftword&logoColor=white" alt="Docx" />
<img src="https://img.shields.io/badge/Progress_Tracking-FF6F00?style=for-the-badge&logo=tqdm&logoColor=white" alt="TQDM" />
</p>

RAG Architecture & AI Models
<p align="left">
<img src="https://img.shields.io/badge/Qdrant-0033FF?style=for-the-badge&logo=qdrant&logoColor=white" />
<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" />
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" />
<img src="https://img.shields.io/badge/CUDA_Optimization-76B900?style=for-the-badge&logo=nvidia&logoColor=white" />
<img src="https://img.shields.io/badge/Qwen_/_Mistral-525CB0?style=for-the-badge&logo=alibabacloud&logoColor=white" />
</p>

<p align="left">
<img src="https://img.shields.io/badge/Agentic_RAG_Architecture-2196F3?style=for-the-badge&logo=ai&logoColor=white" />
<img src="https://img.shields.io/badge/BGE_Reranker_Precision-4CAF50?style=for-the-badge&logo=google-cloud&logoColor=white" />
<img src="https://img.shields.io/badge/Hybrid_Search_BM25_%2B_Dense-FFA500?style=for-the-badge&logo=elasticstack&logoColor=white" />
<img src="https://img.shields.io/badge/Self--Reflection_LLM_Judge-8A2BE2?style=for-the-badge&logo=openai&logoColor=white" />
</p>

Security & On-Premise Deployment

<p align="left">
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker" />
<img src="https://img.shields.io/badge/Bcrypt-4A154B?style=for-the-badge&logo=springsecurity&logoColor=white" alt="Bcrypt" />
<img src="https://img.shields.io/badge/Hashlib-000000?style=for-the-badge&logo=python&logoColor=white" alt="Integrity" />
<img src="https://img.shields.io/badge/DotEnv-ECD53F?style=for-the-badge&logo=dotenv&logoColor=black" alt="Dotenv" />
</p>
---

## 📸 Product Modules & Interface Showcase

Built as a secure, AI-native B2B platform for legal professionals, the system integrates multiple specialized tools into one cohesive workspace. The interface is designed to support high-stakes legal workflows by combining structured analysis, document review, and transparent access to retrieved legal sources.

### 1. Main Dashboard & Secure Login
The platform opens with a secure authentication layer using custom password hashing to safeguard confidential legal activity. Once authenticated, users access a centralized dashboard that provides entry to the system’s full set of legal AI modules.
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/auth_secure_login.png" alt="Ekran bezpiecznego logowania" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/dashboard_main_view.png" alt="Główny dashboard po zalogowaniu" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/backend_auth_logs.png" alt="Logi uwierzytelniania na serwerze" width="1000" />

### 2. Module: Legal Analysis (AI Legal Partner)
The flagship feature of the platform, designed to assist lawyers with complex case research. Users submit detailed legal scenarios, and the Agentic Workflow breaks them down to retrieve relevant case law and statutes. To ensure absolute precision, the system features a manual override—allowing experts to directly inject specific articles or legal acts into the context window if the automated retrieval requires refinement. Crucially, the entire analysis runs locally, ensuring that sensitive client data never leaves the secure environment. The result is a structured, highly accurate legal opinion strictly grounded in verified jurisprudence.

<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/step1_user_prompt.png" alt="Krok 1: Wprowadzenie problemu prawnego" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/step2_context_retrieval.png" alt="Krok 2: Wyszukiwanie odpowiednich przepisów" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/step3_final_opinion1.png" alt="Krok 3: Analiza problemu przez AI" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/step3_final_opinion2.png" alt="Krok 4: Końcowa opinia prawna" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/backend_rag_analysis_trace.png" alt="Ślad wykonania RAG na backendzie" width="1000" />

### 3. Module: Contract Review (Analizator Umów)
A specialized document analysis engine built for automated contract review. Instead of relying on static rules, the system utilizes predefined analytical templates (e.g., for B2B, real estate, or civil contracts) to autonomously retrieve the most relevant legal acts and jurisprudence from the local Qdrant vector database. The LLM then reviews the uploaded agreement against this dynamically gathered legal context, securely identifying risks and non-compliance entirely on-premise.

<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/contract_sidebar_upload.png" alt="Pasek boczny wgrywania umów" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/contract_retrieval_cart.png" alt="Koszyk pobranych artykułów prawnych" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/contract_final_analysis.png" alt="Gotowa analiza ryzyka dla umowy" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/backend_contract_review_logs.png" alt="Logi silnika weryfikacji umów na backendzie" width="1000" />

### 4. Module: Knowledge Base Search (Baza Wiedzy)
A high-performance search engine granting users direct, transparent access to the local Qdrant database of legal acts and court judgments. Engineered with advanced metadata filtering (payload search), this module allows legal professionals to execute highly precise queries by filtering for specific case signatures, document types, or exact article numbers. This capability provides a reliable tool for manual database auditing and independent verification of the exact legal sources retrieved by the system.
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/knowledge_base_search_interface1.png" alt="Knowledge Base search interface" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/knowledge_base_search_interface2.png" alt="Knowledge Base search results" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/knowledge_base_article_view.png" alt="Knowledge Base article view" width="1000" />

### 5. Module: Legal Utility Suite (Narzędzia Pomocnicze)
Beyond probabilistic AI features, the platform integrates a suite of deterministic, hard-coded utilities designed to automate daily operational tasks for legal professionals without the risk of LLM mathematical hallucinations.
* **Statutory Deadline Calculator (Kalkulator Terminów KPA/KPC):** Automates procedural deadline tracking by factoring in Polish civil procedure rules (Art. 115 KC), accurately rolling over weekends and national holidays.
* **Delay Interest Calculator (Kalkulator Odsetek):** Computes statutory interest for late payments using current NBP (National Bank of Poland) reference rates, instantly generating ready-to-copy claim clauses for lawsuit drafting.
* **Automated PDF Generator (Generator Pism):** A streamlined engine that compiles user inputs into a properly formatted, print-ready Pre-Litigation Demand for Payment (.pdf) with full support for Polish typography.

<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/calculator_deadlines.png" alt="Kalkulator terminów KPA/KPC" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/calculator_interest.png" alt="Kalkulator odsetek za opóźnienie" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/Generator_demand_form.png" alt="Generator wezwania - formularz" width="1000" />
<br>
<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/Generator_demand_pdf_output.png" alt="Generator wezwania - podgląd PDF" width="1000" />
---

## 🚀 The "Builder" Approach: Agentic Workflow in Action

Unlike standard RAG wrappers, this system is driven by a custom-built, multi-stage agentic pipeline tailored for the rigorous demands of the legal domain. Below is an actual backend execution trace demonstrating the system's autonomous reasoning in real-time. The agent dynamically decomposes a complex legal scenario, extracts critical "VIP" context, applies GPU-accelerated cross-encoder reranking (running locally on CUDA), and routes the final output through a strict LLM-as-a-Judge ("Sędzia") module for self-reflection and hallucination prevention.

<img src="https://raw.githubusercontent.com/JedrasiakJan/LLM-Legal-Analysis-Engine/main/assets/backend_agentic_workflow_trace.png" alt="Ślad działania potoku agentowego" width="1000" />

*Backend execution trace: Multi-Query Decomposition ➔ VIP Context Extraction ➔ Local GPU Reranking (BAAI) ➔ LLM Judge Audit.*
---

## 🧠 AI-Native Architecture Breakdown

To maximize factual accuracy and prevent hallucinations in high-stakes legal environments, the pipeline is divided into several autonomous, self-correcting steps:

1. **Multi-Query Decomposition:** The primary agent analyzes the natural language prompt and breaks it down into structured JSON sub-queries (e.g., separating questions about board member liability from VAT statute of limitations) for parallel retrieval.
2. **Metadata Extraction & Hybrid Search:** The system intelligently extracts critical legal entities (e.g., exact article numbers like KSH Art. 299) to apply strict payload filters. It then searches the locally hosted **Qdrant** database utilizing a hybrid approach (BM25 + semantic vector embeddings).
3. **Cross-Encoder Reranking:** A local `BAAI/bge-reranker-v2-m3` model, accelerated via CUDA, re-evaluates and scores the retrieved chunks. It aggressively filters out irrelevant noise, passing only the absolute top-scoring, highly dense context to the generator.
4. **Self-Reflection (LLM-as-a-Judge):** Before presenting the final output to the user, a secondary evaluation agent ("Sędzia") audits the generated legal opinion against the raw retrieved statutes. If it detects any inconsistencies or missing citations, it autonomously triggers corrections.

---

## 🛠️ Tech Stack & Infrastructure

* **Core AI & LLMs:** Python, Qwen 32B (Locally hosted & aggressively optimized for context limits), LLM-as-a-Judge agentic methodology.
* **Search & Retrieval Engine:** Qdrant Vector Database (Hybrid Search: BM25 + Vectors), BAAI Cross-Encoders (`bge-reranker-v2-m3`).
* **Infrastructure & Hardware:** Dockerized ecosystem running on a custom RTX 5090 Local Server, engineered specifically to manage strict VRAM constraints and maximize throughput.
* **Frontend & Security:** Streamlit UI protected by custom cryptographic password hashing for secure session management.
* **Development Paradigm:** Built with an AI-first mindset, leveraging advanced AI-assisted coding workflows (Cursor / Claude) for rapid architecture scaling.

---
*Developed by Jan Jędrasiak as an independent AI engineering showcase and advanced R&D portfolio project.*
