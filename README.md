# OccultumAI
GenAI project using Retrieval-Augmented Generation (RAG) with Large Language Models

OccultumAI
OccultumAI is a fantasy-themed Retrieval-Augmented Generation assistant that behaves like a wizard’s spellbook.
It retrieves knowledge from a text-based grimoire and uses a LLM to generate grounded, explainable answers(while keeping everything framed a mystical tone).

Knowledge Base (The Grimoire)
It is a collection of plain text files that contain factual explanations about topics such as dark stars, black holes, and quantum physics.
They are embedded and stored in a vector database for semantic search.

Working
1.Text files are split into small chunks.
2.chunk is converted into an embedding.
3.Embeddings are stored in a vector database (Chroma in this case).
4.User queries are embedded and matched against stored spells.
5.Relevant spells(i.e. data) are retrieved and passed to an LLM.
6.The LLM generates an answer.

The wizard-like personality comes from prompt design, while factual accuracy comes from retrieval.

Tech Stack:
Python
sentence-transformers (MiniLM)
ChromaDB
GPT-4
Gradio (UI)

A magical theme built on serious GenAI architecture
