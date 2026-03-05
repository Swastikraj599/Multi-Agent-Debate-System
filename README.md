# 🤖 Multi-Agent AI Debate System

[![Live Demo](https://img.shields.io/badge/🚀-Live%20Demo-blue)](YOUR_HUGGINGFACE_SPACE_URL)
[![Python](https://img.shields.io/badge/Python-3.11-green.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

> An innovative AI application that simulates expert panel discussions using multiple AI agents with distinct perspectives, expertise, and reasoning approaches.

![Multi-Agent Debate System](https://img.shields.io/badge/Status-Production%20Ready-success)

---

## 📋 Table of Contents

- [Overview](#overview)
- [Key Features](#key-features)
- [Live Demo](#live-demo)
- [Tech Stack](#tech-stack)
- [Installation](#installation)
- [Usage Guide](#usage-guide)
- [Project Architecture](#project-architecture)
- [Advanced Features](#advanced-features)
- [Use Cases](#use-cases)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 🎯 Overview

The **Multi-Agent AI Debate System** is an innovative application that demonstrates advanced concepts in Generative AI and Agentic AI by orchestrating autonomous agents to engage in structured debates on complex topics.

### The Problem
Complex decisions often benefit from multiple perspectives, but traditional AI systems typically provide a single viewpoint.

### The Solution
This system simulates expert panel discussions where three AI agents with different expertise and stances debate topics, challenge each other's reasoning, and provide comprehensive analysis.

**Built for:** Wipro AI Track Training Assessment  
**Focus Areas:** Deep Learning, Machine Learning, Generative AI, Agentic AI  
**Development Period:** February 2026

---

## ✨ Key Features

### 🎭 Three Distinct AI Agents
Each agent has a unique role, expertise area, and stance:
- **Dr. Sarah Chen** - AI Ethics Researcher (Cautious perspective)
- **Marcus Rivera** - Tech Entrepreneur (Optimistic perspective)  
- **Prof. Anika Sharma** - Policy Expert (Balanced perspective)

### 📊 Intelligent Scoring System
- Automated evaluation of argument quality and strength
- Keyword-based scoring algorithm
- Medal-based ranking system (🥇🥈🥉)

### 🔄 Multi-Round Debates
- Configurable debate rounds (1-4 rounds)
- Context-aware argument generation
- Progressive discussion development

### 👥 Custom Agent Personalities
- **NEW!** Create your own agents with custom:
  - Names and professional identities
  - Expertise areas and roles
  - Stances and perspectives

### 📚 Debate History
- **NEW!** Automatic tracking of all debates
- View past debates by number
- Statistics and performance tracking
- JSON-based storage system

### 📄 PDF Export
- **NEW!** Professional debate reports
- Download debates as formatted PDFs
- Include all rounds, scores, and analysis
- Shareable documentation

### 💡 Comprehensive Analysis
- Detailed insights and key takeaways
- Argument strength comparison
- Multi-perspective conclusions

### 🎨 Interactive UI
- User-friendly Gradio interface
- Real-time debate visualization
- Tabbed navigation system
- Example topics for quick start

---

## 🚀 Live Demo

**Try it now:** [YOUR_HUGGINGFACE_SPACE_URL]

No installation required! The app is deployed on Hugging Face Spaces with:
- ✅ Free, permanent hosting
- ✅ Public accessibility
- ✅ Automatic scaling
- ✅ 24/7 availability

---

## 🛠️ Tech Stack

### Core Technologies
- **Python 3.11** - Primary programming language
- **Transformers (Hugging Face)** - NLP model implementation
- **GPT-2** - Base language model for text generation
- **Gradio 6.8.0** - Interactive web interface
- **ReportLab** - PDF generation

### Libraries & Dependencies
```
transformers - Natural Language Processing
torch - Deep learning framework
gradio - Web UI framework
reportlab - PDF document generation
accelerate - Model optimization
```

### Development Tools
- Google Colab - Development environment
- Hugging Face Spaces - Deployment platform
- Git/GitHub - Version control

---

## 📥 Installation

### Option 1: Google Colab (Recommended for Quick Demo)

1. **Open Google Colab:** https://colab.research.google.com
2. **Create New Notebook**
3. **Install Dependencies:**
```python
!pip install -q transformers accelerate gradio reportlab
```

4. **Clone Repository:**
```python
!git clone https://github.com/Swastikraj599/Multi-Agent-Debate-System.git
%cd Multi-Agent-Debate-System
```

5. **Run the Application:**
```python
!python app.py
```

### Option 2: Local Installation

1. **Clone the Repository:**
```bash
git clone https://github.com/Swastikraj599/Multi-Agent-Debate-System.git
cd Multi-Agent-Debate-System
```

2. **Create Virtual Environment:**
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. **Install Dependencies:**
```bash
pip install -r requirements.txt
```

4. **Run the Application:**
```bash
python app.py
```

5. **Access the Interface:**
Open your browser and go to: `http://localhost:7860`

---

## 📖 Usage Guide

### Basic Usage

1. **Enter Topic:** Type any debate-worthy topic in the text field
   - Example: "Should AI development be regulated by governments?"

2. **Select Rounds:** Use slider to choose 1-4 debate rounds
   - 2 rounds recommended for quick demos
   - 3-4 rounds for comprehensive debates

3. **Start Debate:** Click the "🎬 Start Debate" button

4. **View Results:** Watch the debate unfold with real-time arguments

5. **Analyze Scores:** Review the scoring and ranking at the end

6. **Download PDF:** Get a professional report of the debate

### Advanced Usage

#### Custom Agent Personalities

1. Go to **"👥 Custom Agents"** tab
2. Fill in agent details:
   - **Name:** Professional identity
   - **Role:** Area of expertise
   - **Stance:** Perspective on issues
3. Enable "Use Custom Agents" checkbox
4. Start your debate

#### View Debate History

1. Go to **"📚 Debate History"** tab
2. Click **"🔄 Refresh History"** to see all debates
3. Enter a debate number and click **"📖 Load Debate"** to view details

### Example Topics

**Technology:**
- "Should AI development be regulated by governments?"
- "Will AI replace human jobs or create new opportunities?"

**Work Culture:**
- "Is remote work better than office work for productivity?"

**Social Media:**
- "Should social media companies be responsible for content moderation?"

**Economy:**
- "Should cryptocurrencies replace traditional currency?"

---

## 🏗️ Project Architecture

### System Design
```
User Input (Topic)
      ↓
Debate Orchestrator
      ↓
┌─────────────────────────────────┐
│  Agent 1   Agent 2   Agent 3    │
│ (Cautious) (Optimistic) (Balanced)│
└─────────────────────────────────┘
      ↓
Multi-Round Debate
      ↓
Scoring & Analysis Engine
      ↓
┌──────────────────────────────────┐
│ Output + PDF + History Storage   │
└──────────────────────────────────┘
```

### Agent Design

Each agent is initialized with:
- **Name & Role:** Professional identity
- **Expertise Area:** Specialized knowledge domain
- **Stance:** Perspective on issues (cautious/optimistic/balanced)
- **Argument Generator:** GPT-2 based text generation with custom prompting

### Debate Flow

1. **Topic Selection:** User inputs debate topic
2. **Round Configuration:** User selects number of rounds (1-4)
3. **Sequential Arguments:** Agents present arguments in order
4. **Context Awareness:** Each agent considers previous arguments
5. **Scoring Mechanism:** Arguments evaluated on length and quality keywords
6. **Final Analysis:** Comprehensive summary with rankings and insights

### Scoring Algorithm
```python
score = Base_Score + Quality_Bonus

Base_Score = len(argument.split())  # Word count

quality_keywords = ['evidence', 'research', 'data', 'study', 
                   'however', 'therefore', 'because', 'consider']

Quality_Bonus = sum(2 for keyword in quality_keywords 
                   if keyword in argument.lower())
```

---

## 🎨 Advanced Features

### 1. Custom Agent Creation
Create domain-specific agents for specialized debates:
- Healthcare debates with medical professionals
- Financial discussions with economists
- Technical debates with engineers

### 2. Debate History System
- Automatic JSON-based storage
- Retrieve past debates by ID
- Statistics tracking (total debates, win rates)
- Pattern analysis capabilities

### 3. PDF Export Functionality
- Professional formatting with ReportLab
- Includes all debate rounds
- Participant information
- Scoring and rankings
- Timestamped reports

### 4. Context-Aware Responses
Agents consider:
- Previous round arguments
- Opponent positions
- Conversation history (last 300 characters)

---

## 💼 Use Cases

### Educational
- **Critical Thinking:** Teach students to analyze multiple perspectives
- **Debate Practice:** Prepare for competitions
- **AI Education:** Demonstrate multi-agent systems and NLP

### Business
- **Strategy Discussions:** Explore different business approaches
- **Risk Assessment:** Analyze decisions from multiple angles
- **Decision Support:** Get comprehensive viewpoint analysis

### Research
- **Multi-Agent Systems:** Study agent coordination and behavior
- **Argumentation Patterns:** Analyze debate structures
- **LLM Capabilities:** Test language model performance in structured tasks

### Content Creation
- **Balanced Articles:** Generate multi-perspective content
- **Brainstorming:** Explore topics from all sides
- **Script Writing:** Create dialogue for debates/discussions

---

## 📸 Screenshots

*Add screenshots of your application here:*

1. **Main Interface** - Debate configuration screen
2. **Debate in Progress** - Real-time argument generation
3. **Final Analysis** - Scores and rankings
4. **Custom Agents** - Agent personality configuration
5. **Debate History** - Past debates view

---

## 🔮 Future Enhancements

### Planned Features
- [ ] Integration with advanced LLMs (Llama 3, Mistral)
- [ ] Vote counting and audience interaction
- [ ] Debate summary generation using abstractive summarization
- [ ] Support for more than 3 agents
- [ ] Topic-specific agent expertise customization
- [ ] Debate history comparison features
- [ ] Real-time sentiment analysis of arguments
- [ ] Multi-language support
- [ ] Visual debate flow diagrams

### Advanced Improvements
- [ ] Reinforcement Learning for argument quality improvement
- [ ] Fact-checking integration with external knowledge bases
- [ ] Agent personality customization by users
- [ ] Debate tournament mode with multiple topics

---

## 📊 Project Highlights

### Innovation
✅ Multi-agent orchestration without paid APIs  
✅ Automated argument evaluation system  
✅ Context-aware debate progression  
✅ Real-time scoring and analytics  
✅ Custom agent personality system

### Technical Excellence
✅ Modular and scalable architecture  
✅ Efficient prompt engineering  
✅ Clean code with proper documentation  
✅ User-friendly interface design  
✅ Production-ready deployment

### Practical Application
✅ Addresses real-world decision-making scenarios  
✅ Demonstrates GenAI and Agentic AI concepts  
✅ Showcases AI safety considerations (multiple perspectives)  
✅ Production-ready deployment via Gradio sharing  

---

## ⚠️ Known Limitations

1. **Model Constraints:** GPT-2 generates shorter, less sophisticated arguments compared to larger models
2. **Context Window:** Limited conversation history to prevent token overflow
3. **Scoring Simplicity:** Current scoring is keyword-based; could be enhanced with semantic analysis
4. **Response Time:** Multiple agent generations can take 15-30 seconds per round
5. **Consistency:** Arguments may occasionally lack deep logical connections

*These limitations are acknowledged and provide opportunities for future improvements.*

---

## 📚 Learning Outcomes

### AI/ML Concepts Demonstrated
✅ Natural Language Processing (NLP)  
✅ Text Generation with Transformers  
✅ Multi-agent systems and coordination  
✅ Prompt engineering techniques  
✅ Generative AI applications  
✅ Agentic AI behavior modeling  

### Technical Skills Applied
✅ Python programming  
✅ Hugging Face Transformers library  
✅ Gradio UI development  
✅ System architecture design  
✅ Model deployment and sharing  
✅ Git/GitHub version control

---

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch:**
```bash
git checkout -b feature/AmazingFeature
```

3. **Commit your changes:**
```bash
git commit -m 'Add some AmazingFeature'
```

4. **Push to the branch:**
```bash
git push origin feature/AmazingFeature
```

5. **Open a Pull Request**

---

## 📄 License

This project is created for educational purposes as part of Wipro AI Track Training.

---

## 👤 Author

**[Your Name]**  
Wipro AI Track Training Participant  
February 2026

### Connect with Me
- 📧 Email: [your.email@example.com]
- 💼 LinkedIn: [Your LinkedIn Profile]
- 🐙 GitHub: [@Swastikraj599](https://github.com/Swastikraj599)
- 🌐 Portfolio: [Your Portfolio URL]

---

## 🙏 Acknowledgments

- **Wipro AI Track Training** - For providing comprehensive AI/ML education
- **Hugging Face** - For open-source transformers and models
- **Gradio Team** - For the excellent UI framework
- **OpenAI** - For inspiration from multi-agent systems research

---

## 📞 Contact & Support

For questions, suggestions, or support:

- 📧 Email: [your.email@example.com]
- 💼 LinkedIn: [Your LinkedIn]
- 🐙 GitHub Issues: [Create an issue](https://github.com/Swastikraj599/Multi-Agent-Debate-System/issues)

---

## ⭐ If you found this project helpful, please consider giving it a star!

**Last Updated:** March 2026

---

**Built with ❤️ using Python, Transformers, and Gradio**
