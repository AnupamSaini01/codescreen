🧠 GenAI RAG Project — Progress Summary
📌 Goal

Build a GenAI-powered Document Search system using RAG (Retrieval Augmented Generation) that:

Ingests enterprise documents
Performs semantic + keyword hybrid search
Generates grounded answers using LLMs
Provides citations and explainability
🏗️ Architecture Designed
🔄 End-to-End Flow
Document ingestion
Layout-aware semantic chunking
Embedding generation (Azure OpenAI - ADA)
Hybrid indexing (Vector + Keyword)
Milvus (Vector DB)
Elasticsearch (Keyword search)
User query processing
Hybrid retrieval
Semantic reranking
LLM answer generation
Response with citations + confidence score
⚙️ Tech Stack Finalized
Backend
Java 17
Spring Boot
Spring MVC
Maven
AI / RAG
Azure OpenAI (GPT + ADA embeddings)
Semantic ranking (Azure AI Search)
Search & Storage
Milvus (Vector DB)
Elasticsearch (Keyword search)
SQL / PostgreSQL (metadata)
Infrastructure
Azure Blob Storage
Azure Service Bus
Docker (install in progress)
Frontend (future)
React / Angular
📁 Spring Boot Project Structure Designed
com.company.rag
 ├── controller
 ├── service
 ├── pipeline
 │    ├── ingestion
 │    ├── chunking
 │    ├── embedding
 │    ├── indexing
 │    ├── retrieval
 │    ├── reranking
 │    ├── generation
 │    └── citation
 ├── client
 ├── model
 ├── dto
 ├── config
 ├── exception
 ├── util
🧱 Initial Coding Work Done
1. Project Setup
Downloaded from Spring Initializr
Package: com.company.rag
Packaging: JAR
Config: Properties
2. IDE Setup Issue Resolved
Fixed JDK not defined issue (Java 17 required)
Explained IntelliJ configuration steps:
Project Structure → SDK setup
Maven reload
3. Running Issue Debugging
Identified "file not runnable" issue
Explained Spring Boot entry point (RagApplication.java)
Maven sync + JDK setup required
🚀 Next Planned Coding Steps (After Docker restart)
STEP 1 (Next coding task)

👉 Document Upload API

REST endpoint
File ingestion service
First pipeline entry point
STEP 2

👉 Apache Tika integration (text extraction)

STEP 3

👉 Chunking engine (layout-aware)

STEP 4

👉 Embedding + vector storage (Milvus)

🐳 Docker Status
Docker installation in progress
Required for:
Milvus
Elasticsearch
local infrastructure testing
📌 Current Status

✔ Project downloaded
✔ Architecture designed
✔ IDE setup started
✔ JDK issue resolved
✔ Docker installation pending restart
⏳ Ready to begin coding after reboot

🚀 After your restart

When you're back, just say:

👉 “ready to continue”

and we will immediately:

fix any remaining setup issues
run the Spring Boot project
start coding the first real GenAI ingestion API
