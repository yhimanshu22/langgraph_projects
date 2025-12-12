# LangGraph AI Projects

This repository contains a collection of agentic AI applications built using **LangGraph**, **LangChain**, and **Ollama**. The projects demonstrate various patterns of building stateful, multi-agent workflows.

## 📂 Projects

### 1. AI Study Planner
A smart scheduling assistant that generates personalized study plans.
- **`ai_study_planner.ipynb`**: A simple planner that takes subjects and time constraints to generate a schedule.
- **`god_level_ai_study_planner.ipynb`**: An advanced, multi-agent system featuring:
  - **🧠 Strategist**: Analyzes the difficulty of subjects.
  - **📅 Architect**: Creates a detailed Markdown timetable.
  - **⚖️ Auditor**: Reviews the schedule for formatting and quality (includes a feedback loop).
  - **🔗 Librarian**: Curates YouTube learning resources for each subject.

### 2. Sentiment Analysis & Routing
- **`sentiment_classifier.ipynb`**: A tool to classify text sentiment and potentially route it to different handlers (implied by the folder name `sentiment_router`).

### 3. Productivity Tools
- **`email_summarizer.ipynb`**: Summarizes incoming emails.
- **`emailer.ipynb`**: Automates email drafting or sending.
- **`habit_tracker_with_motivation_messages.ipynb`**: Tracks habits and provides motivational feedback.

### 4. RAG (Retrieval-Augmented Generation)
- **`qa_bot_rag.ipynb`**: A Question-Answering bot capable of retrieving information from external sources.

## 🛠️ Tech Stack
- **Python 3.12**
- **LangGraph**: For building stateful, cyclic multi-agent workflows.
- **LangChain**: For LLM orchestration and prompting.
- **Ollama**: Local LLM inference (using `qwen2.5:0.5b`).

## 🚀 Getting Started

### Prerequisites
1. **Install Ollama**: Download and install [Ollama](https://ollama.com/).
2. **Pull the Model**:
   ```bash
   ollama pull qwen2.5:0.5b
   ```

### Installation
1. Clone the repository.
2. Create a virtual environment:
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```
3. Install dependencies (based on notebook usage):
   ```bash
   pip install langchain-ollama langchain-community langchain-core langgraph duckduckgo-search
   ```

### Usage
Open any `.ipynb` file in Jupyter Notebook or VS Code and run the cells to execute the agentic workflows.
