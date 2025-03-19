# Sarcasm Detection in Tamil and Malayalam

## 📌 Overview
This project aims to detect sarcasm in Tamil and Malayalam texts using machine learning models. The dataset includes the original texts in Tamil and Malayalam. Various feature extraction techniques (TF-IDF, Word2Vec) and classification models are evaluated. 
This was done as a part of a Shared Task on "Sarcasm Identification of Dravidian Languages" organised by DravidianCodeMix@2024

## 📊 Model Performance and Result
The results show how different models perform with translated and non-translated texts. The best-performing models are:
- **Ensemble Model (TF-IDF)**: Best performance for Malayalam (without Translation).
- **Meta Stacking (TF-IDF)**: Best performance for Tamil (without Translation).

| Model                   | Feature  | Tamil (Without Translation) | Malayalam (Translation) | Malayalam (Without Translation) |
|-------------------------|----------|-----------------------------|--------------------------|---------------------------------|
| **SVM**                | TFIDF    |0.72                    | 0.52                     | 0.67                        |
|                         | Word2Vec | 0.62                        | 0.38                     | 0.49                            |
| **Logistic Regression** | TFIDF    |0.72                   | 0.53                     | 0.67                        |
|                         | Word2Vec |0.63                        | 0.44                     | 0.46                            |
| **KNN**                | TFIDF    | 0.54                        | 0.48                     | 0.60                            |
|                         | Word2Vec |0.60                        | 0.49 (No grid search)    | -                               |
| **Random Forest**      | TFIDF    | 0.69                        | 0.56                     | 0.66                      |
|                         | Word2Vec | 0.64                        | 0.54                     | 0.50                            |
| **Decision Tree**      | TFIDF    | 0.65                        | 0.52                     | 0.62                            |
|                         | Word2Vec |0.59                        | 0.50                     | 0.49                            |
| **Ensemble Model (with all the above 5 models)**     | TFIDF    | 0.72                    | 0.52                     | **0.67**                        |
|                         | Word2Vec | 0.64                        | 0.52                     | 0.49                            |
| **Bootstrap Aggregating** | TFIDF |0.67                        | 0.52                     | 0.64                            |
|                         | Word2Vec | 0.62                        | 0.52                     | 0.54                            |
| **Gradient Boosting**  | TFIDF    |0.64                        | 0.51                     | 0.64                            |
|                         | Word2Vec |0.64                        | 0.51                     | 0.54                            |
| **Meta Stacking**      | TFIDF    | **0.72**                    | 0.61                     | 0.67                        |
|                         | Word2Vec | 0.61                        | 0.47                     | 0.47                            |

## 🏗️ Tech Stack
- **Programming Language**: Python
- **Libraries Used**:
  - Scikit-learn (Machine Learning)
  - NLTK (Text Preprocessing)
  - Pandas, NumPy (Data Processing)
  - Matplotlib (Visualization)

## 🧑‍🤝‍🧑 The Team and Mentor
Team: Rohan R, Thirumurugan RA, Madussree Ravi, Shivaanee SK
Mentor: Dr. Thenmozhi Durairaj., professor at SSN College of Engineering.
