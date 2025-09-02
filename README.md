# AI Research Paper Creator

An intelligent application that creates comprehensive research papers using LangChain, LangGraph, Tavily, and Google Gemini with a proper tool-based architecture.

## 🏗️ Architecture

This application uses a sophisticated LangGraph workflow with the following components:

- **LangChain**: For AI orchestration and tool management
- **LangGraph**: For structured workflow with state management
- **Google Gemini**: For intelligent content generation
- **Tavily Tool**: For comprehensive web research
- **Document Tools**: For Word and PDF creation

## 🔧 Technologies Used

- **LangChain**: AI workflow orchestration
- **LangGraph**: State-based workflow management with tools
- **Google Gemini**: Content generation and reasoning
- **Tavily**: Web research tool integration
- **python-docx**: Word document creation tool
- **ReportLab**: PDF generation tool

## 📋 Features

- 🔍 **Web Research Tool**: Tavily API integration for real-time research
- 🤖 **AI Writing**: Google Gemini for intelligent paper generation
- 📊 **Workflow Management**: LangGraph for organized multi-step processing
- 📄 **Document Creation Tools**: Automated Word and PDF generation
- 💾 **Auto-save**: Documents saved in `doc/` folder
- 📈 **Graph Visualization**: Visual representation of the workflow

## 🚀 Quick Start

```bash
# Install dependencies
pip install -r requirements.txt

# Run the application
python main.py
```

The application will:
1. Check API keys
2. Prompt for research topic
3. Optionally show LangGraph visualization
4. Create research paper with documents

## 🔄 Workflow Process

1. **Research Node**: Takes user topic and plans research strategy
2. **Tools Execution**: Calls Tavily research tool for web data
3. **Writer Node**: Analyzes research and generates structured paper
4. **Document Tools**: Creates Word document and PDF files
5. **Completion**: Saves files and provides user feedback

## 📁 File Structure

```
Ai_DocEditor/
├── main.py                    # Main LangGraph application
├── requirements.txt           # Python dependencies
├── .env                       # Environment variables (API keys)
├── doc/                       # Output folder
│   ├── langgraph_workflow.png # LangGraph visualization
│   └── *.docx, *.pdf         # Generated research papers
└── README.md                 # Documentation
```

## 🛠️ Tools Architecture

### Tavily Research Tool
- **Purpose**: Web research and data gathering
- **Input**: Research query string
- **Output**: Formatted research results with sources

### Word Document Tool
- **Purpose**: Create formatted Word documents
- **Input**: Paper content and topic
- **Output**: Path to created .docx file

### PDF Creation Tool
- **Purpose**: Generate PDF from content
- **Input**: Document path or content
- **Output**: Path to created .pdf file

## 📊 LangGraph Visualization

The application includes built-in LangGraph visualization:

- **PNG Graph**: Professional workflow diagram using LangGraph's native visualization
- **Auto-Generated**: Created when you choose to view the graph
- **Saved**: Automatically saved as `doc/langgraph_workflow.png`

The graph shows:
- Node connections and flow
- State transitions
- Tool integrations
- Workflow structure

## 🔧 API Configuration

### Google Gemini API
- Get your key: [Google AI Studio](https://makersuite.google.com/app/apikey)
- Set in `.env`: `GOOGLE_API_KEY=your_key_here`

### Tavily API
- Get your key: [Tavily](https://app.tavily.com/)
- Set in `.env`: `TAVILY_API_KEY=your_key_here`

## 🚨 Troubleshooting

### Common Issues:

1. **Import Errors**
   ```bash
   pip install -r requirements.txt
   ```

2. **API Key Issues**
   - Verify keys are set in `.env` file
   - Check API key validity and quotas

3. **Tool Execution Errors**
   - Ensure internet connectivity for Tavily
   - Check file permissions for document creation

4. **LangGraph Errors**
   - Verify all required packages are installed
   - Check Python version compatibility (3.8+)

## 📈 Example Usage

```python
# Run the main application
python main.py

# Input: "artificial intelligence in healthcare"
# Output: 
#   - Word document with comprehensive research paper
#   - PDF version of the same paper
#   - Proper academic structure with citations
```

## 🎯 Advanced Features

- **State Management**: Conversation context preservation
- **Error Recovery**: Graceful handling of API failures
- **Tool Chaining**: Sequential tool execution
- **Memory Checkpointing**: Workflow state persistence
- **Async Processing**: Non-blocking operation execution

## 📜 License

This project is open source. Feel free to modify and distribute.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
