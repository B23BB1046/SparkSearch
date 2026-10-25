# SparkSearch — E-commerce Product Recommendations

A retrieval-augmented product recommendation assistant for interior decoration. The system retrieves relevant product information, generates grounded product explanations, and surfaces semantically related queries through a Streamlit interface.

## Features
- Product retrieval using Elasticsearch and vector-search components.
- LLM-generated explanations grounded in retrieved catalogue content.
- Related-query suggestions for further exploration.
- Two-hour query caching to reduce repeated model calls.
- Streamlit UI with screenshots and evaluation-related project folders.

## Project structure
| Directory / file | Purpose |
|---|---|
| `src/` | Application logic |
| `frontend/` | Frontend components |
| `evals/` | Evaluation-related files |
| `incremental/` | Incremental processing components |
| `screenshots/` | UI screenshots |
| `requirements.txt` | Python dependencies |

## Setup
From the repository root:
1. `cd SparkSearch-main`
2. Create and activate a Python virtual environment.
3. Install dependencies with `pip install -r requirements.txt`.
4. Configure the required API credentials, search endpoints, and cache settings through environment variables.
5. Follow the application entry-point instructions in the source files.

## Stack
Python · Streamlit · Elasticsearch · FAISS · Sentence Transformers · LangChain · Google GenAI · Redis / caching

## Evaluation
Evaluate retrieval relevance on representative interior-design queries, track response latency and cache hit rate, and check that generated descriptions do not invent product features or availability.

## Security and limitations
Do not commit API keys, credentials, or private catalogue data. Recommendations depend on catalogue quality, search configuration, and the reliability of the generated explanations.