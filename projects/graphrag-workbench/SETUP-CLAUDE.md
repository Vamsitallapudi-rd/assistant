# Running this workbench with Claude (Anthropic) — no Ollama needed

Changes vs upstream:
- **Extraction / summaries:** Claude via the Anthropic API (default `claude-sonnet-5-5`).
- **Embeddings:** local Hugging Face model `BAAI/bge-base-en-v1.5` (768-dim, CPU, ONNX via fastembed).
  Served by `scripts/embed_server.py` on 127.0.0.1:11435 (OpenAI-compatible). The build starts it
  automatically; the model downloads once (~220 MB) into `.graphrag/hf-models`.

## Setup (on your machine)
1. Install Node 20.9+, pnpm, Python 3.12 and uv.
2. `pnpm install && uv sync --frozen`
3. `pnpm dev`, then open http://127.0.0.1:3000
4. Projects → Build providers → Cloud tab → paste your Anthropic key (or `export ANTHROPIC_API_KEY=...` before `pnpm dev`)
5. Name the project, add a text-backed PDF, click **Run with Claude**.

## Notes
- Other 768-dim models also work without changing the vector size, e.g. `nomic-ai/nomic-embed-text-v1.5`.
  If you pick a model with a different size, also change `CLOUD_DEFAULTS.embeddingVectorSize` in `lib/server/providerConfig.ts`.
- If you change the embedding model, stop the old server first: `pkill -f embed_server.py`.
- Embedding server logs: `logs/embed-server.log`.
- The "Run with Ollama" button still exists but needs Ollama; ignore it.
