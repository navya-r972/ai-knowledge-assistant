# AI Knowledge Assistant

An intelligent multi-agent system for processing and querying personal knowledge bases. Built with LangChain, LangGraph, and Ollama, it uses Retrieval-Augmented Generation (RAG) to provide contextual and accurate responses.

## 🚀 Features

- **Multi-Agent Intelligence**
  - Specialized agents for retrieval, research, writing, and critique
  - State preservation between agent interactions
  - Detailed logging and debugging capabilities
  - Contextual query understanding

- **Modern Web Interface**
  - Full-viewport responsive design
  - Collapsible agent reasoning sections
  - Real-time markdown rendering
  - Interactive chat experience
  - Loading animations and error handling

- **Knowledge Processing**
  - Vector-based document storage with ChromaDB
  - Support for PDF document ingestion
  - Metadata-rich document handling
  - Contextual retrieval system

## 🛠️ Technical Stack

### Backend
- Python 3.10+
- LangChain & LangGraph for agent orchestration
- Ollama for local LLM inference
- ChromaDB for vector storage
- FastAPI for API endpoints
- Unstructured for document processing

### Frontend
- HTML5 & Modern CSS
- Vanilla JavaScript
- Marked.js for markdown rendering
- Responsive Flexbox layout

## 🚦 Getting Started

1. **Set Up Python Environment**
```bash
# Create a virtual environment
python3 -m venv .venv

# Activate the virtual environment
# On Windows
.venv\Scripts\activate
# On Unix or MacOS
source .venv/bin/activate

# Upgrade pip
python3 -m pip install --upgrade pip
```

2. **Install Dependencies**
```bash
# Install all required packages
pip install -r requirements.txt
```

3. **Configure Environment**
Create a `.env` file with:
```env
GROQ_API_KEY="gsk........."
OLLAMA_MODEL="llama-3.3-70b-versatile"
```

4. **Start the Assistant**
```bash
uvicorn api:app --reload
```

5. **Access the Interface**
Open `http://localhost:8000` in your browser to start interacting with your AI Knowledge Assistant.

## 📂 Project Structure

```
.
├── api.py            # FastAPI endpoints
├── main.py           # Agent workflow and chain
├── processor.py      # Document processing
├── static/
│   └── index.html    # Web interface
├── docs/            # Knowledge base storage
└── chroma_db/       # Vector store
```

## 🤖 Agent Workflow

1. **Retriever Agent**
   - Searches knowledge base for relevant information
   - Returns context for further processing

2. **Researcher Agent**
   - Analyzes retrieved context
   - Identifies key information and relationships

3. **Writer Agent**
   - Drafts comprehensive responses
   - Incorporates context and analysis

4. **Critic Agent**
   - Reviews and refines responses
   - Ensures accuracy and completeness

## 💡 Usage

1. **Knowledge Base Setup**
   - Place documents in the `docs` directory
   - System automatically processes and indexes them

2. **Interacting with the Assistant**
   - Use the web interface to ask questions
   - View detailed agent reasoning
   - Get contextual, sourced responses

## 🔒 Security Notes

- Environment variables for configuration
- Input validation on all endpoints
- Secure document handling
- Local LLM inference

## 🚧 Known Limitations

- Requires pre-existing knowledge base
- Limited agent interaction flexibility
- Performance considerations with large documents

## 📝 Future Enhancements

- Enhanced multi-format document support
- Advanced reasoning capabilities
- Dynamic agent role assignment
- Improved error recovery
- Comprehensive unit testing

## 🤝 Contributing

Feel free to submit issues, fork the repository, and create pull requests for any improvements.

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.
