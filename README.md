# QuickQuizzer ֎

An intelligent flashcard and practice test generator powered by AI that helps students create personalized study materials from any topic or uploaded documents.

## 🌟 Features

### 📇 Smart Flashcards
- **Interactive Flip Cards**: Beautiful animated flashcards with click-to-flip functionality
- **Multiple Choice Questions**: AI-generated MCQs with 4 options each
- **Instant Feedback**: Color-coded correct/incorrect answers
- **Navigation**: Easy previous/next navigation through flashcard sets

### 🚀 Practice Tests
- **Multiple Question Types**: 
  - Multiple Choice Questions
  - Fill in the Blank
  - True/False
  - Question & Answer (open-ended)
- **Intelligent Scoring**: AI-powered evaluation for all question types
- **Detailed Results**: Comprehensive feedback with explanations
- **Session Review**: AI-generated overall performance analysis

### 📄 Document Integration
- **File Upload Support**: PDF, DOCX, and PPTX files
- **Context-Aware Generation**: Questions based on your uploaded content
- **Curriculum Database**: Connect to school curriculum databases via LlamaIndex
- **Smart Context Retrieval**: Vector database search for relevant educational content

### ⚙ Customization
- **Flexible Question Counts**: Configure 0-7 questions per type
- **Topic-Based Generation**: Generate content for any subject
- **Progressive Learning**: Track performance across sessions

## 🛠️ Technology Stack

- **Frontend**: Streamlit with custom HTML/CSS/JavaScript
- **AI Engine**: Groq API with Llama-3-70B model
- **Document Processing**: PyPDF2, python-docx, python-pptx
- **Vector Database**: LlamaIndex Cloud integration
- **HTTP Client**: httpx for robust API calls

## 📋 Prerequisites

- Python 3.8+
- Groq API key
- LlamaIndex API key (optional, for curriculum database)

## 🚀 Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sathvik3103/QuickQuizzer.git
   cd QuickQuizzer
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up API keys**:
   - Get your Groq API key from [Groq Console](https://console.groq.com/)
   - (Optional) Get LlamaIndex API key for curriculum database features
   - Update the `.env` file with your actual API keys

4. **Run the application**:
   ```bash
   streamlit run flashcard_demo.py
   ```

## 📖 Usage

### Generating Flashcards
1. Enter your study topic in the input field
2. (Optional) Upload PDF, DOCX, or PPTX files for context
3. (Optional) Enable curriculum database connection
4. Click "📇 Generate Flash Cards" 
5. Navigate through your personalized flashcards

### Creating Practice Tests
1. Enter your study topic
2. Configure question counts in the sidebar (0-7 per type)
3. Upload context documents if needed
4. Click "🚀 Generate Practice Test"
5. Answer questions and receive detailed feedback

### Document Upload
- Supports PDF, DOCX, and PPTX files
- Automatically extracts text content
- Generates questions based on document content
- Preview functionality for uploaded PDFs

## ⚡ Key Features Explained

### AI-Powered Question Generation
- Uses advanced language models for intelligent question creation
- Supports multiple question formats automatically
- Context-aware generation from uploaded documents

### Smart Answer Evaluation
- Exact matching for MCQ, True/False, and Fill-in-the-blank
- AI evaluation for open-ended questions with scoring (0-1 scale)
- Detailed explanations for all answer types

### Enhanced User Experience
- Modern, responsive design with custom CSS
- Animated flashcard interactions
- Progress tracking and session management
- Comprehensive result analytics

## 🔧 Configuration

### Environment Variables (.env file)
```bash
# Required
GROQ_API_KEY=your_groq_api_key_here

# Optional - for curriculum database features
LLAMA_INDEX_API_KEY=your_llamaindex_api_key_here
VECTOR_DB_INDEX_ID=your_index_id_here
VECTOR_DB_PROJECT_ID=your_project_id_here
VECTOR_DB_ORG_ID=your_organization_id_here
```

## 📊 Question Types & Scoring

| Question Type | Scoring Method | Max Score |
|--------------|----------------|-----------|
| Multiple Choice | Exact Match | 1.0 |
| True/False | Exact Match | 1.0 |
| Fill in the Blank | Exact Match | 1.0 |
| Question & Answer | AI Evaluation | 1.0 |

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **Groq** for providing fast and reliable AI model access
- **LlamaIndex** for vector database and retrieval capabilities
- **Streamlit** for the excellent web framework
- Open source libraries: PyPDF2, python-docx, python-pptx

## 📞 Support

If you encounter any issues or have questions, please:
1. Check the existing issues on GitHub
2. Create a new issue with detailed information
3. Provide error logs and steps to reproduce

---

**Made with ❤️ for better learning experiences**
