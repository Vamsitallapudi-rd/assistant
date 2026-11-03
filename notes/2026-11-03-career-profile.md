# Career profile: Vamsi Tallapudi

Taken from my resume (Nov 2026). Contact details left out on purpose.

## In one line
Applied AI engineer, 4+ years building production GenAI/LLM systems for clinical trials and pharma. Based in Hyderabad.

## Work history
| When | Role | Company | Where |
|---|---|---|---|
| Feb 2026 – now | Software Engineering Expert, Digital R&D | Sanofi | Hyderabad |
| May 2024 – Jan 2026 | Software Engineer 2, DDIT Applied AI | Bristol-Myers Squibb | Hyderabad |
| Jul 2022 – Apr 2024 | Senior Systems Engineer | Cognizant | Bangalore |

### Sanofi (current)
- **Compass:** Python + React platform using clinical/operational data, statistical risk models, explainable site recommendations, and LLM visit prep. Replaces a ~$3.5M/year vendor licence and cuts low-value visits ~30% (~$400K/year).
- **ClinTrialBench:** LLM benchmark for clinical-trial reasoning and regulatory compliance (FDA warning letters, ICH, 21 CFR). Shows the gap between exam-style knowledge and real GxP competence. Under review at EMNLP.
- **Protocol PDF → JSON pipeline:** PDFPlumber → Markdown → Claude, producing visit × assessment matrices. Gemini LLM-as-judge eval over ~30 protocols, ~85% field-level accuracy.
- **Interpretability PoC:** Sparse Autoencoders on GPT-2 and BioGPT.

### Bristol-Myers Squibb
- **GenAI Safety Narrative platform:** LLM + RAG drafts with source citations. Authoring time ~2 hours → ~2 minutes. Aimed at replacing a ~$4–5M/year vendor tool.
- **Clinical data pipeline:** AE, lab, disposition, EDC data → LLM-ready text in S3. 30 lakh+ rows, 50+ studies, ~$300–400K/year savings.
- **Protocol Amendment Analyzer:** 90%+ accuracy, ~60 review hours/week saved.
- **GPS ETL pipelines:** 15+ clinical datasets, 10–15 lakh records per deviation, prep time down to 1–2 minutes.
- **NER/extraction:** replaced John Snow Labs models with Gemini/OpenAI for ICD-10/11, HIPAA, drug codes across 100+ protocols (~$30K/year).
- Data quality for 600+ protocols, 4 Tableau dashboards. Sentiment analysis across 52 countries (NLTK).

### Cognizant
- Cloud data solutions (Python, SQL, Excel, MongoDB), ML for classification, Agile/Waterfall delivery.

## Skills (short)
- **GenAI:** LLMs, RAG, prompt engineering, LangChain, LangGraph, PydanticAI, agents, MCP, tool calling, structured outputs.
- **Inference:** vLLM, batching, KV cache, speculative decoding, quantisation (GPTQ, AWQ, FP8, INT4).
- **Evaluation:** LangSmith, LLM-as-judge, human eval, hallucination detection, benchmarks.
- **Retrieval:** FAISS, Pinecone, hybrid/semantic search, embeddings.
- **NLP/DL:** NER, biomedical NLP, Hugging Face, PyTorch, SAEs.
- **Data:** ETL, Redshift, Impala, PostgreSQL, MySQL, MongoDB, Parquet, Arrow.
- **Cloud:** Azure, GitHub Actions, CI/CD.
- **AI safety:** prompt injection, jailbreak eval, PII detection.
- **Domain:** clinical trial analytics, protocols, safety narratives, regulatory (FDA, ICH, 21 CFR, GxP), medical coding.

## Education
- M.Tech, AI and Data Science, KIET Kakinada (2022–2024)
- B.Tech, EEE, Aditya University, Surampalem (2018–2021)
- Diploma, EEE, APT Anaparthi (2015–2018)
- IBM Data Science and IBM Data Engineering Professional Certificates
