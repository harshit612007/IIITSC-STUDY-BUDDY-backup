# 🎓 Study-Buddy

<div align="center">

![Study-Buddy Banner](https://img.shields.io/badge/Study--Buddy-AI%20Assistant-007AFF?style=for-the-badge&logo=apple&logoColor=white)

**AI-powered learning assistant that thinks like you do.**

[![Made with Streamlit](https://img.shields.io/badge/Made%20with-Streamlit-FF4B4B?style=flat-square&logo=streamlit)](https://streamlit.io)
[![Powered by Groq](https://img.shields.io/badge/Powered%20by-Groq-000000?style=flat-square)](https://groq.com)
[![Powered by Google Gemini](https://img.shields.io/badge/Powered%20by-Google%20Gemini-4285F4?style=flat-square&logo=google)](https://ai.google.dev)
[![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue?style=flat-square&logo=python)](https://www.python.org)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)

[Demo](#-demo) • [Features](#-features) • [Installation](#-installation) • [Usage](#-usage) • [Deployment](#-deployment)

</div>

---

## 📖 About

**Study-Buddy** is an intelligent learning assistant designed for IIIT Sri City students. It combines the power of **Retrieval-Augmented Generation (RAG)**, **conversational AI**, and **document processing** to help students learn more effectively.

Upload your study materials, ask questions, and even generate professional question papers—all powered by cutting-edge AI from **Groq** and **Google Gemini**.

---

## ✨ Features

### 🧠 **Smart RAG (Retrieval-Augmented Generation)**
- Upload PDFs and text files
- Get instant, context-aware answers from your documents
- Semantic search using state-of-the-art embeddings
- View source citations for transparency

### 📝 **Question Paper Generation**
- Generate professional exam papers in seconds
- Download in **both PDF and DOCX formats**
- Editable Word documents with proper formatting
- Customizable topics and difficulty levels

### 💬 **Conversational AI**
- Natural dialogue with context memory
- Works with or without uploaded documents
- General knowledge questions answered intelligently
- Powered by Groq's Llama 3.3 70B + Google Gemini models

### 🎨 **Beautiful Apple-Style UI**
- Dark gradient theme inspired by Apple.com
- Glassmorphism effects with blur
- Smooth animations and transitions
- Fully responsive design

### 🚀 **Free & Fast**
- No API costs for embeddings (uses HuggingFace)
- Free Groq API tier available
- Instant responses
- Works offline after initial setup

---

## 🎥 Demo

### Main Interface
```
┌─────────────────────────────────────────────┐
│           🎓 Study-Buddy                    │
│   AI-powered learning assistant             │
└─────────────────────────────────────────────┘

┌──────────┐  ┌──────────┐  ┌──────────┐
│ 🧠 Smart │  │ 📝 Papers│  │ 💬 Chat  │
│   RAG    │  │ Generator│  │ Context  │
└──────────┘  └──────────┘  └──────────┘

        📚 Upload Your Documents
        Drop PDFs or text files here
```

### Example Conversations

**Document-based Query:**
```
👤 What are the main topics in this textbook?
🤖 Based on the document, the main topics include:
   1. Data Structures (Arrays, Trees, Graphs)
   2. Algorithms (Sorting, Searching)
   3. Complexity Analysis
   📚 View Sources → [Shows relevant excerpts]
```

**Question Paper Generation:**
```
👤 Generate a question paper on Python with 10 MCQs
🤖 [Displays formatted question paper]
   📥 Download PDF | 📄 Download DOCX
```

---

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- pip package manager
- Groq API key ([Get free key](https://console.groq.com/keys))

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/harshit612007/study-buddy.git
   cd study-buddy
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables** (Optional)
   
   Create a `.env` file:
   ```env
   GROQ_API_KEY=your_groq_api_key_here
   ```

4. **Run the application**
   ```bash
   streamlit run app.py
   ```

5. **Open your browser**
   
   Navigate to `http://localhost:8501`

---

## 📦 Tech Stack

| Technology | Purpose |
|------------|---------|
| **Streamlit** | Web framework for the UI |
| **Groq** | LLM API (Llama 3.3 70B) |
| **Google Gemini** | Alternative LLM support |
| **LangChain** | RAG orchestration |
| **HuggingFace** | Free embeddings model |
| **FAISS** | Vector database for search |
| **python-docx** | DOCX generation |
| **FPDF** | PDF generation |
| **PyPDF** | PDF document loading |

---

## 📚 Usage Guide

### 1. Configure API Key
- Enter your Groq API key in the configuration section
- Or set it in your `.env` file
- Get a free key at [console.groq.com](https://console.groq.com/keys)

### 2. Upload Documents
- Click on the file uploader
- Select PDF or TXT files
- Click "🚀 Process Documents"
- Wait for processing to complete

### 3. Ask Questions
**Document-based queries:**
```
"Summarize chapter 3"
"What is the attendance policy?"
"Explain the lab safety rules"
```

**General knowledge:**
```
"Explain binary search trees"
"What's the difference between TCP and UDP?"
"Write a Python function to reverse a string"
```

### 4. Generate Question Papers
```
"Generate a question paper on Data Structures"
"Create an exam with 10 MCQs on Python"
"Make a test on Operating Systems"
```

Download the generated paper in:
- **PDF** format (for printing)
- **DOCX** format (editable in Word)

---

## 🎨 UI Features

### Apple-Inspired Design
- **Dark gradient backgrounds** with smooth transitions
- **Glassmorphism effects** with backdrop blur
- **Smooth animations** using cubic-bezier curves
- **Gradient text** in hero section
- **Custom scrollbars** with blue accents

### Interactive Elements
- **Feature cards** that lift on hover
- **Status badges** with live updates
- **Expandable sections** for cleaner interface
- **Professional buttons** with shadow effects
- **Responsive layout** for all screen sizes

---

## 🌐 Deployment

### Deploy to Streamlit Cloud (Recommended)

1. **Push to GitHub**
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **Deploy on Streamlit Cloud**
   - Go to [share.streamlit.io](https://share.streamlit.io)
   - Click "New app"
   - Select your repository
   - Add secrets in TOML format:
     ```toml
     GROQ_API_KEY = "your_api_key_here"
     ```
   - Click "Deploy"

3. **Your app is live!** 🎉
   ```
   https://your-app-name.streamlit.app
   ```

### Other Deployment Options
- **Hugging Face Spaces** - [huggingface.co/spaces](https://huggingface.co/spaces)
- **Railway** - [railway.app](https://railway.app)
- **Render** - [render.com](https://render.com)

See [DEPLOYMENT.md](DEPLOYMENT.md) for detailed instructions.

---

## 📁 Project Structure

```
study-buddy/
├── app.py                 # Main Streamlit application
├── requirements.txt       # Python dependencies
├── .env.example          # Example environment file
├── .gitignore            # Git ignore rules
├── README.md             # This file
└── docs/
    ├── DEPLOYMENT.md     # Deployment guide
    └── TESTING.md        # Local testing guide
```

---

## 🔧 Configuration

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `GROQ_API_KEY` | Groq API key for LLM | Yes |

### Application Settings

Customize in `app.py`:

```python
# Model configuration
model="llama-3.3-70b-versatile"
temperature=0.7

# Document processing
chunk_size=3000
chunk_overlap=200

# Retrieval settings
search_kwargs={"k": 4}
```

---

## 🐛 Troubleshooting

### Common Issues

**App won't start**
```bash
# Check Python version
python --version  # Need 3.8+

# Reinstall dependencies
pip install --upgrade pip
pip install -r requirements.txt
```

**API key errors**
- Verify key starts with `gsk_`
- Check for extra spaces in `.env`
- Enter key directly in app interface

**Upload fails**
- File size limit: 200MB
- Supported formats: PDF, TXT
- Try with smaller test file

**Slow performance**
- First run downloads ~90MB model (one-time)
- Reduce `chunk_size` for large documents
- Process fewer documents at once

### Get Help
- [Streamlit Docs](https://docs.streamlit.io)
- [Groq Documentation](https://console.groq.com/docs)
- [LangChain Guide](https://python.langchain.com)
- [Open an Issue](https://github.com/harshit612007/study-buddy/issues)

---

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/amazing-feature
   ```
3. **Commit your changes**
   ```bash
   git commit -m "Add amazing feature"
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/amazing-feature
   ```
5. **Open a Pull Request**

### Development Setup
```bash
# Clone your fork
git clone https://github.com/harshit612007/study-buddy.git

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run in development mode
streamlit run app.py
```

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **Groq** - For providing fast LLM inference
- **Google Gemini** - For powerful AI capabilities
- **Streamlit** - For the amazing web framework
- **HuggingFace** - For free embedding models
- **LangChain** - For RAG orchestration
- **Apple** - For design inspiration
- **IIIT Sri City** - For being awesome 🎓

---

## 📧 Contact

**Developer:** Harshit Pansari  
**Email:** harshitpansari15@gmail.com  
**GitHub:** [@harshit612007](https://github.com/harshit612007)  
**LinkedIn:** [Harshit Pansari](https://www.linkedin.com/in/harshit-pansari-065514383)

---

## 🗺️ Roadmap

### Version 2.0 (Coming Soon)
- [ ] Multi-language support
- [ ] Voice input/output
- [ ] Collaborative study rooms
- [ ] Mobile app (React Native)
- [ ] Study analytics dashboard
- [ ] Flashcard generation
- [ ] Practice quiz mode
- [ ] Export to Notion/Obsidian

### Version 1.1 (Current)
- [x] PDF & DOCX question paper generation
- [x] Apple-style UI
- [x] Document upload & RAG
- [x] Conversational AI
- [x] Source citations

---

## ⭐ Star History

If you find this project helpful, please consider giving it a star! ⭐

[![Star History Chart](https://api.star-history.com/svg?repos=harshit612007/study-buddy&type=Date)](https://star-history.com/#harshit612007/study-buddy&Date)

---

## 📊 Stats

![GitHub stars](https://img.shields.io/github/stars/harshit612007/study-buddy?style=social)
![GitHub forks](https://img.shields.io/github/forks/harshit612007/study-buddy?style=social)
![GitHub watchers](https://img.shields.io/github/watchers/harshit612007/study-buddy?style=social)

---

<div align="center">

**Made with ❤️ for students, by students**

[⬆ Back to Top](#-study-buddy)

</div>
