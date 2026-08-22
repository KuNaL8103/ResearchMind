# 🔬 ResearchMind - Multi-Agent Research System

ResearchMind is an AI-powered research assistant that leverages multiple specialized agents to perform web research, extract information, generate reports, and evaluate output quality.

## Features

- **Search Agent** — Finds relevant information using Tavily Search.
- **Reader Agent** — Extracts and summarizes content from the most relevant source.
- **Writer Chain** — Generates a structured research report.
- **Critic Chain** — Reviews and scores the generated report for quality and completeness.
- **Streamlit UI** — Interactive web interface for running research workflows.

---

## System Architecture

```text
User Query
    │
    ▼
Search Agent
    │
    ▼
Reader Agent
    │
    ▼
Writer Chain
    │
    ▼
Critic Chain
    │
    ▼
Final Research Report
```

---

## Tech Stack

- Python
- LangChain
- Groq LLM
- Tavily Search API
- Streamlit

---

## Installation

Clone the repository:

```bash
git clone https://github.com/KuNaL8103/MultiAgent-Research-System.git
cd MultiAgent-Research-System
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Create a `.env` file:

```bash
cp .env.example .env
```

Add your API keys:

```env
GROQ_API_KEY=your_groq_api_key
TAVILY_API_KEY=your_tavily_api_key
```

---

## Usage

### Run from Command Line

```bash
python pipeline.py
```

### Run the Web Interface

```bash
streamlit run app.py
```

---

## Project Structure

```text
ResearchMind/
│
├── agents.py 
├── pipeline.py 
├── app.py 
├── tools.py
├── requirements.txt
├── .env.example 
└── README.md
```

---

## Workflow

1. User submits a research query.
2. Search Agent retrieves relevant web sources.
3. Reader Agent extracts detailed information from the top source.
4. Writer Chain generates a structured report.
5. Critic Chain evaluates and scores the report.
6. Final report and feedback are displayed to the user.

---
