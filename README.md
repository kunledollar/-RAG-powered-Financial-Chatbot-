# 📊 AI-Powered Financial Chatbot (RAG + Streamlit + FastAPI)

This project is a Retrieval-Augmented Generation (RAG) based chatbot that uses real-time stock data and internal financial documents to answer finance-related questions intelligently.

## 🔧 Features

- 💬 RAG-powered Q&A with financial PDFs (LangChain)
- 📈 Live stock data via yfinance
- 🧠 Agentic workflows using prompt engineering
- 🌐 FastAPI backend + Streamlit UI

## 📂 Project Structure

- `backend/` — Handles the API, RAG chain, and real-time finance logic
- `streamlit_app/` — Interactive front-end for user chat
- `data/` — RAG-ready financial documents (e.g., Apple Q1 2025 report)

## 🚀 How to Run Locally

```bash
# Clone the repo
git clone https://github.com/yourusername/financial-chatbot.git
cd financial-chatbot

# Set up Python environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Start the backend
uvicorn backend.main:app --reload

# In a new terminal, run the Streamlit app
streamlit run streamlit_app/app.py
