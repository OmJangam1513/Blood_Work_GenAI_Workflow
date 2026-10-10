# 🩸 Blood Work Analyzer – GenAI Workflow

A Python-based application built with **Streamlit, LangChain, and Groq LLMs** that helps users understand their blood test reports through simple explanations, identification of abnormal values, and practical dietary suggestions.

## 🚀 Features

- **Blood Report Analysis:** Helps interpret blood test results in an easy-to-understand format.
- **Abnormal Value Identification:** Highlights test values that may be outside the provided reference ranges.
- **AI-Generated Summaries:** Converts medical terminology into simpler explanations.
- **Diet Recommendations:** Generates practical diet suggestions based on the provided report and user context.
- **Interactive Interface:** Provides a user-friendly interface through Streamlit.
- **GenAI Integration:** Uses LangChain to interact with language models through the Groq API.

## 🛠️ Technologies Used

- **Python** – Core programming language
- **Streamlit** – Web application interface
- **LangChain** – LLM integration and workflow development
- **Groq API** – Language model inference
- **python-dotenv** – Environment variable management
- **uv** – Python dependency and project management

## 📁 Project Structure

```text
Blood_Work_GenAI_Workflow/
├── 2_health_analysis/
│   └── streamlit_app/
│       └── app.py
├── .env.example
├── .gitignore
├── pyproject.toml
├── uv.lock
└── README.md
```

*Note: Update the structure above if your actual project contains additional files or folders.*

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/OmJangam1513/Blood_Work_GenAI_Workflow.git
cd Blood_Work_GenAI_Workflow
```

### 2. Install uv

If `uv` is not installed, follow the instructions at [Astral uv](https://docs.astral.sh/uv/getting-started/installation/).

### 3. Install dependencies

```bash
uv sync
```

### 4. Configure environment variables

Create a `.env` file in the project root and add your Groq API key:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Obtain an API key from the [Groq Console](https://console.groq.com/).

**Security note:** Never upload your `.env` file or API keys to GitHub. Keep `.env` in `.gitignore`. Commit `.env.example` with placeholder values instead.

### 5. Run the application

```bash
uv run streamlit run 2_health_analysis/streamlit_app/app.py
```

Streamlit will provide a local URL, usually:

```text
http://localhost:8501
```

Open it in your browser to use the application.

## 🔄 How It Works

1. The user provides blood test information or a supported report.
2. The application processes the available test data.
3. The LangChain workflow sends the relevant information to the configured Groq language model.
4. The model generates explanations and identifies potentially abnormal values based on the available information.
5. The application presents the results and dietary suggestions through the Streamlit interface.

*The exact workflow depends on the features implemented in the current version of the application.*

## 🔮 Future Enhancements

- Support for uploading PDF blood reports and extracting test values automatically.
- Reference-range validation for different age groups and other relevant factors.
- Visual charts for tracking blood test results over time.
- Personalized dietary recommendations with additional user context.
- Downloadable analysis reports.
- Integration with structured medical reference data to improve reliability.

## ⚠️ Disclaimer

This application is intended for **educational and informational purposes only**. It does not provide a medical diagnosis and should not replace consultation with a qualified healthcare professional. AI-generated interpretations and dietary suggestions may be inaccurate. Always consult a healthcare professional before making medical or dietary decisions based on blood test results.

## 👨‍💻 Author

**Om Jangam**

- GitHub: [@OmJangam1513](https://github.com/OmJangam1513)

---

⭐ If you find this project useful, consider giving the repository a star.
