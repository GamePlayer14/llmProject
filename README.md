# LLM Project

## Project Task  
Sentiment analysis on IMDb movie reviews. The objective was to classify reviews as either positive or negative using a pre-trained language model.

## Dataset  
IMDb Large Movie Review Dataset — a well-known benchmark dataset for binary sentiment classification. It contains 50,000 labeled reviews (25,000 for training and 25,000 for testing), evenly split between positive and negative.

Dataset source: https://ai.stanford.edu/~amaas/data/sentiment/

## Pre-trained Model  
Used `bert-base-uncased` from Hugging Face. It is a general-purpose transformer model pre-trained on a large corpus of English data. For this task, it was fine-tuned using `AutoModelForSequenceClassification` from the `transformers` library.

## Performance Metrics  
- Metric used: Accuracy  
- Final validation accuracy: ~91.6%  
- The model demonstrated strong performance on this binary classification task with minimal overfitting after two training epochs.

## Hyperparameters  
- Learning rate: 5e-5  
- Batch size: 16  
- Epochs: 2  
- Optimizer: AdamW  

AdamW was chosen for its effectiveness in training transformer models. The learning rate and epoch count were selected to balance performance and training time without overfitting.

## Relevant Links  
- Model on Hugging Face: https://huggingface.co/Tylerus/bert-imdb-sentiment  
- Dataset: https://ai.stanford.edu/~amaas/data/sentiment/



