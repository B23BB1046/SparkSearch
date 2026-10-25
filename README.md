# SparkSearch — E-commerce Product Recommendations

A retrieval-augmented product recommendation assistant for interior decoration. It searches a product catalogue, uses a language model to explain relevant products, and suggests semantically related queries in a Streamlit interface.

## Highlights
- Retrieval over product information using Elasticsearch and vector-search components.
- RAG-based product explanations generated from retrieved product context.
- Similar-query suggestions to help users explore related needs.
- Two-hour query caching to reduce repeated LLM calls and improve responsiveness.
- Streamlit UI with screenshots and evaluation-related project folders.

## Repository layout
The project source is organized under `SparkSearch-main/`.

| Path | Purpose |
|---|---|
| `SparkSearch-main/README.md` | Original project overview and UI context |
| `SparkSearch-main/requirements.txt` | Python dependencies |
| `SparkSearch-main/src/` | Application source |
| `SparkSearch-main/frontend/` | Frontend components |
| `SparkSearch-main/evals/` | Evaluation-related files |
| `SparkSearch-main/incremental/` | Incremental processing components |
| `SparkSearch-main/screenshots/` | UI screenshots |

## Getting started
1. Clone the repository:
   `git clone https://github.com/B23BB1046/SparkSearch.git`
2. Enter the project directory: `cd SparkSearch/SparkSearch-main`
3. Create and activate a Python virtual environment.
4. Install dependencies: `pip install -r requirements.txt`.
5. Configure required service credentials and endpoints using environment variables. Do not commit secrets.
6. Follow the entry-point and service configuration documented in the source code.

## Tech stack
Python · Streamlit · Elasticsearch · FAISS · Sentence Transformers · LangChain · Google GenAI · Redis / caching

## Evaluation and reliability
Product recommendations depend on catalogue quality, retrieval relevance, and the grounding of generated explanations. Evaluate retrieval with representative queries, measure latency and cache hit rate, and verify that generated descriptions do not invent product properties.

## Future improvements
- Document index creation, required environment variables, and startup commands in detail.
- Add sample data or a safe demo mode that works without private catalogue credentials.
- Report retrieval metrics, response latency, and caching performance.
- Add tests for search, caching, and failure handling.