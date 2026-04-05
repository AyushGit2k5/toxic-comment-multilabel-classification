# Toxic Comment Multi-Label Classification (NLP)

## Problem
Developed a multi-label text classification system to detect multiple forms of toxicity in online comments, including toxic, severe toxic, obscene, threat, insult, and identity hate.

## Dataset
Used the Toxic Comment Classification dataset containing user-generated comments annotated with six toxicity labels. Each comment can belong to multiple classes simultaneously, making this a multi-label classification task.

## Approach
- Applied TF-IDF vectorization with a Linear SVM as a baseline model.  
- Implemented a BiLSTM neural network to capture sequential dependencies in text.  
- Fine-tuned a DistilBERT transformer model to leverage contextual embeddings and improve semantic understanding.  
- Performed consistent preprocessing and tokenization across models, with threshold tuning for multi-label prediction.  

## Evaluation
Evaluated models on a held-out test set using precision, recall, and F1-score, with emphasis on macro/micro F1 due to class imbalance and multi-label structure.

## Results
The DistilBERT model achieved the best overall performance, significantly outperforming traditional baselines by capturing context-dependent toxic language and improving F1-score across multiple labels.

## Key Learnings
- Transformer-based models outperform traditional and sequence-based models on complex NLP tasks.  
- Multi-label classification requires careful threshold tuning and evaluation beyond simple accuracy.  

## Future Improvements
- Experiment with larger transformer models (e.g., RoBERTa)  
- Improve handling of class imbalance  
- Deploy as a real-time content moderation system  
