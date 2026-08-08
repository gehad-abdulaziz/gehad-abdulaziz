<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6B46C1,100:0EA5E9&height=220&section=header&text=Gehad%20Abdulaziz&fontSize=52&fontColor=ffffff&fontAlignY=38&desc=NLP%20%26%20LLM%20Engineer%20%7C%20Building%20Trustworthy%20Generative%20AI&descAlignY=58&descSize=18&animation=fadeIn" width="100%"/>

<a href="https://linkedin.com/in/gehad-abdulaziz-228973287"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:gehadabdelaziz179@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>
<a href="https://www.kaggle.com/gehadabdulaziz"><img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white"/></a>
<img src="https://komarev.com/ghpvc/?username=gehad-abdulaziz&style=for-the-badge&color=6B46C1&label=PROFILE+VIEWS"/>

</div>

<br>

```py
class NLPEngineer:
    def __init__(self):
        self.name        = "Gehad Abdulaziz Ibrahim"
        self.role         = "NLP Engineer · LLM & Generative AI"
        self.base         = "Giza, Egypt 🇪🇬"
        self.education    = "B.Sc. Computer Science (AI Track) — Helwan University, GPA 3.84"
        self.focus        = ["Confidence-Aware RAG", "Multi-Agent Systems", "Speech Intelligence"]
        self.currently_at = "DEPI — Agentic AI & GenAI System Developer Trainee"

    def philosophy(self):
        return "I don't just build models that answer — I build systems that know when NOT to."

me = NLPEngineer()
```

<br>

## 🧠 About Me

I'm an **AI & NLP Engineer** who builds production-minded systems on top of Large Language Models — not just prompt wrappers, but pipelines that reason about their own confidence before they speak.

- 🔭 Currently engineering **AraCheck**, a bilingual medical RAG assistant with a tiered LLM → RAG → Web-Search escalation pipeline that only reaches for more evidence when it's genuinely unsure
- 🎙️ Building **clinical speech intelligence** — ASR + zero-shot NER pipelines that transcribe *and* understand medical audio
- 🧩 Fascinated by **multi-task learning** — training one shared encoder to handle four different language-understanding problems at once
- 🌱 Deep in an **Agentic AI & GenAI System Developer** track at DEPI — LangGraph, multi-agent orchestration, deployment & monitoring
- 🗣️ Native Arabic speaker building **Arabic-first NLP** — because most of the field forgets my language exists
- 💬 Ask me about: RAG architecture, confidence calibration, transformer internals, or why your chatbot is hallucinating

---

## 🛠️ Tech Stack

<div align="center">

**LLMs & Agentic AI**
<br>
<img src="https://img.shields.io/badge/LangGraph-1C3C3C?style=for-the-badge&logo=langchain&logoColor=white"/>
<img src="https://img.shields.io/badge/Hugging%20Face-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/Qdrant-DC244C?style=for-the-badge&logo=qdrant&logoColor=white"/>
<img src="https://img.shields.io/badge/Groq-F55036?style=for-the-badge&logo=groq&logoColor=white"/>
<img src="https://img.shields.io/badge/LoRA%2FQLoRA-7C3AED?style=for-the-badge"/>

**Deep Learning & NLP**
<br>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
<img src="https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white"/>
<img src="https://img.shields.io/badge/spaCy-09A3D5?style=for-the-badge&logo=spacy&logoColor=white"/>
<img src="https://img.shields.io/badge/Transformers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
<img src="https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white"/>

**Speech & Multimodal**
<br>
<img src="https://img.shields.io/badge/Whisper-412991?style=for-the-badge&logo=openai&logoColor=white"/>
<img src="https://img.shields.io/badge/OCR-4B5563?style=for-the-badge"/>
<img src="https://img.shields.io/badge/Vision--Language%20Models-4B5563?style=for-the-badge"/>

**Serving & Tooling**
<br>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
<img src="https://img.shields.io/badge/Streamlit-FF4B4B?style=for-the-badge&logo=streamlit&logoColor=white"/>
<img src="https://img.shields.io/badge/Gradio-F97316?style=for-the-badge&logo=gradio&logoColor=white"/>
<img src="https://img.shields.io/badge/MLflow-0194E2?style=for-the-badge&logo=mlflow&logoColor=white"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
<img src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white"/>

</div>

---

## 🚀 Featured Work

### 🩺 AraCheck — Bilingual Medical RAG Assistant
**Confidence-aware retrieval so the model knows when to look further before it answers**

An agentic pipeline (LangGraph) that escalates a medical query through LLM → RAG → web-search — only climbing tiers when confidence is genuinely low, cutting down on hallucinated answers. Built the retrieval core: `BAAI/bge-m3` embeddings, Qdrant vector search, cross-encoder reranking, and a **margin-based confidence score** instead of a fixed similarity cutoff. Helped fold voice (Whisper) and image understanding (VLM) into one chat pipeline with numbered source citations.

`Python` `FastAPI` `LangGraph` `Qdrant` `Hugging Face` `Groq API` `Next.js`

---

### 🎙️ Medical ASR v6 — Multi-Specialty Clinical Speech Recognition
**Transcription that understands what it just heard**

End-to-end pipeline pairing `faster-whisper large-v3` with **zero-shot NER (GLiNER)** to pull 9 clinical entity types with no task-specific retraining. Auto-detects the medical specialty from the audio to route it to specialty-aware prompts, and grades every transcript A–D on ASR/NER confidence for clinical review. Shipped as a Streamlit app with live recording, file upload, and confidence-highlighted text.

`Python` `faster-whisper` `GLiNER` `Hugging Face` `Streamlit`

---

### 🔗 Multi-Task BiRNN — One Encoder, Four GLUE Tasks
**73.45% accuracy sharing a single brain across sentiment, paraphrase, duplicate-detection & NLI**

A shared bidirectional RNN with an ESIM-style soft-alignment (attention) layer, trained jointly across SST-2, MRPC, QQP, and MNLI. Got there through staged improvements — added capacity, soft alignment, more data — and stabilized training with label smoothing, gradient clipping, and stochastic weight averaging. Packaged as a live Gradio demo.

`PyTorch` `GloVe` `Gradio`

---

### 🔍 Food Reviews Semantic Search Engine
**Search by meaning, not keywords — over 3,000 Amazon food reviews**

Led a 6-member team and owned the data pipeline for a semantic search engine, then benchmarked a TF-IDF/cosine baseline against Sentence-Transformer embeddings using Precision@5.

`Python` `scikit-learn` `Sentence-Transformers`

<div align="center">

[![More Projects](https://img.shields.io/badge/See_all_repositories-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/gehad-abdulaziz?tab=repositories)

</div>

---

## 🎓 Path So Far

```text
2023 ─── B.Sc. Computer Science (AI Track) begins @ Helwan University
2025 ─── Data Science Trainee @ DEPI — Python, ML, MLOps foundations
2025 ─── Machine Learning — DEY Upskilling Programs
2026 ─── Deep Learning for Computer Vision — DEY Upskilling Programs
2026 ─── NLP 90-Hour Track @ NTI — Transformers built from scratch, Arabic NLP
2026 ─── AI & Data Science Trainee — Agentic AI & GenAI System Developer @ DEPI  ← now
2027 ─── Graduating — focus: NLP & LLMs
```

**Currently building:** Confidence-aware agentic RAG · Multi-agent orchestration with LangGraph · Production LLM deployment & monitoring

---

## 📊 GitHub Stats

<div align="center">
<img height="165" src="https://github-readme-stats.vercel.app/api?username=gehad-abdulaziz&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&title_color=A78BFA&icon_color=38BDF8"/>
<img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=gehad-abdulaziz&layout=compact&theme=tokyonight&hide_border=true&title_color=A78BFA&langs_count=8"/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=gehad-abdulaziz&theme=tokyonight&hide_border=true&ring=38BDF8&fire=A78BFA"/>

</div>

---

## 🌐 Let's Talk NLP

<div align="center">

I'm always up for collaborating on RAG systems, agentic pipelines, or Arabic NLP — reach out.

<a href="https://linkedin.com/in/gehad-abdulaziz-228973287"><img src="https://img.shields.io/badge/Connect_on_LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white"/></a>
<a href="mailto:gehadabdelaziz179@gmail.com"><img src="https://img.shields.io/badge/Send_an_Email-D14836?style=for-the-badge&logo=gmail&logoColor=white"/></a>

<br><br>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0EA5E9,100:6B46C1&height=100&section=footer" width="100%"/>

</div>
