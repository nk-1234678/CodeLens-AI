# CodeLens AI 🔍

## 🌐 Live Demo

🚀 **Try CodeLens AI:** [Try Here](https://codelens-review.streamlit.app) 

**AI-Powered Code Review & Explanation Assistant**

CodeLens AI is an intelligent code analysis application powered by Google's Gemini API. It helps developers identify potential code issues, improve code quality, and understand unfamiliar programs through AI-generated explanations.

The application supports multiple programming languages and provides two main functionalities: Code Review and Code Explanation.

## ✨ Features

### 1. AI Code Review
- Identifies potential bugs, syntax issues, and risky coding patterns.
- Highlights readability and maintainability concerns.
- Provides practical improvement suggestions.
- Assigns an overall code quality level: Low, Medium, or High.
- Generates structured JSON review results.

### 2. AI Code Explanation
- Explains the overall purpose of the code.
- Describes important functions, variables, and components.
- Provides a step-by-step execution flow.
- Offers line-by-line explanations.
- Explains expected inputs, outputs, dependencies, and limitations.

### 3. Multiple Input Options
- Paste source code directly into the application.
- Upload source-code files for analysis.
- Supports file uploads up to 1 MB.
- Limits code input to 50,000 characters.

### 4. Safety & Validation
- Submitted code is analyzed as text and is never executed.
- Validates uploaded file size and UTF-8 encoding.
- Treats submitted code as untrusted input.
- Handles API errors and empty AI responses.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python | Core application logic |
| Streamlit | Interactive web interface |
| Google Gemini API | AI-powered code analysis |
| Pydantic | Structured response validation |
| Python-dotenv | Environment variable management |

## 🧠 How It Works

1. The user selects either Code Review or Code Explanation.
2. The user selects a programming language.
3. Source code is pasted or uploaded.
4. The application sends the code and relevant instructions to Gemini.
5. Gemini analyzes the submitted code.
6. The application displays the generated review or explanation.

**Code Review Workflow:**

`Source Code → Gemini API → Structured JSON → Review Results`

**Code Explanation Workflow:**

`Source Code → Line Numbering → Gemini API → Detailed Explanation`

## 📂 Project Structure

```text
CodeLens-AI/
│
├── app.py
├── review_engine.py
├── schemas.py
├── requirements.txt
├── .env
├── .gitignore
└── README.md
```

## ⚙️ Installation & Setup

### Prerequisites
- Python 3.10 or above
- Google Gemini API key
- Git

### 1. Clone the Repository

```bash
git clone https://github.com/nk-1234678/codelens-ai.git
```

### 2. Navigate to the Project

```bash
cd codelens-ai
```

### 3. Create a Virtual Environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure the API Key

Create a `.env` file in the project root:

```env
GEMINI_API_KEY=your_gemini_api_key
```

Get your API key from [Google AI Studio](https://aistudio.google.com/).

### 6. Run the Application

```bash
streamlit run app.py
```

The application will open in your browser.

## 🔐 Environment Variables

| Variable | Description |
|---|---|
| `GEMINI_API_KEY` | Google Gemini API key |

**Important:** Never commit your `.env` file or expose your API key in a public repository.

## 🌐 Deployment

CodeLens AI can be deployed using [Streamlit Community Cloud](https://share.streamlit.io/).

1. Push the project to GitHub.
2. Connect your GitHub repository to Streamlit Community Cloud.
3. Select `app.py` as the main application file.
4. Add your `GEMINI_API_KEY` in the application's Secrets settings.
5. Deploy the application.

## ⚠️ Limitations

- AI-generated reviews may contain inaccurate or incomplete suggestions.
- The application analyzes submitted code as text; it does not compile or execute programs.
- Review results depend on the quality and context of the submitted code.
- Large code submissions may be limited by model input and output token constraints.
- A valid Gemini API key and available API quota are required.

## 🔮 Future Improvements

- Support for downloadable code review reports.
- More detailed severity classification for identified issues.
- Integration with static code analysis tools.
- Support for additional programming languages.
- Code improvement recommendations with before-and-after examples.

## 👩‍💻 Author

**Neelam Kumari**

B.Tech Computer Science & Engineering



*CodeLens AI — Understand your code. Improve your code. Build better software.*
