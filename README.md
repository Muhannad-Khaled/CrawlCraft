# CrawlCraft

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Groq](https://img.shields.io/badge/Powered%20By-Groq-orange?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

**CrawlCraft** is a reactive AI agent powered by Groq, MCP, and Firecrawl. It can crawl websites, extract structured data, and perform tool-driven reasoning. Designed for automation, research, and intelligent data gathering.

---

## 🚀 Features

- **Reactive Architecture:** Built using **LangGraph** and **MCP tools** for dynamic decision-making.
- **Advanced Crawling:** Web crawling and data extraction using **Firecrawl**.
- **Reasoning Engine:** Powered by **Groq LLM** for fast, step-by-step reasoning.
- **Data Handling:** Capable of handling structured and semi-structured web data.
- **Extensible:** Easy to extend with new tools and API integrations.

---

## 🛠 Technologies Used

- **Python 3.10+**
- **LangGraph** (Agent orchestration)
- **LangChain MCP Adapters**
- **Groq Chat Models** (`kimi-k2-instruct-0905`)
- **Firecrawl** (Web scraping)
- **AsyncIO** (Concurrent operations)

---

## 📦 Installation

### 1. Clone the repository
```bash
git clone [https://github.com/Muhannad-Khaled/CrawlCraft.git](https://github.com/Muhannad-Khaled/CrawlCraft.git)
cd CrawlCraft
```

### 2. Create and activate a virtual environment

**Windows:**
```bash
python -m venv venv
source venv/Scripts/activate
```

**Linux/macOS:**
```bash
python -m venv venv
source venv/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Set up environment variables
Create a `.env` file in the root directory and add your keys:

```ini
GROQ_API_KEY=your_groq_api_key_here
FIRECRAWL_API_KEY=your_firecrawl_api_key_here
```
> **Important:** The `.env` file is included in `.gitignore` to protect your secrets.

---

## ⚡ Usage

Run the agent with the following command:

```bash
python main.py
```

The agent will launch in the terminal and prompt you for input. You can type natural language queries or commands.

**Example Interaction:**

```text
You: Crawl the homepage of example.com and extract all email addresses

Agent: Found the following emails: contact@example.com, info@example.com
```

Type `quit` to exit the application.

---

## 🧩 Project Structure

```bash
CrawlCraft/
├─ main.py            # Entry point for the agent
├─ .env               # Environment variables (ignored by Git)
├─ .gitignore         # Files to ignore
├─ README.md          # Project documentation
├─ pyproject.toml     # Python project metadata
└─ uv.lock            # Dependency lock file
```

---

## 💡 Extending the Agent

- **Add Tools:** Add new MCP tools by modifying the tools list in `main.py`.
- **Modify Behavior:** Update the system prompts in `messages` to change how the agent reasons.
- **Integrations:** Integrate additional APIs or data sources as needed by creating new adapter functions.

---

## 🔒 Security

- **Never commit your `.env` file.**
- Keep all API keys secret.
- Rotate keys immediately if you suspect they have been leaked.

---

## ⭐️ Acknowledgements

- [LangGraph](https://langchain-ai.github.io/langgraph/)
- [LangChain MCP](https://python.langchain.com/)
- [Groq](https://groq.com/)
- [Firecrawl](https://www.firecrawl.dev/)
