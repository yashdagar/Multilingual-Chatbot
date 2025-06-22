


### 📥 Installation Steps
1️⃣ Clone the repository:
```bash
git clone 
cd 
```

2️⃣ Create and activate virtual environment:
```bash
python -m venv rag_env
source rag_env/bin/activate  # On Windows: rag_env\Scripts\activate
```

3️⃣ Install dependencies:
```bash
cd backend
pip install -r requirements
```

## 🚀 Usage Guide

### 🦙 Running the Ollama server (open-source LLM)
📥 Download Ollama from [Ollama Official Site](https://ollama.com/download)

Run the following commands in terminal:
```bash
ollama serve
ollama run llama3.1
```
To stop the server:
```bash
ollama stop llama3.1
```

### 🦙 Downloading the embeddings model (Fasttext by Facebook Research)
Run the following commands in terminal in the backend/app/models folder:
```bash
wget https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.en.300.bin.gz
gunzip cc.en.300.bin.gz
```


### ▶️ Running the Project (after creating your environment)

1️⃣ Start the FastAPI server:
```bash
cd backend
uvicorn app.main:app --reload
```

2️⃣ Start the frontend server:
```bash
cd frontend
npm i
npm run dev
```

