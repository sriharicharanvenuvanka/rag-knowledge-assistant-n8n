# RAG-Powered Knowledge Assistant

## Overview

A document-based question-answering assistant built with n8n. It uses Retrieval-Augmented Generation (RAG) to answer questions using information from an uploaded PDF.

## Problem Statement

A general-purpose language model may not know the contents of a specific document. This project demonstrates how a knowledge assistant can retrieve relevant information from a document and use it to answer user questions.

## Tech Stack

- **Workflow automation:** n8n
- **LLM:** OpenAI (if used in your working workflow)
- **Vector database:** Supabase (if used in your working workflow)
- **Knowledge source:** PDF document
- **Technique:** Retrieval-Augmented Generation (RAG)

## How It Works

1. A PDF provides the knowledge source.
2. The document is processed into smaller text chunks.
3. The chunks are converted into embeddings and stored in a vector database.
4. A user's question triggers retrieval of relevant information.
5. The language model uses the retrieved context to generate an answer.

## Current Status

The standalone RAG assistant has been tested with questions about the uploaded PDF.

## Demo

Add screenshots of the n8n workflow and an example question with its answer here.

## Limitations

This repository documents the standalone RAG assistant. Integration with a live telephone voice agent is a separate development task.

## Future Improvements

- Integrate with a voice agent.
- Add error handling and evaluation tests.
- Improve source-grounded answers and handling of questions outside the knowledge base.

## Setup

Import the exported n8n workflow into an n8n instance, configure the required credentials and connect your own knowledge document.

Do not include API keys or exported credentials in this repository.
