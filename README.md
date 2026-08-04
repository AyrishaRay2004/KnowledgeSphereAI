# KnowledgeSphereAI

> 🚧 **Work in Progress**
>
> KnowledgeSphereAI is an offline, multimodal Retrieval-Augmented Generation (RAG) assistant currently under active development. The project is being built incrementally, and new features will be added over time.

---

# Overview

KnowledgeSphereAI is a personal project focused on building a secure, fully local AI assistant capable of understanding and answering questions from multiple types of documents without relying on cloud services.

The goal is to create a modular RAG system that combines document retrieval, OCR, multilingual understanding, and multimodal processing into a single offline application — architected so that no document, query, or answer ever needs to leave the machine it runs on.

This repository is an independent implementation built for learning, experimentation, and continuous development using open-source technologies.

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

# Motivation

The objective of this project is to explore modern Retrieval-Augmented Generation (RAG) techniques, document intelligence, multimodal AI, and secure local deployment using open-source technologies.

It also serves as a personal portfolio project to experiment with scalable AI system design and continuously improve practical machine learning and software engineering skills.

---

# My Role

Designing and building the platform end-to-end, solo: RAG pipeline, OCR/multimodal ingestion, security layer (RBAC, PII masking, malware scanning), human-in-the-loop review workflow, evaluation dashboard, and report/export tooling.

---

# Repository Structure

```text
KnowledgeSphereAI/
│
├── app/
├── ingestion/
├── retrieval/
├── embeddings/
├── ocr/
├── multimodal/
├── security/
├── exports/
├── evaluation/
├── data/
├── models/
├── docs/
└── README.md
```

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

# Acknowledgements

This project is inspired by concepts explored while working on document intelligence and Retrieval-Augmented Generation systems during my internship. This repository is an independent implementation developed using publicly available tools and open-source technologies. It does not contain any proprietary code, datasets, configurations, or organization-specific assets.

---

📫 Feel free to reach out if you'd like to know more about the project or discuss the architecture.

