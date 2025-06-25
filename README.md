# Langchain Demo With gemma2:2b

<img width="940" alt="ollama screenshot" src="https://github.com/user-attachments/assets/ee3e0163-1e21-46b5-825c-72444248bd88" />

## Overview

This project demonstrates a LangChain-powered application using the Ollama model (gemma2:2b), with inference served through the Groq API. It provides an interactive interface for asking questions and receiving insightful, context-aware answers about data science and related topics.

## Key Features

- **Groq API Integration**: Utilizes the Groq API for fast, scalable inference.
- **Ollama Model (gemma2:2b)**: Leverages state-of-the-art language modeling for high-quality natural language responses.
- **LangChain Framework**: Orchestrates prompt handling, chaining, and response logic for a seamless user experience.
- **Modern UI**: Clean, dark-themed interface suitable for demos and practical use.
- **Data Science Q&A**: Out-of-the-box, the demo explains complex data science topics in clear, concise terms.

## Example Output

> *What is data science?*  
> Data Science is a multifaceted field that uses **scientific methods, processes, algorithms, and systems** to extract knowledge and insights from structured and unstructured data...  
> (See screenshot above for full sample output.)

## How It Works

1. **User Input**: Enter any question (e.g., "What is data science?").
2. **Request Handling**: The LangChain app sends your question to the backend, which then queries the Groq API with the Ollama model.
3. **Model Inference**: The Groq API generates a response using the Ollama large language model.
4. **Display**: The answer is rendered in the app with structured, easy-to-read formatting.

## Setup & Usage

### Prerequisites

- Python 3.8+
- Groq API credentials
- Ollama model access/configuration
- Node.js (if using a JS or React frontend)
- [Optional] Docker for containerized deployment

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/shishiradk/Ollama.git
   cd Ollama
   ```

2. **Install Python dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables:**
   - `GROQ_API_KEY`: Your Groq API key
   - `OLLAMA_MODEL`: (optional) Set to `gemma2:2b` or your preferred model

4. **Start the backend server:**
   ```bash
   python app.py
   ```

5. **[If applicable] Start the frontend:**
   ```bash
   npm install
   npm start
   ```

6. **Open the app:**  
   Visit `http://localhost:3000` in your browser.

## File Structure

- `app.py` or `main.py` – Backend logic for handling API calls and LangChain orchestration.
- `frontend/` – UI code (React or other framework).
- `requirements.txt` – Python dependencies.
- `README.md` – This file.

## Customization

- **Switch Models:** Change the Ollama model by modifying the `OLLAMA_MODEL` environment variable.
- **Expand Prompts:** Update prompt chains in the backend to support more advanced workflows.
- **Styling:** Modify frontend code for different themes or branding.

## Contributing

Pull requests and suggestions are welcome! Please open an issue to discuss major changes first.

## License

[MIT License](LICENSE) (or specify your license here)

---

**Demo Screenshot:**

![LangChain Demo Screenshot](<img width="940" alt="ollama screenshot" src="https://github.com/user-attachments/assets/9e3f755d-c3fb-4a4d-90ab-74563a55faac" />
)

---

*This project uses Groq API and Ollama to showcase the power of modern LLMs for interactive Q&A demos.*
