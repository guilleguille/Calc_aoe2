# Calc_aoe2 - ChatGPT Automatic Code Generator

Welcome! This repository is fully integrated with ChatGPT to **automatically generate and commit code** directly to your repo.

## 🚀 Quick Start (No Setup Needed!)

### Method 1: GitHub Web Interface (Easiest) ⭐

1. Go to your repository: https://github.com/guilleguille/Calc_aoe2
2. Click **Actions** tab
3. Click **"Generate Code with ChatGPT"** workflow on the left
4. Click **"Run workflow"** button
5. Fill in:
   - **Prompt**: Describe what code you want (e.g., "Create a function to calculate unit armor bonuses")
   - **Filename**: Where to save (e.g., `src/calculator.py`)
   - **Language**: Select the programming language
6. Click **"Run workflow"**
7. Wait 30-60 seconds ✅
8. **Code is generated AND automatically committed!**

### Method 2: Command Line (Local)

```bash
# First time setup
git clone https://github.com/guilleguille/Calc_aoe2.git
cd Calc_aoe2
cp .env.example .env
# Edit .env and add your OpenAI API key
pip install -r requirements.txt

# Generate and auto-commit code
python auto_generate.py "Create a unit bonus calculator" src/calculator.py python
```

## 📋 Usage Examples

### Via GitHub Actions (Recommended)
1. Go to Actions → "Generate Code with ChatGPT" → Run workflow
2. Input examples:
   - **Prompt**: "Create a class to manage AOE2 civilization bonuses with methods for calculating attack and armor"
   - **Filename**: `src/civilization.py`
   - **Language**: `python`

### Via Command Line
```bash
# Python
python auto_generate.py "Create a damage calculator function" src/damage.py python

# JavaScript
python auto_generate.py "Create a React component for unit stats display" src/UnitStats.jsx javascript

# Java
python auto_generate.py "Create a class for managing resource tracking" src/Resources.java java
```

## 🔐 Security & API Key Setup

### Add Your OpenAI API Key to GitHub Secrets:

1. Go to: **Settings** → **Secrets and variables** → **Actions**
2. Click **"New repository secret"**
3. Name: `OPENAI_API_KEY`
4. Value: Your API key from https://platform.openai.com/api-keys
5. Click **Add secret**

That's it! The workflow will use it automatically.

## ✨ What Happens Automatically

When you trigger code generation:
1. ✅ ChatGPT generates well-documented, production-ready code
2. ✅ Code is automatically saved to your specified file
3. ✅ File is staged and committed to git
4. ✅ Changes are pushed to GitHub
5. ✅ You see the commit in your repository history

**No manual commits needed!**

## 📝 Features

- 🤖 ChatGPT-4 generates clean, documented code
- 📦 Automatic Git commit and push
- 🎯 Multiple language support (Python, JavaScript, Java, C++, Go, Rust, etc.)
- 📂 Automatically creates directories
- 💾 Includes docstrings and comments
- 🔒 Secure API key management

## 🆘 Troubleshooting

**"No changes to commit"** message?
- This means ChatGPT generated the same code or nothing was created
- Check your prompt and try again with more details

**GitHub Actions failing?**
- Go to Actions tab → Click the failed run → See error details
- Make sure `OPENAI_API_KEY` secret is set in Settings

**Want to generate locally instead?**
- Use `python auto_generate.py` command
- Make sure `.env` file has your API key

## 📊 Supported Languages

- Python
- JavaScript / TypeScript
- Java
- C++
- C#
- Go
- Rust
- (and many more!)

## 🎯 Pro Tips

1. **Be specific in your prompts** - "Create a function that calculates unit bonus damage based on civilization and attack type" works better than just "calculator"
2. **Use clear filenames** - `src/unit_calculator.py` is better than `test.py`
3. **Review generated code** - Always check what was created before using it in production
4. **Iterate** - If you want changes, generate again with a new prompt

## 📞 Need Help?

Check the generated code in your commits! Everything is tracked in your Git history.

---

**That's it! You're all set. Start generating code now! 🎉**
