# Running this workbench with Claude (Anthropic)

Changes vs upstream: the "cloud" preset now uses Claude for extraction. Embeddings stay on local Ollama (Anthropic has no embedding API).

## One-time setup (on your own machine)
1. Install Ollama: https://ollama.com/download, then `ollama pull embeddinggemma`
2. `pnpm install && uv sync --frozen`
3. `pnpm dev` and open http://127.0.0.1:3000
4. Projects → Build providers → Cloud tab → paste your Anthropic key (or export ANTHROPIC_API_KEY before `pnpm dev`)
5. Add a text-backed PDF → "Run with Claude"

Model default: `claude-sonnet-5-5` (editable in the Cloud tab).
