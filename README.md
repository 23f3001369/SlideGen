# SlideGen – Auto-Generate Presentations from Text

Turn bulk text or Markdown into a fully formatted PowerPoint that **matches your chosen template’s look & feel**. Bring your own LLM API key (OpenAI, Anthropic, Gemini, etc.).  
⚡ **No AI image generation** — the app **reuses images** found in the uploaded template/presentation.

---

## ✨ Features
- Paste long text/Markdown + optional one-line guidance (e.g., *“investor pitch deck”*).  
- Upload a `.pptx` or `.potx` template — styles, colors, fonts, and layouts are respected via placeholders.  
- BYO LLM API key: works with OpenAI / Anthropic / Gemini (keys are not stored or logged).  
- Intelligent slide splitting & bulleting via LLM with structured JSON output.  
- Reuse any images discovered in the uploaded template/presentation (tastefully placed).  
- Download a brand new `.pptx` generated from your template.  

---

## 🛠️ Tech Stack
- **Backend:** Python (FastAPI) + `python-pptx`  
- **Frontend:** Plain HTML / CSS / JavaScript  
- **Providers:** OpenAI, Anthropic, Gemini (easily extendable to others)  

---

## 🚀 Run Locally
```bash
python -m venv .venv && source .venv/bin/activate   # Windows: .venv\Scripts\activate
pip install -r requirements.txt
uvicorn app:app --reload
# open http://localhost:8000
