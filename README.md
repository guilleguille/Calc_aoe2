# Calc_aoe2 - ChatGPT Code Generator Integration

Welcome to Calc_aoe2! This repository is integrated with ChatGPT to generate code directly into your project.

## 🚀 Getting Started

### 1. Set Up Your OpenAI API Key

1. Get your API key from [OpenAI Platform](https://platform.openai.com/api-keys)
2. Copy `.env.example` to `.env`:
   ```bash
   cp .env.example .env
   ```
3. Add your API key to `.env`:
   ```
   OPENAI_API_KEY=sk-your-key-here
   ```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Generate Code with ChatGPT

Use the `generate_code.py` script to create code:

```bash
# Generate and display code
python generate_code.py "Create a function to calculate unit armor bonuses in Age of Empires 2"

# Generate and save to a file
python generate_code.py "Create a function to calculate unit armor bonuses" src/armor_calculator.py

# Generate JavaScript code
python generate_code.py "Create a React component for unit selection" src/UnitSelector.jsx javascript

# Generate Java code
python generate_code.py "Create a class for managing unit statistics" src/UnitStats.java java
```

## 📋 Usage Examples

### Python Code Generation
```bash
python generate_code.py "Create a class to manage AOE2 civilization bonuses" src/civilization.py
```

### JavaScript/React Code Generation
```bash
python generate_code.py "Create a React hook for managing selected units" src/useUnitSelection.js javascript
```

### Save Generated Code Directly
The script will automatically:
- Create directories if they don't exist
- Format the code properly
- Add documentation and comments
- Save it to the specified file

## 🔧 How It Works

1. You provide a prompt describing what code you want
2. ChatGPT generates well-documented, production-ready code
3. The code is automatically saved to your repository
4. You can review, edit, and commit the generated code

## 💡 Tips

- Be specific in your prompts for better results
- Specify the file path to automatically organize your code
- Mention the programming language for best results
- Generated code includes docstrings and comments

## ⚠️ Important

- Never commit `.env` file with your API key
- Keep your `OPENAI_API_KEY` secure and private
- Review generated code before committing to ensure quality

## 📝 License

(Add your license here)
