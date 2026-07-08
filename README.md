# Welcome to OpenCrawling 🌐

**High-Performance Enterprise Data Ingestion, Federation & Security Framework for AI and Search.**

OpenCrawling is an open-source, cloud-native framework designed to solve the hardest problem in enterprise AI and search: **securely connecting siloed content repositories to modern ingestion pipelines.** 

Going far beyond simple web scraping, OpenCrawling acts as an intelligent bridge between legacy/enterprise content stores (ECM, CRM, relational databases, cloud buckets) and modern search engines, vector databases, and Large Language Model (LLM) pipelines.

---

## 💡 Why OpenCrawling?

When building Retrieval-Augmented Generation (RAG) systems or enterprise search, getting the data is only half the battle. You also need to respect document permissions, handle incremental updates, and scale without bottlenecking source systems. 

OpenCrawling is built from the ground up to address these challenges with modern software architecture:

*   🔒 **Enterprise Security First (ACL Mapping):** Built-in synchronization of native Access Control Lists (ACLs). We ensure that your AI search engines and RAG pipelines only return documents the querying user is explicitly authorized to see.
*   ⚡ **High-Performance & Non-Blocking:** Powered by **Java 25** and **Spring Boot 4**, leveraging Virtual Threads and structured concurrency for massive I/O throughput with minimal resource footprint.
*   🤖 **AI & RAG Ready:** Native support for on-the-fly document transformation, text extraction, semantic chunking, and embedding generation before payloads hit vector stores.
*   🔌 **Pluggable SPI Architecture:** Clean, modular interfaces that make it trivial for developers to build and plug in custom connectors without altering the core orchestration engine.

---

## 🏗️ Architecture & Core Modules

Our ecosystem is organized into clean, decoupled modules:

| Module | Description |
| :--- | :--- |
| **`opencrawling-core`** | The runtime engine managing Virtual Thread task execution, rate-limiting, scheduling, and state persistence. |
| **`opencrawling-connector-api`** | Lightweight Java SPIs defining `RepositoryConnector`, `TransformationConnector`, and `OutputConnector` interfaces. |
| **`opencrawling-connectors`** | Out-of-the-box adapters for web crawling, enterprise content management systems, and vector/search databases. |
| **`opencrawling-security`** | The authority and token-mapping layer that translates repository permissions into search-engine security filters. |

---

## 🛠️ Technology Stack

*   **Core:** Java 25 (LTS), Spring Boot 4.x
*   **Concurrency:** Virtual Threads & Structured Concurrency
*   **Build & Deployment:** Maven / Gradle Multi-Module, Docker, Kubernetes ready
*   **License:** Apache License 2.0

---

## 🤝 Get Involved

We are building a community of developers, architects, and data engineers passionate about open-source enterprise data integration and AI infrastructure. 

*   📖 **Read the Documentation:** [Link to Docs/Website]
*   🐛 **Report Issues:** Check individual repository issue trackers.
*   💬 **Join the Discussion:** [Link to Discord / GitHub Discussions]
*   ⭐ **Star our Repositories:** If you find our work useful, give us a star!

*Built with passion for the Open Source and AI community.*
