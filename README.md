# GSI-notebooks

Notebooks for RAG using NVIDIA endpoints at build.nvidia.com and Langchain.

RAG-arxiv-example.ipynb shows how to form a simple pipeline of retrieval augmented generation (RAG) using Langchain and three models (embedding / reranking model / LLM), to retrieve information from PDF files such as research papers in Arxiv and answer questions related to the research papers.

MultiQueryRetrieverNVblog.ipynb focuses on multi query retriever, which generate multiple queries based on the original query using LLM, then using each query to retrieve answers. Based on the union of all the answers from html such as NVIDIA developer blogs, a reranking model is used to choose the answer with the highest ranking score.

You don't need to download the models, as the LLM / embedding / reranking models are hosted at NVIDIA endpoints (https://build.nvidia.com/). You need to generate a NVIDIA API key to use the model endpoints.
