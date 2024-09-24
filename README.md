# Scientific-RAG-Gemini
An end-to-end RAG system using Gemini and Langchain catered to research based usage. A web app using Streamlit, hosted using Ngrok/localtunnel. LlamaParse (using GPT model) to parse research documents with much higher quality, and also Pinecone with LlamaIndex for cloud based vector database and retrieval (AWS).

### Gemini_RAG_for_Scientific_Papers

In this notebook, we setup a RAG for scientific papers. The Gemini LLM (LMM) is used since it has a free tier that is ideal for application development. The prompt-to-answer pipeline is constructed using LangChain due to its flexibility. We also use LlamaParse (the gpt4o version) to convert pdf files into text. We use this perticular pdf parser due to equations and other complex structures in scientific papers. Regular pdf readers such as pypdf aren't able to properly process the documents resulting in poor performancing RAGs. Chroma vector store is paired with this LlamaIndex library to create the index.

Note: For more basic information on RAG please check out my [RAG-HF-Langchain](https://github.com/AarifCha/RAG-HF-Langchain) github.
