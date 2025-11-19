# Agentic AI Learning

This repository contains projects and exercises for learning Agentic AI with LangChain.

---

## 🚀 Quick Start Guide

### Prerequisites

- Python 3.10 or higher installed
- Google API Key (for Gemini model)

---

## 📋 Setup Instructions

### Step 1: Clone the Repository

```bash
git clone https://github.com/pankajit/Agentic-AI-Learning.git
cd Agentic-AI-Learning
```

---

### Step 2: Create a Virtual Environment

Creating a virtual environment isolates your project dependencies from your system Python installation.

#### **For macOS/Linux:**

```bash
# Create virtual environment
python3 -m venv venv

# Activate virtual environment
source venv/bin/activate
```

#### **For Windows:**

```cmd
# Create virtual environment
python -m venv venv

# Activate virtual environment (Command Prompt)
venv\Scripts\activate

# OR for PowerShell
venv\Scripts\Activate.ps1
```

> **Note:** After activation, you should see `(venv)` at the beginning of your terminal prompt.

---

### Step 3: Install Dependencies

Navigate to the specific project folder (e.g., Day3) and install the required packages:

#### **For macOS/Linux:**

```bash
cd Day3
pip install -r requirements.txt
```

#### **For Windows:**

```cmd
cd Day3
pip install -r requirements.txt
```

---

### Step 4: Create `.env` File

The `.env` file stores your API keys and other sensitive configuration securely.

#### **For macOS/Linux:**

```bash
# Navigate to the project directory (e.g., Day3)
cd Day3

# Create .env file using touch
touch .env

# Open with your preferred editor (nano, vim, or any text editor)
nano .env
```

Then add the following content:

```env
GOOGLE_API_KEY=your_google_api_key_here
```

**Save and exit:**
- In nano: Press `Ctrl + X`, then `Y`, then `Enter`
- In vim: Press `Esc`, type `:wq`, then `Enter`

#### **For Windows:**

```cmd
# Navigate to the project directory (e.g., Day3)
cd Day3

# Create .env file using Command Prompt
type nul > .env

# OR using PowerShell
New-Item .env -ItemType File

# Open with Notepad
notepad .env
```

Then add the following content:

```env
GOOGLE_API_KEY=your_google_api_key_here
```

**Save the file:** Click `File > Save` and close Notepad.

---

### Step 5: Get Your Google API Key

1. Go to [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Sign in with your Google account
3. Click "Create API Key"
4. Copy the generated API key
5. Paste it in your `.env` file (replace `your_google_api_key_here`)

---

### Step 6: Run the Application

#### **For macOS/Linux:**

```bash
# Make sure you're in the project directory with the main Python file
streamlit run resume.py
```

#### **For Windows:**

```cmd
# Make sure you're in the project directory with the main Python file
streamlit run resume.py
```

The application will open in your default browser at `http://localhost:8501`

---

## 🛑 Deactivating Virtual Environment

When you're done working, you can deactivate the virtual environment:

#### **For both macOS/Linux and Windows:**

```bash
deactivate
```

---

## 📂 Project Structure

```plaintext
Agentic-AI-Learning/
├── README.MD
├── Day3/
│   ├── README.md
│   ├── requirements.txt
│   ├── resume.py
│   ├── .env (you create this)
│   ├── chroma_store/
│   └── Resume samples (PDFs)
```

---

## ⚠️ Important Notes

1. **Never commit `.env` file:** The `.env` file contains sensitive information. Make sure it's listed in `.gitignore`
2. **Keep API keys secret:** Never share your API keys publicly or commit them to version control
3. **Virtual environment:** Always activate your virtual environment before working on the project
4. **Dependencies:** If you encounter any package conflicts, try creating a fresh virtual environment

---

## 🐛 Troubleshooting

### Virtual Environment Issues

**macOS/Linux:**
- If `python3` doesn't work, try `python`
- If you get permission errors, ensure you have write access to the directory

**Windows:**
- If PowerShell script execution is disabled, run: `Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`
- If `python` doesn't work, try `py` or `python3`

### Module Not Found Errors

```bash
# Make sure virtual environment is activated (you should see (venv) in prompt)
# Then reinstall requirements
pip install -r requirements.txt
```

### API Key Issues

- Ensure there are no extra spaces or quotes around your API key in `.env`
- Verify your API key is valid at [Google AI Studio](https://makersuite.google.com/app/apikey)

---

## 📚 Resources

- [LangChain Documentation](https://python.langchain.com/)
- [Google Gemini API](https://ai.google.dev/)
- [Streamlit Documentation](https://docs.streamlit.io/)

---

## 👥 Contributing

Feel free to fork this repository and submit pull requests for improvements!

---

## 📝 License

This project is for educational purposes.
