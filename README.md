# Toxic Comment Multi-Label Classification

## Problem
Built a multi-label text classification system to automatically detect different forms of toxicity in online comments, including toxic, severe toxic, obscene, threat, insult, and identity hate content.

## Dataset
Toxic Comment Classification dataset consisting of user-generated text comments annotated with six toxicity-related labels, where each comment may belong to multiple classes simultaneously.

## Approach
Implemented and compared multiple models for multi-label classification, including a TF-IDF + Linear SVM baseline, a BiLSTM neural network, and a DistilBERT transformer model to capture contextual semantic information.

## Evaluation
Evaluated models using F1-score, precision, and recall on a held-out test set, with per-label threshold tuning to improve multi-label prediction performance.

## Results
The DistilBERT-based model significantly outperformed traditional baselines, achieving the strongest overall F1-score by effectively capturing context-dependent toxic language patterns.

## Future Improvements
Potential improvements include experimenting with larger transformer models, addressing class imbalance more explicitly, and deploying the model as an automated content moderation system.
