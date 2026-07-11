# IE7500: Applied Natural Language Processing
# Project Overview

In this project, we will be developing a Retrieval-Augmented Generation (RAG) system that retrieves scientific information and rewrites it into three different communication styles: Caveman, Gen-Z, and Conversational. The overall goal is to promote accessibility scientific research by ensuring thorough summarization while still keeping the original meaning and key findings accurate.

Review recent research on Retrieval-Augmented Generation (RAG), semantic search, transformer-based language models, embedding models, and prompt engineering to identify the best approach for retrieving and translating scientific literature.

This project will begin with the BAAI/bge-base-en-v1.5 embedding model because it performs well on semantic retrieval tasks, especially with scientific text. As the project progresses, different chunk sizes, retrieval settings, and embedding models will be compared to see which combination produces the most accurate and relevant results.

We will begin by running small-scale experiments using a subset of the SciTLDR dataset to verify that data preprocessing, document chunking, embedding generation, vector indexing, and semantic retrieval are all working correctly before connecting the language generation component.

After importing necessary libraries such as Python, Pandas, NumPy, Hugging Face Transformers, Sentence Transformers, Scikit-learn, and PyTorch. We can leverage the appropriate tools needed for data preprocessing, embedding generation, semantic retrieval, vector indexing, and response generation.

The SciTLDR training, development, and testing datasets will be loaded from three JSONL files (development, testing, training). The sentence lists will first be combined into complete paragraphs before being cleaned and checked for missing values. Each document will then be divided into overlapping chunks, converted into embeddings, and stored in a searchable vector index for semantic retrieval.

With each stage, there will be an accompanying code. These stages include data preprocessing, document chunking, embedding generation, vector indexing, semantic retrieval, context building, and response generation. Organizing the project this way makes it easier to test, debug, and improve each component individually.

The goal is to have a user submits a scientific question and the system will convert the question into an embedding and compare it against the embedded document chunks using cosine similarity. The most relevant chunks will be combined into a single context and passed to a language model, which will rewrite the scientific information into one of three communication styles. This approach helps keep the generated response grounded in the original scientific literature while making the content easier to understand.

Finally, we will assess how well the system performs when retrieving relevant scientific information and how effectively it rewrites that information for different audiences. Retrieval quality will be reviewed using cosine similarity scores along with manual inspection of the retrieved chunks. The generated responses will then be evaluated based on scientific accuracy, readability, clarity, and consistency across the three communication styles. Additional experiments will compare different chunk sizes, retrieval settings, and embedding models to determine which configuration produces the best overall performance.
