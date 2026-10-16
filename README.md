# NewsBot Intelligence System

**Course:** ITAI 2373 – Natural Language Processing  
**Project:** Midterm Project  
**Student:** Patrick  
**Platform:** Google Colab / Python

## Project Overview

The NewsBot Intelligence System is a Natural Language Processing (NLP) project designed to automatically analyze and organize news articles.

The system uses different NLP techniques to clean text, identify important words, classify news articles, analyze sentiment, and extract useful information such as people, organizations, locations, and dates.

The goal of this project is to demonstrate how NLP techniques from Modules 1–8 can work together to solve real-world problems.

## Dataset

I used the BBC News Classification dataset from Kaggle.

- **Original articles:** 1,490
- **Articles after cleaning:** 1,440
- **Categories:** Business, Entertainment, Politics, Sport, and Technology
- **Language:** English

Dataset source: https://www.kaggle.com/competitions/learn-ai-bbc/data

The dataset was used to train and test the news classification models.

## NLP Techniques Used

The project includes the following techniques:

1. **Text Preprocessing:** Cleaning text, removing stop words, and lemmatization.
2. **TF-IDF:** Identifying important words and converting text into numerical features.
3. **Part-of-Speech Tagging:** Identifying nouns, verbs, adjectives, and grammatical patterns.
4. **Dependency Parsing:** Analyzing relationships between words in sentences.
5. **Sentiment Analysis:** Identifying positive, negative, and neutral sentiment using VADER.
6. **Text Classification:** Training machine learning models to categorize articles.
7. **Named Entity Recognition:** Extracting people, organizations, locations, dates, and money amounts.
8. **System Integration:** Combining these techniques into one NewsBot system.

## Machine Learning Results

I compared three classification models:

| Model | Test Accuracy |
|---|---|
| Naive Bayes | 93.75% |
| Logistic Regression | 93.06% |
| Support Vector Machine (SVM) | 75.00% |

Naive Bayes performed the best and was selected for the NewsBot system.

## NewsBot Testing Results

I tested the completed system using three example articles.

| Test Article | Predicted Category | Confidence |
|---|---|---|
| Microsoft AI Acquisition | Technology | 41.41% |
| Lakers Championship | Sport | 80.30% |
| Climate Change Report | Business | 36.28% |

All three articles were processed successfully.

The climate change article received low classification confidence, showing that the system may have difficulty with topics that do not clearly fit into the available categories.

## Tools and Libraries

- Python
- Google Colab
- pandas and NumPy
- scikit-learn
- spaCy
- NLTK
- Matplotlib
- TF-IDF Vectorizer
- VADER Sentiment Analyzer

## Project Files

**Midterm_NewsBot_Intelligence_System.ipynb**  
The main Jupyter notebook containing the code, analyses, visualizations, machine learning models, and NewsBot testing.

**BBC_News_Train[1].csv**  
The news dataset used for the project.

**README.md**  
Project overview, methods, results, and instructions.

## How to Run the Project

1. Download or open the Jupyter notebook in Google Colab.
2. Upload the BBC News CSV dataset to the Colab session.
3. Install any required Python libraries using the installation cells in the notebook.
4. Run the notebook cells in order.
5. Review the results, charts, and model evaluations.
6. Run the NewsBot testing section to see how it analyzes new articles.

Make sure the CSV filename in the notebook matches the uploaded dataset.

## Business Applications

NewsBot could be useful for:

- **Media companies:** Automatically organizing news articles.
- **Market research:** Analyzing news sentiment and identifying trends.
- **Content management:** Making articles easier to organize and search.
- **Business intelligence:** Identifying companies, people, and events mentioned in news articles.

## Challenges and Limitations

One challenge was combining different NLP techniques into a single working system. I also experienced errors when the machine learning model received incorrect input features.

The testing results showed that the system can make mistakes when articles do not clearly belong to one category. Sentiment analysis and entity recognition can also produce incorrect results.

These limitations show why testing and human review are important.

## Individual Contributions

I completed the project independently, including:

- Preparing and cleaning the dataset.
- Implementing the NLP techniques.
- Training and comparing classification models.
- Analyzing and visualizing the results.
- Integrating the NewsBot system.
- Testing the system with new articles.
- Reviewing the code and documenting the project.

## Future Improvements

In the future, I would like to improve the system by:

- Adding more news categories.
- Testing with more articles.
- Improving classification accuracy for uncertain predictions.
- Exploring advanced language models such as BERT.
- Creating an interactive dashboard.

## Conclusion

This project helped me understand how different NLP techniques can work together to analyze news articles.

The best classification model achieved 93.75% test accuracy, and the NewsBot system successfully processed three new articles.

The project also helped me practice Python programming, machine learning, data analysis, and problem-solving.
