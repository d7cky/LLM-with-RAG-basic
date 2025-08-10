# LLM with RAG basic

![n8n.io - Screenshot](https://raw.githubusercontent.com/n8n-io/self-hosted-ai-starter-kit/main/assets/n8n-demo.gif)

### What’s included

✅ [**Self-hosted n8n**](https://n8n.io/) - Low-code platform with over 400
integrations and advanced AI components

✅ [**Ollama**](https://ollama.com/) - Cross-platform LLM platform to install
and run the latest local LLMs

✅ [**Open WebUI**](https://openwebui.com/) - ChatGPT-like interface to
privately interact with your local models and N8N agents

✅ [**Supabase**](https://supabase.com/) - Open-source, high performance vector
store with an comprehensive API

## Installation

```
git clone https://github.com/d7cky/LLM-with-RAG-basic.git
cd LLM-with-RAG-basic
docker compose up
```

> [!NOTE]
> You must install Ollama on your mac

After you followed the quick start set-up below, change the Ollama credentials
by using `http://host.docker.internal:11434/` as the host.

## ⚡️ Quick start and usage

1. Open <http://localhost:5678/> in your browser to set up n8n. You’ll only
   have to do this once. You are NOT creating an account with n8n in the setup here,
   it is only a local account for your instance!
2. Open the included workflow:
   <http://localhost:5678/workflow/vTN9y2dLXqTiDfPT>
3. Create credentials for every service:
   
   Ollama URL: http://ollama:11434

   Qdrant URL: http://qdrant:6333 (API key can be whatever since this is running locally)

   Google Drive: Follow [this guide from n8n](https://docs.n8n.io/integrations/builtin/credentials/google/).
   Don't use localhost for the redirect URI, just use another domain you have, it will still work!
   Alternatively, you can set up [local file triggers](https://docs.n8n.io/integrations/builtin/core-nodes/n8n-nodes-base.localfiletrigger/).
4. Select **Test workflow** to start running the workflow.
5. If this is the first time you’re running the workflow, you may need to wait
   until Ollama finishes downloading Llama3.1.

To open n8n at any time, visit <http://localhost:5678/> in your browser.
To open Open WebUI at any time, visit <http://localhost:3000/>.

With your n8n instance, you’ll have access to over 400 integrations and a
suite of basic and advanced AI nodes such as
[AI Agent](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.agent/),
[Text classifier](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.text-classifier/),
and [Information Extractor](https://docs.n8n.io/integrations/builtin/cluster-nodes/root-nodes/n8n-nodes-langchain.information-extractor/)
nodes. To keep everything local, just remember to use the Ollama node for your
language model and Supabase as your vector store.

## 📜 Acknowledgments

This project uses code from [Repository Name](https://github.com/tuyenhm68/self-hosted-ai-starter-kit-2) by [the n8n team]. Special thanks for providing such a great open-source resource!
