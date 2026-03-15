# 🧠 RAG Knowledge Bot

> Retrieval-Augmented Generation bot that answers questions from your own knowledge base.

## What It Does

Instead of hallucinating answers, this bot retrieves accurate information
directly from your own documents and knowledge base:

1. Receives question via chat trigger
2. AI Agent processes the query
3. Searches Pinecone vector database for relevant context
4. Gemini AI generates accurate answer using retrieved context
5. Sends response via WhatsApp
6. Logs every interaction to Google Sheets for review

## Why RAG?

Standard AI makes up answers. RAG retrieves real information from
your documents first — then generates a response based on actual data.
This means zero hallucination on topics you've trained it on.

## Use Cases

- Customer support bot trained on your FAQ docs
- Internal knowledge base assistant
- Policy and compliance Q&A bot
- Product documentation helper

## Tech Stack

- **n8n** — workflow automation
- **Gemini AI** — language model for response generation
- **Pinecone** — vector database for knowledge storage
- **WhatsApp Business API** — response delivery
- **Google Sheets** — interaction logging
- **Window Buffer Memory** — conversation context retention

## How to Use

1. Import `RAG_Knowledge_Bot.json` into n8n
2. Configure Gemini, Pinecone, WhatsApp and Google Sheets credentials
3. Set your Pinecone index name in the vector store node
4. Upload your knowledge base documents to Pinecone
5. Activate the workflow and start asking questions

## Part of Spectre Flow Engine

This workflow is part of the [Spectre Flow](https://spectre-flow-website.vercel.app) AI infrastructure stack.

---
Built by [Ayanokouji](https://github.com/Darkus39) · Spectre Flow
