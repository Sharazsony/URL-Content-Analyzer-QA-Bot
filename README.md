# URL Content Analyzer QA Bot

A Flask-based web application that allows users to input a URL, extract and embed its content using Google Gemini, and ask questions about the content using advanced AI models. Built with LangChain, FAISS, and Gemini API.

## Features
- Extracts and processes content from any public URL
- Splits content into chunks and creates vector embeddings
- Stores embeddings in a FAISS vector database
- Lets users ask questions about the processed content
- Uses Google Gemini for embeddings and Q&A
- Modern, responsive web UI

## Tech Stack

<p align="left">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
  <img src="https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white" alt="Flask"/>
  <img src="https://img.shields.io/badge/LangChain-2ECC40?style=for-the-badge&logo=chainlink&logoColor=white" alt="LangChain"/>
  <img src="https://img.shields.io/badge/FAISS-009688?style=for-the-badge&logo=vectorworks&logoColor=white" alt="FAISS"/>
  <img src="https://img.shields.io/badge/Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white" alt="Gemini API"/>
  <img src="https://img.shields.io/badge/Trafilatura-FF9800?style=for-the-badge&logo=readthedocs&logoColor=white" alt="Trafilatura"/>
  <img src="https://img.shields.io/badge/Bootstrap-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white" alt="Bootstrap"/>
</p>

<details>
<summary>Text List</summary>

- Python 3.10+
- Flask
- LangChain
- FAISS (faiss-cpu)
- Google Gemini API
- Trafilatura (web scraping)
- Bootstrap (frontend)

</details>

## Getting Started

### 1. Clone the repository
```bash
git clone https://github.com/Sharazsony/URL-Content-Analyzer-QA-Bot.git
cd URL-Content-Analyzer-QA-Bot
```

### 2. Create a virtual environment (recommended)
```bash
python -m venv env
# On Windows:
env\Scripts\activate
# On Mac/Linux:
source env/bin/activate
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Set up environment variables
Create a `.env` file in the project root:
```
GEMINI_API_KEY=your_google_gemini_api_key_here
SESSION_SECRET=your_flask_secret_key_here
```
**Never commit your `.env` file!**

### 5. Run the app
```bash
python BackendBuilder/app.py
```

The app will be available at [http://localhost:5000](http://localhost:5000).

## Security & Best Practices
- `.env` is in `.gitignore` to protect your API keys and secrets.
- Never share your API keys publicly.
- For production, use a production-ready WSGI server (e.g., Gunicorn, Waitress).

## License
MIT

---

**Made with ❤️ by Sharazsony**
