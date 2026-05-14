
# Agentic Story Intelligence & Personalization Engine

LangGraph-based multi-agent AI system for story analysis, contextual retrieval, memory-driven recommendations, and AI workflow orchestration using RAG and FastAPI.

This project uses LangGraph and LangChain to build collaborative AI agents capable of analyzing stories, extracting metadata, retrieving contextual memory, and generating personalized content recommendations through structured multi-step workflows.

## Features

- Multi-agent workflow orchestration using LangGraph
- RAG-based contextual retrieval with ChromaDB
- Story summarization and metadata extraction
- Genre and theme classification
- Personalized story recommendations
- Structured JSON outputs
- FastAPI backend APIs
- Stateful workflow execution
- Persistent memory using vector search

---

# Agent Workflow

The system uses multiple specialized AI agents that collaborate together to process story-related tasks.

### Agents

- Planner Agent
- Story Retriever Agent
- Story Analysis Agent
- Genre Classification Agent
- Recommendation Agent
- Validation Agent

---

# Architecture Flow

```text
User Query
   ↓
Planner Agent
   ↓
Retriever Agent → ChromaDB / Vector Search
   ↓
Story Analysis Agent
   ↓
Recommendation Agent
   ↓
Validation Agent
   ↓
Structured JSON Response
````

---

# Example Use Cases

* Analyze uploaded stories
* Generate concise summaries
* Extract genres, themes, and characters
* Recommend stories based on user preferences
* Retrieve contextual memory using RAG
* Generate structured metadata for content pipelines

---

# Example JSON Output

```json
{
  "title": "The Last Letter",
  "genre": "Emotional Drama",
  "themes": ["love", "loss", "family"],
  "characters": ["Aarav", "Meera"],
  "summary": "A story about two childhood friends reconnecting after years apart.",
  "recommendation_reason": "Recommended because the user prefers emotional character-driven stories."
}
```

---

# Tech Stack

## AI / LLM Systems

* LangGraph
* LangChain
* RAG (Retrieval-Augmented Generation)
* ChromaDB
* Vector Embeddings
* Structured Prompting
* Tool Calling

## Backend

* FastAPI
* Python
* REST APIs
* Async Workflow Execution

## Storage

* PostgreSQL
* ChromaDB
* SQLite Fallback

---

# API Endpoints

## Analyze Story

```http
POST /analyze-story
```

Analyzes uploaded story content and generates structured metadata.

---

## Generate Summary

```http
POST /story-summary
```

Generates concise summaries for long-form content.

---

## Extract Metadata

```http
POST /extract-metadata
```

Extracts genres, themes, characters, and contextual signals.

---

## Recommend Stories

```http
POST /recommend-story
```

Generates personalized story recommendations using contextual memory and user preferences.

---

# Project Structure

```text
agentic-story-intelligence-engine/
│
├── story_agents/
├── service/
├── scripts/
├── schema/
├── client/
├── data/
├── media/
├── docker/
│
├── run_service.py
├── streamlit_app.py
├── requirements.txt
├── compose.yaml
└── README.md
```

---

# Setup

## Clone Repository

```bash
git clone https://github.com/N-Aryan/agentic-story-intelligence-engine.git
cd agentic-story-intelligence-engine
```

---

## Install Dependencies

```bash
pip install -r requirements.txt
```

---

## Run Backend Service

```bash
python run_service.py
```

---

## Run Streamlit UI

```bash
streamlit run streamlit_app.py
```

---

# Future Improvements

* Hybrid retrieval pipelines
* Long-term conversational memory
* Multi-user personalization
* Real-time recommendation streaming
* Fine-tuned open-source LLM integration
* Audio-story understanding workflows

---

# License

MIT License

```
```
