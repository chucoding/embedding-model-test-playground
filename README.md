# 🛝 embedding-model-test-playground
![embedding-model-test-playground](https://github.com/user-attachments/assets/33f04a5f-b7c6-4222-9453-714f3a44f355)

## Overview
This project is a playground for testing and comparing different embedding models using LangChain. It provides an environment to experiment with vector databases and embedding models.

## Features
- **Multiple Embedding Model Support**
  - Clova AI Embedding Model
    - Model: `bge-m3`
    - Provider: Naver Clova Studio
  - OpenAI Embedding Model
    - Model: `text-embedding-3-large`
    - Provider: OpenAI

- **Vector Search Capabilities**
  - Similarity-based Search
    - Cosine similarity-based ranking
    - Similarity score display
  - MMR-based Search (Maximal Marginal Relevance)
    - Balance between diversity and relevance
    - Avoid redundant results
  - Metadata Filtering
    - Python function-based filtering
    - Dynamic filter conditions
  - Top-K Search (Default: Top-3)

- **Document Management**
  - Document Addition/Deletion
  - Metadata Management
    - Dynamic metadata field addition/removal
    - Key-value pair based metadata
  - In-memory Vector Store

- **User-Friendly Interface**
  - Streamlit-based intuitive UI
  - Real-time search results display
  - Document and metadata visualization

## Getting Started
### Server (Docker)
```bash
# Run Docker container
docker-compose up -d --build
```

### Local Development
```bash
# Run Streamlit server
streamlit run server.py
```

## Requirements
- Python 3.8 or higher
- Docker & Docker Compose
- OpenAI API Key
- Naver Clova Studio API Key

## Configuration
Create `.env` file from `.env.sample`:
```bash
# Copy .env.sample to .env
cp .env.sample .env
```

Then, edit the `.env` file and set your API keys:
- `OPENAI_API_KEY`: Your OpenAI API key
- `NCP_CLOVASTUDIO_API_KEY`: Your Naver Clova Studio API key

## License
This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).