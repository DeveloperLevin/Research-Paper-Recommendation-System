# Research Paper Recommendation System

This project is a **BERT model based recommendation system** designed to help users discover relevant academic research papers based on their search queries. It leverages **BERT embeddings** to capture the semantic meaning of the queries and research paper abstracts, enabling accurate and efficient recommendations.

## Features

- **User Query Search**: Enter a query (keywords or phrases) to receive a ranked list of relevant research papers.
- **BERT Embeddings**: Utilizes pre-trained **BERT** (Bidirectional Encoder Representations from Transformers) to create vector embeddings for both user queries and research paper abstracts.
- **Cosine Similarity**: Compares the query embeddings with paper embeddings using cosine similarity to recommend papers most relevant to the query.
- **Fine-tuning**: The BERT model is fine-tuned on a custom dataset of research paper abstracts to improve recommendation accuracy.
- **Flask Backend**: A Flask API serves the model and handles requests from the frontend.
- **React Frontend**: The user interface is built with **React** using **Vite** for fast, modern web development.

## Tech Stack

### Backend

- **Flask**: A lightweight Python framework for creating the API to handle requests and serve recommendations.
- **BERT**: The NLP model used to create meaningful embeddings from text data (using Hugging Face).
- **PyTorch**: For fine-tuning the BERT model on a custom dataset.

### Frontend

- **React**: A JavaScript library for building user interfaces.
- **Vite**: A build tool that provides a fast development environment.
- **Axios**: For making API requests from the frontend to the backend.

## How It Works

1. **Query Input**: The user enters a search query, which can be keywords or phrases related to research topics.
2. **Text Embedding**: The system tokenizes the query and converts it into an embedding using the fine-tuned BERT model.
3. **Similarity Calculation**: The cosine similarity is calculated between the query embedding and the embeddings of research paper abstracts in the database.
4. **Recommendation**: The system returns a ranked list of relevant papers based on the similarity scores.

## Conclusion

The Research Paper Recommendation System provides a user-friendly interface for academics and researchers to easily find relevant papers, enhancing their research experience.
