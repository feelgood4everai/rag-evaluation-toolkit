# RAG Evaluation Toolkit

Evaluate RAG (Retrieval-Augmented Generation) pipelines with production-ready metrics. Stop guessing if your RAG system works—measure it.

## Why This Exists

After deploying 5 RAG systems for enterprise clients, I kept hitting the same problems:
- Silent failures in production
- Costs spiraling unexpectedly  
- Quality degrading over time
- Debugging taking hours instead of minutes

This toolkit gives you visibility into what's actually happening in your RAG pipeline.

## What It Measures

- **Retrieval accuracy** — Is your system finding the right context?
- **Answer relevance** — Are responses actually useful?
- **Latency & cost** — Track performance per query
- **Drift detection** — Catch when quality degrades

## Quick Start

```bash
pip install -r requirements.txt
python app.py
```

Then open `http://localhost:7860` in your browser.

## Usage

1. **Upload your documents** — PDF, TXT, or paste text directly
2. **Configure your retriever** — Choose embedding model, chunk size, overlap
3. **Add test questions** — Ground truth pairs or let it auto-generate
4. **Run evaluation** — Get metrics on accuracy, latency, cost
5. **Iterate** — Adjust parameters and compare runs

## Live Demo

[Try it on Hugging Face](https://huggingface.co/spaces/AnandGeetha/rag-evaluation-toolkit)

## Tech Stack

- Python 3.11+
- Gradio for UI
- OpenAI/Anthropic APIs for LLM evaluation
- Sentence transformers for embeddings

## License

MIT — Use it, modify it, deploy it.

---

*Built by [Anand](https://github.com/feelgood4everai) after one too many 2am production incidents.*
