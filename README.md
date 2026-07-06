# IE7500
Applied Natural Language Processing

1. Research and Selection of Methods
Define Objectives: In this project we will be developing a NLP that will summarize scientific papers using a pretrained FLAN-T5 transformer. The goal will be to generate concise, interpretable, and custom summaries from research papers while preserving the key takeaways.
Literature Review: Review recent research on transformer-based summarization models such as T5, BART, and FLAN-T5 to identify the most effective approach.
Benchmarking: This project will move forward with FLAN-T5 due to its strong summarization performance while not requiring extensive training. 
Preliminary Experiments: We will be conducting small-scale experiements using a subset of the SciTDLR dataset to verify data preprocessing, tokenization, model compatability, and baseline summarization performance.
3. Model Implementation
Framework Selection: Implement the project using Python, Hugging Face Transformers, PyTorch, Pandas, NumPy, and Scikit-learn. These libraries provide efficient tools for preprocessing, model training, and evaluation.
Dataset Preparation: Load the SciTLDR training, validation, and test datasets from JSONL files. Perform exploratory data analysis, clean the text, remove incomplete records, tokenize the documents, and prepare the inputs for sequence-to-sequence training.
Model Development: Implement the pretrained FLAN-T5 model using a modular workflow that separates data loading, preprocessing, training, inference, and evaluation into reusable notebook sections.
Training & Fine-Tuning: Fine-tune the pretrained FLAN-T5 model using the SciTLDR training dataset by optimizing hyperparameters such as learning rate, batch size, maximum sequence length, and number of training epochs.
Evaluation & Metrics: We will be evaluating th emodel using various ROUGE scores to measure summary quality. Validation loss and inference examples will also be reviewed to assess model performance and identify opportunities for improvement.
