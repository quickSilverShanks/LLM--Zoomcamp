# LLM--Zoomcamp

Create practical LLM applications with search, retrieval, RAG, evaluation, monitoring, and production workflows for AI systems.

This repository contains some of the useful codes/notebooks from the LLM Zoomcamp and some other related online sessions. The idea is to be able to use LLMs and Agents and related production grade evaluation, monitoring etc for agentic applications.

If interested in checking all the codes or openAI equivalent codes, its recommended to check the referenced github link for the course.

## Module 01 - Agentic RAG

- Build a RAG pipeline with keyword search
- Make it agentic with function calling

Keep llm api keys in .env file as shown in .env.example and make sure .env is added in gitignore. Use below commands to setup the environment:

*Note*: The original codes use openai based gpt models and are available for reference in `original notebooks` folder. I have used groq for the most part and hence working notebooks have codes modified accordingly. The modifications are minimal though and something similar can be done to accommodate for local ollama models as well. The price calculations are still on gpt model rates for indicative/learning purpose.

```bash
conda create -n llm_zoomcamp python=3.14
conda activate llm_zoomcamp
pip install requests minsearch sqlitesearch openai jupyter python-dotenv toyaikit gitsource
```

Assignment has its own readme file with instructions.

## Module 02 - Vector Search

- Semantic search with embeddings
- minsearch, sqlitesearch, and PGVector

Keep llm api keys in .env file as shown in .env.example and make sure .env is added in gitignore. Use below commands to setup the environment:

```bash
conda activate llm_zoomcamp
pip install sentence-transformers psycopg[binary]
```

PGVector requires Docker, Postgres database with concurrent access, can handle millions of records and is best for production systems as compared to other alternatives used in this module. Pull the image specified below and start postgres with pgvector:

```bash
docker run -it \
    --name pgvector \
    -e POSTGRES_USER=user \
    -e POSTGRES_PASSWORD=pswd \
    -e POSTGRES_DB=faq \
    -v pgvector_data:/var/lib/postgresql/data \
    -p 5432:5432 \
    pgvector/pgvector:pg17
```

Assignment has its own readme file with instructions.

<br><br><br><hr>

Reference Links:
- Course Homepage: https://datatalks.club/docs/courses/llm-zoomcamp/
- Course Material: https://github.com/DataTalksClub/llm-zoomcamp
- Youtube Playlist: https://www.youtube.com/playlist?list=PL3MmuxUbc_hLZFNgSad56pDBKK8KO0XIv
