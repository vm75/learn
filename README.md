# Python, Vibe Coding & AI Development Setup Guide

Welcome to your journey into Python programming, vibe coding, and AI development! This guide will walk you through setting up your development environment on Windows.

## Table of Contents
1. [Create GitHub Account](#1-create-github-account)
2. [Install Essential Tools](#2-install-essential-tools)
3. [Install Python 3.12 with pyenv](#3-install-python-312-with-pyenv)
4. [Setup VS Code Extensions](#4-setup-vs-code-extensions)
5. [Login to GitHub Copilot](#5-login-to-github-copilot)
6. [Create New Repository](#6-create-new-repository)
7. [Try Vibe Coding with Copilot](#7-try-vibe-coding-with-copilot)

---

## 1. Create GitHub Account

1. Go to [GitHub.com](https://github.com)
2. Click **"Sign up"** in the top right corner
3. Fill out the registration form:
   - Choose a unique username
   - Use a valid email address
   - Create a strong password
4. Verify your email address
5. Complete any additional setup steps

> **💡 Tip**: Choose a professional username as it will be part of your developer identity!

---

## 2. Install Essential Tools

### A. Install Git

#### Option 1: Download from Official Website
1. Go to [git-scm.com](https://git-scm.com)
2. Click **"Download for Windows"**
3. Run the installer with default settings
4. Verify installation by opening Command Prompt and typing:
   ```cmd
   git --version
   ```

#### Option 2: Using Winget (Windows Package Manager)
```cmd
winget install Git.Git
```

### B. Install VS Code

#### Option 1: Download from Official Website
1. Go to [code.visualstudio.com](https://code.visualstudio.com)
2. Click **"Download for Windows"**
3. Run the installer
4. During installation, check these options:
   - ✅ Add "Open with Code" action to Windows Explorer file context menu
   - ✅ Add "Open with Code" action to Windows Explorer directory context menu
   - ✅ Register Code as an editor for supported file types
   - ✅ Add to PATH

#### Option 2: Using Winget
```cmd
winget install Microsoft.VisualStudioCode
```

### C. Install pyenv-win

pyenv allows you to manage multiple Python versions easily.

1. Open PowerShell as Administrator
2. Run the following commands:
   ```powershell
   Set-ExecutionPolicy Unrestricted -Force
   Invoke-WebRequest -UseBasicParsing -Uri "https://raw.githubusercontent.com/pyenv-win/pyenv-win/master/pyenv-win/install-pyenv-win.ps1" -OutFile "./install-pyenv-win.ps1"; &"./install-pyenv-win.ps1"
   ```

---

## 3. Install Python 3.12 with pyenv

2. **Install Python 3.12:**
   ```cmd
   pyenv install 3.12
   ```

3. **Set Python 3.12 as global default:**
   ```cmd
   pyenv global 3.12
   ```

---

## 4. Setup VS Code Extensions

### Essential Extensions for Python & AI Development

1. **Open VS Code**
2. Click on the Extensions icon (or press `Ctrl+Shift+X`)
3. Install these extensions:

#### A. GitHub Copilot
- Search for "GitHub Copilot"
- Install **GitHub Copilot** by GitHub
- Install **GitHub Copilot Chat** by GitHub

#### B. Python Development
- Search for "Python"
- Install **Python** by Microsoft
- Install **Pylance** by Microsoft (usually comes with Python extension)

---

## 5. Create New Repository

### Option 1: Using VS Code (Recommended)

1. **Open VS Code**
2. **Open Command Palette** (`Ctrl+Shift+P`)
3. **Type:** `Git: Clone`
4. **Select:** "Clone from GitHub"
5. **Create new repository:**
   - Click "Create repository..."
   - Enter repository name (e.g., "my-python-ai-journey")
   - Choose public or private
   - Select local folder to clone to

### Option 2: Using GitHub Website + VS Code

1. **Go to GitHub.com**
2. **Click the "+" icon** → "New repository"
3. **Fill out the form:**
   - Repository name: `my-python-ai-journey`
   - Description: "Learning Python, vibe coding, and AI development"
   - ✅ Public (or Private if preferred)
   - ✅ Add a README file
   - ✅ Add .gitignore (choose Python template)
   - ✅ Choose a license (MIT is popular for learning projects)

4. **Clone to local machine:**
   ```cmd
   git clone https://github.com/YOUR_USERNAME/my-python-ai-journey.git
   cd my-python-ai-journey
   code .
   ```

---

## 6. Try Vibe Coding with Copilot

### What is Vibe Coding?
Vibe coding is a collaborative approach where you describe what you want to build in natural language, and AI tools like GitHub Copilot help generate the code. It's about maintaining the flow and creativity while AI handles boilerplate and implementation details.

### Let's Create Your First Python Project!

1. **Create a new Python file:** `hello_ai.py`

2. **Start with a comment describing what you want:**
   ```python
   # Create a simple Python program that greets the user and demonstrates basic AI concepts
   ```

3. **Let Copilot suggest code:** Press `Tab` to accept suggestions

4. **Try these vibe coding examples:**

#### Example 1: Interactive Greeting
```python
# Create a function that asks for user's name and gives personalized greeting
# with some fun facts about their name length
```

#### Example 2: Simple Data Analysis
```python
# Create a program that analyzes a list of numbers and provides insights
# like average, maximum, minimum, and finds patterns
```

#### Example 3: AI-Inspired Quote Generator
```python
# Build a random motivational quote generator for programmers
# with different categories like debugging, learning, and creativity
```

### Copilot Chat Tips

1. **Open Copilot Chat:** `Ctrl+Shift+I`
2. **Ask questions like:**
   - "How do I create a virtual environment?"
   - "Explain this Python code"
   - "Help me debug this function"
   - "Suggest improvements for this code"

### Best Practices for Vibe Coding

1. **Write descriptive comments** before coding
2. **Use meaningful variable names**
3. **Ask Copilot to explain complex code**
4. **Iterate and refine** with Copilot's help
5. **Don't accept everything** - review and understand suggestions
6. **Learn from the suggestions** - ask "why" questions

---

## Quick Start Checklist

- [ ] GitHub account created
- [ ] Git installed and configured
- [ ] VS Code installed with extensions
- [ ] pyenv-win installed and configured
- [ ] Python 3.12 installed via pyenv
- [ ] GitHub Copilot logged in and active
- [ ] New repository created
- [ ] First Python file created with Copilot assistance

---

## Troubleshooting

### Common Issues

**Git not recognized:**
- Restart your terminal after installation
- Check if Git is in your PATH environment variable

**pyenv commands not working:**
- Ensure environment variables are set correctly
- Restart your terminal or computer
- Try running as administrator

**Copilot not working:**
- Check your GitHub Copilot subscription status
- Ensure you're logged into the correct GitHub account
- Try signing out and signing back in

**Python version issues:**
- Run `pyenv rehash` after installing new Python versions
- Check `pyenv versions` to see installed versions
- Use `pyenv global 3.12.0` to set the default version

---

## Next Steps

Once you have everything set up:

1. **Learn Python basics** with Copilot assistance
2. **Explore AI/ML libraries** like pandas, numpy, scikit-learn
3. **Build projects** that interest you
4. **Join the community** - share your learning journey!

## Resources

- [Python Official Documentation](https://docs.python.org/3/)
- [GitHub Copilot Documentation](https://docs.github.com/en/copilot)
- [VS Code Python Tutorial](https://code.visualstudio.com/docs/python/python-tutorial)
- [Real Python](https://realpython.com/) - Excellent Python tutorials

---

**Happy Coding! 🚀🐍✨**

Remember: The best way to learn is by doing. Start small, be curious, and let Copilot be your coding companion on this exciting journey!
