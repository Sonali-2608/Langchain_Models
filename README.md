# LangChain Models

A small repository demonstrating how to work with LangChain-style model wrappers and embeddings for OpenAI, Anthropic, and Hugging Face services.

## Project Structure

- `1.LLMs/`
  - `llm.py` — core logic for interacting with large language models.

- `2.ChatModels/`
  - `1.Chatmodel_openAI.py` — chat model integration for OpenAI.
  - `2.Chatmodel_anthropic.py` — chat model integration for Anthropic.
  - `3.chatmodel_hf_api.py` — chat interaction through Hugging Face API.
  - `4.chatmodel_hf_local.py` — local Hugging Face chat model support.

- `3.Embedded_Models/`
  - `1.embedding_openai_query.py` — OpenAI embedding for query data.
  - `2.embeddings_openai_docs.py` — OpenAI embeddings for document processing.
  - `3.embeddings_hf_local.py` — local Hugging Face embeddings.
  - `4.document_similarity.py` — document similarity and retrieval logic.

## Requirements

Dependencies are listed in `requirements.txt`. Core packages include:

- `langchain`
- `openai`
- `anthropic`
- `transformers`
- `huggingface-hub`
- `sentence-transformers`
- `python-dotenv`
- `numpy`
- `scikit-learn`

## Setup

1. Create and activate a Python virtual environment:

```powershell
python -m venv venv
venv\Scripts\Activate.ps1
```

2. Install dependencies:

```powershell
pip install -r requirements.txt
```

3. Create a `.env` file with your API keys and configuration. Example:

```env
OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
HF_API_TOKEN=your_huggingface_api_token
```

## Usage

- Use `1.LLMs/llm.py` to run general LLM workflows.
- Use `2.ChatModels/` scripts to experiment with chat model integrations from OpenAI, Anthropic, and Hugging Face.
- Use `3.Embedded_Models/` scripts to generate embeddings and perform document similarity searches.

> Note: Each script may require custom configuration or environment variables depending on the provider.

## Notes

- This repository is intended as a learning and experimentation workspace for LangChain-style model wrappers.
- Review each script to understand required input formats and environment setup.
- Keep API keys secure and do not commit `.env` to source control.

## License

This repository does not include a license file. Add one if you plan to publish or share publicly.
