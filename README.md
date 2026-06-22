# LLM--Zoomcamp

Create practical LLM applications with search, retrieval, RAG, evaluation, monitoring, and production workflows for AI systems.

This repository contains some of the useful codes/notebooks from the LLM Zoomcamp and some other related online sessions. The idea is to be able to use LLMs and Agents and related production grade evaluation, monitoring etc for agentic applications.

If interested in checking all the codes or openAI equivalent codes, its recommended to check the referenced github link for the course.

## Module 01 - Agentic RAG

Keep llm api keys in .env file as shown in .env.example and make sure .env is added in gitignore. Use below commands to setup the environment:

*Note*: The original codes use openai based gpt models and are available for reference in `original notebooks` folder. I have used groq for the most part and hence working notebooks have codes modified accordingly. The modifications are minimal though and somehting similar can be done to accomodate for local ollama models as well. The price calculations are still on gpt model rates for indicative/learning purpose.

```bash
conda create -n llm_zoomcamp python=3.14
conda activate llm_zoomcamp
pip install requests minsearch sqlitesearch openai jupyter python-dotenv
```


<br><br><br><hr>

Reference Links:
- Course Homepage: https://datatalks.club/docs/courses/llm-zoomcamp/
- Course Material: https://github.com/DataTalksClub/llm-zoomcamp
- Youtube Playlist: https://www.youtube.com/playlist?list=PL3MmuxUbc_hLZFNgSad56pDBKK8KO0XIv
