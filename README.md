# 🎮 AI 3D PyGame Visualizer

Welcome to the **AI 3D PyGame Visualizer**! This project is an advanced autonomous agent system that generates, extracts, and automatically executes interactive PyGame code in the browser. 

By combining the reasoning powers of **DeepSeek R1** with the execution capabilities of **OpenAI GPT-4o** and the **browser-use** library, this application turns your natural language ideas into playable 3D/2D visual simulations entirely on its own.

---

## ✨ Features

- **Prompt-to-Game Creation:** Describe the game or visual physics simulation you want in plain text, and watch it come to life.
- **DeepSeek R1 Reasoning:** Leverages DeepSeek-Reasoner's chain-of-thought to architect robust and error-free PyGame mechanics.
- **GPT-4o Code Extraction:** Ensures the generated code is perfectly parsed and ready for execution.
- **Autonomous Browser Execution:** A multi-agent browser system automatically navigates to an online Python playground (Trinket.io), pastes your code, and runs it—without you lifting a finger!
- **Streamlit Interface:** A clean, easy-to-use web interface for entering API keys and prompts.

## 🚀 Getting Started

### 1. Clone the Repository
```bash
git clone https://github.com/Aditya29-22/ai_3dpygame_r1.git
cd ai_3dpygame_r1
```

### 2. Install Dependencies
Make sure you have Python installed, then run:
```bash
python -m pip install -r requirements.txt
```

### 3. API Keys Required
You will need two API keys to run the application:
1. **DeepSeek API Key** (for generating the PyGame logic)
2. **OpenAI API Key** (for parsing the code and driving the browser automation)

*You can securely enter these keys directly into the app's sidebar once it's running.*

### 4. Run the Application
Launch the Streamlit app:
```bash
python -m streamlit run ai_3dpygame_r1.py
```

## 🧠 How the Multi-Agent Setup Works
1. **The Thinker (DeepSeek R1):** Reads your input and outputs an extensive thought-process mapping out exactly how the PyGame code should be structured.
2. **The Extractor (GPT-4o via Agno):** Takes DeepSeek's raw reasoning output and perfectly extracts just the executable Python code.
3. **The Browser Agents (Browser-Use):**
   - **Navigator Agent:** Opens a browser window and proceeds to Trinket.io.
   - **Coder Agent:** Waits for the environment to load and pastes the extracted Python code.
   - **Executor Agent:** Interacts with the browser UI to hit the "run" button.
   - **Viewer Agent:** Monitors the live PyGame window to ensure successful visual execution.

## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Aditya29-22/ai_3dpygame_r1/issues) for any planned updates or to submit your own.
