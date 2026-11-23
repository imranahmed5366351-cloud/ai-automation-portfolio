# Trading Knowledge Base RAG Assistant

## Overview
I built an AI-powered Trading Knowledge Base using n8n, Pinecone, and OpenAI. The system uses Retrieval-Augmented Generation (RAG) to process trading knowledge documents and answer user questions using relevant retrieved information.

## Problem
Finding specific information in trading learning materials can be time-consuming. This project helps users retrieve relevant information from a knowledge base and receive AI-generated answers.

## Tools Used
- n8n
- Pinecone Vector Database
- OpenAI Embeddings
- GPT-4.1-mini
- Google Drive
- Gmail
- Webhook
- Retrieval-Augmented Generation (RAG)

## How It Works

### Workflow 1: Knowledge Base Ingestion
1. Downloads a Trading Basics PDF from Google Drive.
2. Extracts text from the PDF.
3. Converts the extracted text into vector embeddings using OpenAI.
4. Stores the embeddings in Pinecone.

### Workflow 2: RAG Query Handler
1. Receives a user's question through a webhook.
2. Searches Pinecone for relevant information.
3. Retrieves matching context from the knowledge base.
4. Uses GPT-4.1-mini to generate an answer.
5. Sends the generated answer to the user through Gmail.

## What I Learned
- Building a RAG architecture with n8n
- Working with vector databases and embeddings
- Connecting OpenAI with Pinecone
- Processing PDF documents
- Building webhook-based AI workflows
- Automating email responses with Gmail

## Project Status
Personal learning project. The workflows demonstrate document ingestion, semantic search, and AI-powered question answering.
## Workflow Screenshots

### 1. Knowledge Base Ingestion
![Knowledge Base Ingestion](rag-knowledge-base-ingestion.png)

### 2. RAG Query Handler
![RAG Query Handler](rag-query-handler.png)

## Workflow JSON Files

- [Download Knowledge Base Ingestion Workflow](RAG_Knowledge_Base_Ingestion_Sanitized.json)
- [Download RAG Query Handler Workflow](RAG_Query_Handler_Sanitized.json)
