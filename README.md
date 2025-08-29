# Project Overview
This project tackles the challenge of automatically moderating Google Maps reviews by detecting policy-violating content. wo LLMs(Large Language Models), Gemma 3 and Qwen 3, are implemented and evaluated to classify reviews into four categories: genuine feedback, advertisements, irrelevant content, and rant without visit, while running locally on a consumer-grade desktop.

Our results show that Gemma 3 achieved better overall performance, while also being significantly faster than Qwen 3.

# Setup Instructions

### Prerequisites
- **Hardware:** A machine with sufficient RAM (≥16GB recommended). A GPU with ≥8GB VRAM is ideal for accelerated inference.
- **Software:** Python 3.9+, Jupyter, and Ollama installed on your system.

Before running the Jupyter notebook, please ensure you have the required inference services installed and running.

### Clone the Repository and Install Dependencies
```
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
pip install -r requirements.txt
```

### Install Ollama

Ollama is required to run the language models locally.

**Download and install Ollama from the official website:**
[https://ollama.com/download](https://ollama.com/download)

### Install & Run the Models

After installing Ollama, you need to download and run the specific models used in this project (qwen3:8b, gemma3:12b). The notebook will connect to these local models for inference.

Open a terminal (Command Prompt, PowerShell, or shell) and run the following commands (e.g. for qwen3:8b):

`ollama run qwen3:8b`
