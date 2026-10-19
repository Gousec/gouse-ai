# RAG Document Assistant

A portfolio project exploring **Retrieval-Augmented Generation (RAG)**: retrieving relevant passages from documents and using them to help answer questions with traceable sources.

**Status:** 🚧 In development. The roadmap below describes intended features; they should be marked complete only after implementation and testing.

## 🎯 Goals

- Ingest documents and split them into searchable chunks
- Retrieve relevant context for a user question
- Generate answers grounded in retrieved passages
- Show source references so users can verify answers
- Evaluate retrieval and answer quality with a repeatable test set

## 🧱 Planned Architecture

1. **Document ingestion** — load and normalize supported documents
2. **Chunking** — split text into configurable overlapping chunks
3. **Indexing** — create embeddings and store searchable chunks
4. **Retrieval** — find context relevant to each question
5. **Answer generation** — respond using retrieved context
6. **Evaluation** — measure retrieval quality, answer faithfulness, latency, and cost

## 🛠️ Proposed Stack

- **Language:** Python
- **API:** FastAPI
- **Retrieval:** embedding-based semantic search; hybrid retrieval may be added
- **Testing:** pytest
- **Packaging:** Docker

The implementation will choose specific libraries and models based on reproducibility, resource requirements, and evaluation results.

## 🚀 Getting Started

Implementation is not yet ready for a runnable installation. Setup instructions, dependencies, example documents, and runnable commands will be added as the first version is completed.

## 📏 Evaluation Plan

The project will use a small, documented question-and-answer test set to assess:

- **Retrieval:** Recall@K and/or MRR
- **Answer quality:** correctness, faithfulness to retrieved context, and citation support
- **System performance:** response latency and estimated cost where applicable

No performance numbers are published yet; measurements will be added after experiments are run.

## 🗺️ Roadmap

- [ ] Add document loading and chunking
- [ ] Implement semantic retrieval
- [ ] Generate grounded answers with source references
- [ ] Add a repeatable evaluation set and metrics
- [ ] Expose the pipeline through an API
- [ ] Add automated tests and Docker support
- [ ] Document measured results and known limitations

## 👋 About

I'm Gouse, an AI/ML practitioner interested in NLP, LLM applications, deep learning, and scalable data processing.

- GitHub profile: [@Gousec](https://github.com/Gousec)
- More projects: [Browse my repositories](https://github.com/Gousec?tab=repositories)

---

*Built incrementally with an emphasis on reproducibility, evaluation, and practical engineering.*
