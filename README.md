# RAG Automation Workflow

A full Retrieval-Augmented Generation (RAG) pipeline that enables 
businesses to query their documents using natural language. 
Built with n8n, Qdrant, and OpenAI.

## Demo

[

![Watch the demo]
https://img.youtube.com/vi/h10HkO8-b8w/0.jpg

]https://www.youtube.com/watch?v=h10HkO8-b8w

## How It Works

1. **Webhook** receives incoming customer messages via HTTP POST
2. **AI Agent** processes the query using OpenAI Chat Model
3. **Qdrant Vector Store** searches the knowledge base using embeddings
4. **Cohere Reranker** reranks results for accuracy
5. **HTTP Request** forwards the response to the target endpoint
6. **Respond to Webhook** sends the final AI reply back to the user

## Tools Used

- n8n
- OpenAI (Chat Model + Embeddings)
- Qdrant Vector Store
- Cohere Reranker
- Webhook + HTTP Request
