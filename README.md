# YouTube Video Q&A

A simple RAG-based project that lets you ask questions about a YouTube video using its transcript.

The project extracts the video transcript, splits it into chunks, creates embeddings, and stores them in a FAISS index. When a question is asked, it retrieves the most relevant parts of the transcript and uses an LLM to generate an answer based on that context.

## Features

* Extract transcripts from YouTube videos
* Generate a summary of the video
* Ask questions about the video content
* Retrieve relevant context using semantic search
* Show timestamps with the generated answers

## Tech Stack

* Python
* Hugging Face Transformers
* Sentence Transformers
* FAISS
* YouTube Transcript API
* PyTorch

## Models

* `microsoft/Phi-4-mini-instruct`
* `sentence-transformers/all-MiniLM-L6-v2`
* `facebook/bart-large-cnn`

## How It Works

YouTube Video → Transcript → Text Chunks → Embeddings → FAISS → Relevant Context → LLM → Answer

## Notes

The video needs to have an available English transcript. A GPU is recommended for faster inference.
