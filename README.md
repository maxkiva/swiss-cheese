# 🧀 Swiss Cheese: A GenAI Tax Assistant for Switzerland

**Swiss Cheese** is an intelligent assistant designed to help individuals complete Swiss tax returns and estimate tax liabilities. It supports natural language interaction, reads scanned tax forms like the *Lohnausweis*, and applies rules from the 2024 Zurich tax documents.

## 📁 Repository Contents

- `swiss_cheese_submission_final.ipynb` — Core notebook containing:
  - File upload and processing logic
  - Gemini API integration for extraction and reasoning
  - LangGraph and LangChain-based conversational state handling
  - JSON repair and embedding generation
  - Municipality-level tax rate application from CSV

- `data/` — Example files and official tax documentation:
  - `Lohnausweis_2024_1_fake.png`
  - `STE_ZH_2024.pdf`, `305_Wegleitung_ZH_2024.pdf`, `kantonsteuer_631_1.pdf` (and more)

## 🧠 Technologies Used

This notebook makes use of:

- **Google GenAI SDK**
  - `google.genai`, `google.api_core.retry`, `google.genai.types`
- **LangGraph & LangChain**
  - `StateGraph`, `Chroma`, `GoogleGenerativeAIEmbeddings`
- **Pandas** for structured data handling
- **Pillow (PIL)** for image processing
- **dotenv** for environment variable loading
- **json_repair** for LLM output cleanup
- **IPython.display** for interactive output in the notebook
- **requests** for API interaction

## 🚀 Getting Started

1. Clone this repo:
   ```bash
   git clone https://github.com/your-username/swiss-cheese-tax-assistant.git
   cd swiss-cheese-tax-assistant

  
