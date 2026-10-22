# Aether AI — Software Requirements Engineering Platform

An enterprise AI-powered Software Requirements Engineering platform adhering strictly to **ISO/IEC/IEEE 29148:2018** and **IEEE 830-1998** standards.

## 🚀 Key Capabilities

1. **9-Stage Controlled AI Requirements Elicitation**:
   - Structured sequential lifecycle with strict stage-gating and Context Guard.
   - Multilingual support (English, Hindi, Hinglish).
   - Real-time atomic requirement extraction (`FR-XXX`, `NFR-XXX`, `CON-XXX`, `ASM-XXX`, `INT-XXX`, `STK-XXX`).
2. **Quality & Ambiguity Audit**:
   - Heuristic non-verifiable words detection and semantic conflict analysis.
   - Vector-based Cosine Similarity deduplication (`Xenova/multilingual-e5-small`).
3. **ISO/IEC/IEEE 29148 Verification**:
   - Completeness, consistency, singularity, and testability scoring.
4. **Exact-Template SRS Generation & Export**:
   - IEEE Sections 1–6 and Appendices A, B, and C with PDF/DOCX generation.
5. **Traceability & Continuous Change Control**:
   - 5-Tier bidirectional traceability matrix.
   - Semantic diff viewer for continuous versioning (v1.0 → v1.1).

## 📚 Research Papers & Academic Foundation

The architectural design of Aether AI is research-informed by three peer-reviewed literature publications:
1. **Paper 1**: *"Using LLMs in Software Requirements Specifications: An Empirical Evaluation"* — Zero-hallucination prompting, human-in-the-loop validation, and context tuning.
2. **Paper 2**: *"REQINONE: A Large Language Model-Based Agent for Software Requirements Specification Generation"* — Multi-agent elicitation, FR vs NFR 7-tier categorization, and trace-to-source evidence linking.
3. **Paper 3**: *"A Framework for Structurally Deterministic Pipeline Based Drafting and Quality Improvement of SRS Using Language Models and Reinforcement Learning"* — Sentence embeddings, K-Means semantic topic clustering, deterministic section mapping, and incremental SRS updating.

📄 **Comprehensive Technical Documentation & PDF:**
- 📘 [PROJECT_RESEARCH_ALGORITHMS_AND_ARCHITECTURE.md](file:///c:/shubham%20dalvi%20project/Major_project_2026/PROJECT_RESEARCH_ALGORITHMS_AND_ARCHITECTURE.md) (Full Technical Specification)
- 📑 [Aether_AI_Research_and_Algorithm_Architecture.pdf](file:///c:/shubham%20dalvi%20project/Major_project_2026/Aether_AI_Research_and_Algorithm_Architecture.pdf) (Generated Technical Report PDF)

## 🛠️ Tech Stack
- **Frontend**: Next.js (App Router), Vanilla CSS, Tailwind CSS, Lucide Icons
- **Backend**: Express.js, MongoDB (Mongoose), In-Memory DB Fallback, Ollama AI Provider (CodeLlama / Gemma)
- **Neural Embeddings**: `Xenova/multilingual-e5-small` (384-dimensional dense vectors in ONNX Runtime)
- **Document Export**: PDFKit (`pdfkit`), Docx (`docx`)

## 🏁 Quick Start

### 1. Backend Setup
```bash
cd backend
npm install
npm run dev
```

### 2. Frontend Setup
```bash
cd frontend
npm install
npm run dev
```

### 3. Generate Research Architecture PDF
```bash
node backend/scripts/generateReportPdf.js
```

