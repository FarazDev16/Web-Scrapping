# Website Summarizer with OpenAI

This project fetches the content of a given website, cleans it up with **BeautifulSoup**, and uses the **OpenAI API** to generate a short Markdown-formatted summary.  
It works in both **Jupyter Notebooks** and **VS Code terminal** (with `rich` for pretty output).

---

## 🚀 Features
- Fetches and parses any website using `requests` + `BeautifulSoup`
- Cleans irrelevant elements (scripts, styles, images, inputs)
- Uses OpenAI GPT models to generate a **short summary** of the website
- Displays results in:
  - **Jupyter Notebook** (rendered Markdown)
  - **VS Code / Terminal** (styled Markdown via `rich`)

---

## 📦 Installation

1. Clone this repo or copy the script files.
2. Create a Python virtual environment (recommended):

   ```bash
   python -m venv venv
   source venv/bin/activate   # macOS/Linux
   venv\Scripts\activate      # Windows


pip install -r requirements.txt

🔑 Setup OpenAI API Key

Create a .env file in the project root.

Add your OpenAI API key inside:

OPENAI_API_KEY=sk-proj-xxxxxxxxxxxxxxxxxxxxxxxx

Run the script to summarize a website:

python WebScrapping.py

📂 Project Structure
.
├── WebScrapping.py
├── requirements.txt
├── README.md
└── .env