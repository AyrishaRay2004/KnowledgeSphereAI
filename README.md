# KnowledgeSphereAI

> 🚧 **Work in Progress**
>
> KnowledgeSphereAI is an offline, multimodal Retrieval-Augmented Generation (RAG) assistant currently under active development. The project is being built incrementally, and new features will be added over time.

---

# Overview

KnowledgeSphereAI is a personal project focused on building a secure, fully local AI assistant capable of understanding and answering questions from multiple types of documents without relying on cloud services.

The goal is to create a modular RAG system that combines document retrieval, OCR, multilingual understanding, and multimodal processing into a single offline application — architected so that no document, query, or answer ever needs to leave the machine it runs on.

This repository is a personal, independently rebuilt version of a system I originally designed and built during my summer internship. The original deployment and its proprietary configuration belong to the organization and are not published here. What you'll find in this repo is my own from-scratch recreation of the architecture and features — re-pointed at open-source, locally-run tooling (Ollama, open embedding models) instead of any internal infrastructure — built to demonstrate and continue developing the ideas on my own time.

---

# Planned Features

### Document Intelligence

* PDF question answering
* Microsoft Word, PowerPoint, and Excel support
* Text file ingestion
* Scanned document processing

### Retrieval

* FAISS vector database
* BM25 keyword search
* Hybrid retrieval with reciprocal-rank fusion
* Cross-encoder reranking
* Query rewriting and adaptive retrieval

### OCR

* PaddleOCR
* EasyOCR fallback
* TrOCR
* Image preprocessing (denoise, deskew, contrast, super-resolution)

### Multimodal AI

* Image understanding (CLIP-based image embeddings)
* Audio transcription
* Video document processing

### Multilingual Support

* Automatic language detection
* Multilingual embeddings
* Cross-language semantic search

### Security

* Local-only execution
* Role-based access control enforced at the retrieval layer, not just the UI
* Encryption for uploaded files
* Malware scanning
* Personally Identifiable Information (PII) masking via NER

### Human-in-the-Loop & Evaluation

* Reviewer queue for correcting and approving AI-generated answers
* Feedback loop into future responses
* Evaluation dashboard with RAGAS-style automated answer-quality scoring
* Per-query latency and performance metrics

### Knowledge Graph

* Relation extraction and graph-backed storage (optional, Neo4j)

### User Experience

* Streamlit-based interface
* Chat history
* Session management
* Report export (DOCX, PDF, XLSX)

---

# Technology Stack

| Component     | Technologies                                   |
| ------------- | ----------------------------------------------- |
| Language      | Python                                           |
| UI            | Streamlit                                        |
| LLM           | Ollama                                           |
| Vector Search | FAISS                                            |
| Retrieval     | BM25, reciprocal-rank fusion, cross-encoder rerank |
| Embeddings    | Sentence Transformers, multilingual-e5, CLIP     |
| OCR           | PaddleOCR, EasyOCR, TrOCR                        |
| Speech        | Faster-Whisper, Piper                            |
| Knowledge Graph | Neo4j                                          |
| Database      | SQLite                                           |
| Security      | spaCy, ClamAV, cryptography (Fernet)             |

---

# Current Status

This project is under active development.

The public repository will evolve gradually as features are completed, tested, and documented.

Upcoming additions include:

* Hybrid retrieval pipeline
* OCR improvements
* Image understanding
* Audio support
* Evaluation dashboard
* Report generation
* Knowledge graph integration
* Performance optimizations

---

# My Role

Designing and building the platform end-to-end as an independent project, including the RAG pipeline, OCR and multimodal document ingestion, security features (RBAC, PII masking, and malware scanning), human-in-the-loop review workflow, evaluation dashboard, and report/export capabilities.

---

# Roadmap

* [ ] Local chat interface
* [ ] PDF question answering
* [ ] Hybrid retrieval
* [ ] OCR pipeline
* [ ] Multilingual support
* [ ] Image understanding
* [ ] Audio transcription
* [ ] Report generation
* [ ] Evaluation dashboard
* [ ] Knowledge graph support

---

# License

This project is released under the MIT License.

---

📫 Feel free to reach out if you'd like to know more about the project or discuss the architecture.

