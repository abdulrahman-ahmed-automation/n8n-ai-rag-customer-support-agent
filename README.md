# n8n AI Customer Support Agent (RAG + Google Drive)

This workflow connects a Google Drive folder to an n8n AI Agent so users can ask questions directly about uploaded files and product catalogs.

## Demo


https://github.com/user-attachments/assets/759cf16d-f376-435e-adb5-7ebce7197834



## How it works

1. **Data Sync:** Whenever a new file (CSV, PDF, or text) is uploaded to a specific Google Drive folder, n8n downloads it, splits the text into chunks, and saves the OpenAI embeddings into a vector store.
2. **Chat & Retrieval:** When a user sends a message, the AI Agent searches the stored files, keeps track of the conversation memory, and answers based strictly on the file data.

## Tech Stack

- n8n
- OpenAI API (Chat Model & Embeddings)
- Google Drive API

## How to use

1. Download `AI RAG Customer Support Agent (Google Drive to Chat).json` from this repository.
2. Import the workflow into your n8n workspace.
3. Connect your Google Drive and OpenAI credentials, pick your folder, and activate it.
  
