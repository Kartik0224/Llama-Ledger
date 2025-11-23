# local-llms-analyse-finance
In this project, I explored how local LLMs can be used to label data and support analyses. Specifically, I used Llama2 model to automatically categorise my bank transaction data.

## Installing local LLMs with Ollama (currently support MacOS and Linux)
https://ollama.ai/



## Personal finance dashboard:
<img width="1505" alt="Screenshot 2024-02-02 at 12 00 46 AM" src="https://github.com/thu-vu92/local-llms-analyse-finance/assets/22730220/68142afa-58a8-4be9-940e-ede8ffb0da65">

# LocalLLM Finance Analyzer  
### GenAI-Powered Personal Finance Categorization Using Local LLMs

This project demonstrates how **local Large Language Models (LLMs)** can be used to automatically categorize personal banking transactions and generate financial insights. Using **Ollama + Llama2**, the system processes raw transaction descriptions and assigns meaningful categories, followed by interactive financial dashboards built with Plotly.

---

##  Project Overview

The goal of this project was to explore how **local LLMs** can support financial data analysis without relying on cloud APIs.  
Key capabilities:

- Use **Llama2 (local model)** to classify transaction descriptions into categories such as groceries, entertainment, utilities, etc.  
- Automate label generation by batching 30 transactions at a time to stay within token limits.  
- Validate model outputs using Pydantic to ensure clean, structured results.  
- Build a fully interactive finance dashboard showcasing income/expense insights for different years.

---

##  Tech Stack

- **Local LLMs:** Llama2 via Ollama  
- **Python Libraries:**  
  - LangChain  
  - Pandas  
  - Plotly Express  
  - Panel  
  - Pydantic  
- **Tools:**  
  - VS Code  
  - Jupyter Notebook  

---

##  Features

- **Local LLM Classification:**  
  Automatically categorizes 300+ bank transactions using Llama2 running on-device.

- **Custom Model File:**  
  Built a custom "expense analyzer" model with tailored system prompts and temperature tuning.

- **Batch Processing Engine:**  
  Processes long datasets by splitting inputs into optimal batches (30 items per prompt).

- **Validation Pipeline:**  
  Ensures every LLM output matches the required format using regex + Pydantic validation.

- **Interactive Dashboard:**  
  Visualizes:  
  - Yearly income breakdown  
  - Yearly expense breakdown  
  - Monthly savings trends  

---

