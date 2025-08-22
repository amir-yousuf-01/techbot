TechPro FAQ Chatbot – Project Description and Summary
Description
This project is a simple, end-to-end FAQ chatbot built in a Jupyter notebook that answers common questions about a fictional product called TechPro. It demonstrates a classic TF-IDF + machine learning approach for matching user queries to the closest known question and returning its predefined answer.

The workflow:

Data: A small in-notebook dataset of common Q&A pairs about TechPro (e.g., pricing, password reset, mobile apps, integrations).

Text Features: Converts questions into numeric features using TF-IDF (TfidfVectorizer).

Model: Trains a RandomForestClassifier to predict the most similar known question given a user’s query vector.

Inference: Maps the predicted question back to its corresponding answer and returns it to the user.

CLI Loop: A simple input loop to chat with the bot directly in the console.

This template is useful for beginners to learn how to:

Represent text data with TF-IDF

Train a basic classifier for intent/question matching

Build a minimal retrieval-style FAQ assistant without deep learning

Run an interactive chatbot loop in Python

Summary
Purpose: Provide instant answers to common TechPro FAQs using a lightweight ML pipeline.

Tech Stack: Python, pandas, scikit-learn (TF-IDF + RandomForest), Jupyter.

Data Schema: Two columns — “Question” and “Answer”; all data defined inline.

Pipeline:

Vectorize known questions with TF-IDF

Train RandomForest on question texts to classify incoming queries as one of the known questions

On user input, transform with the same vectorizer, predict the closest known question, and return its mapped answer
