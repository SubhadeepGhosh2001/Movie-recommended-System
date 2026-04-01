# 🎬 Movie Recommended System (GraphRAG)

An **AI-powered Movie Recommendation System** built using a **GraphRAG architecture** that combines **graph databases, vector search, and large language models** to generate intelligent movie suggestions.

This project uses **Neo4j, Pinecone, Gemini, and LangChain.js** to build a hybrid retrieval system capable of understanding both **semantic similarity and relationships between movies**.

---

# 🚀 Features

* 🎥 Intelligent movie recommendations
* 🧠 Hybrid **Graph + Vector Retrieval**
* 🤖 Natural language movie queries
* ⚡ Fast semantic search using embeddings
* 📊 Knowledge graph for movie relationships
* 🔍 Context-aware retrieval using GraphRAG

---

# 🧠 What is GraphRAG?

Traditional Retrieval-Augmented Generation (RAG) systems rely only on **vector similarity**, which may miss relationships between entities.
GraphRAG improves this by combining **vector embeddings with knowledge graphs**, allowing AI systems to understand both **semantic similarity and structured relationships**. ([Medium][1])

This enables:

* Better contextual retrieval
* Relationship-aware recommendations
* Reduced hallucinations
* Explainable results

---

# 🏗️ System Architecture

```
User Query
     │
     ▼
Gemini LLM
     │
     ▼
LangChain Orchestration
     │
     ├── Vector Search (Pinecone)
     │
     └── Graph Query (Neo4j)
            │
            ▼
     Context Retrieval
            │
            ▼
       LLM Response
```

---

# 🛠️ Tech Stack

### Backend

* Node.js
* LangChain.js

### AI / LLM

* Google Gemini API

### Databases

* Neo4j (Graph Database)
* Pinecone (Vector Database)

### Libraries

* `@langchain/core`
* `@langchain/google-genai`
* `neo4j-driver`
* `@pinecone-database/pinecone`
* `pdf-parse`
* `dotenv`

---

# 📂 Project Structure

```
movie_recommended_project
│
├── 1_testConnection.js
├── 7_runIndexing.js
├── 13_runQuery.js
│
├── package.json
├── .env
│
└── dataset/
```

---

# ⚙️ Installation

Clone the repository:

```bash
git clone https://github.com/SubhadeepGhosh2001/Movie-recommended-System.git
cd Movie-recommended-System
```

Install dependencies:

```bash
npm install
```

---

# 🔑 Environment Variables

Create a `.env` file:

```
GOOGLE_API_KEY=your_gemini_api_key

NEO4J_URI=your_neo4j_uri
NEO4J_USERNAME=neo4j
NEO4J_PASSWORD=your_password

PINECONE_API_KEY=your_pinecone_key
PINECONE_INDEX=your_index_name
```

---

# ▶️ Run the Project

### 1️⃣ Test database connection

```
npm run test
```

### 2️⃣ Index movie data

```
npm run index
```

### 3️⃣ Run queries

```
npm run query
```

---

# 🔍 Example Query

```
What movies are similar to Interstellar?
```

Output example:

```
Recommended Movies:
- The Martian
- Gravity
- Arrival
```

---

# 📚 Learning Outcomes

Through this project you will learn:

* GraphRAG architecture
* Knowledge graph modeling
* Vector embeddings
* LLM-powered retrieval systems
* Hybrid search (Graph + Vector)

---

# 🧑‍💻 Author

**Subhadeep Ghosh**

* AI / GenAI / Backend Developer

GitHub:
[https://github.com/SubhadeepGhosh2001](https://github.com/SubhadeepGhosh2001)

---

# ⭐ If you like this project

Give the repository a ⭐ on GitHub!
