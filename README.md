# 🎬 Movie Review Sentiment Analysis

*(Placeholder: You can design a cool 1280x640px tech banner in Canva/Figma and drag-and-drop the image here later!)*

## 📌 Project Overview
A complete machine learning pipeline designed to automatically classify movie reviews as positive or negative. This project utilizes Natural Language Processing (NLP) techniques and a tuned probabilistic classifier to extract emotional tone from raw text data.

**🎯 Final Model Accuracy:** 83.41%

## 🛠️ Tech Stack & Methodology
* **Language:** Python
* **Libraries:** Scikit-learn, Pandas, NumPy, Matplotlib, Seaborn
* **Text Vectorization:** TF-IDF (Term Frequency-Inverse Document Frequency). Used to penalize common filler words and highlight unique, sentiment-heavy vocabulary (Restricted to Top 10,000 features using Unigrams & Bigrams).
* **Model:** Multinomial Naive Bayes.
* **Optimization:** Deployed `GridSearchCV` for hyperparameter tuning to find the optimal Laplace smoothing parameter ($\alpha = 0.1$).

## 📊 Results & Performance
The model was trained and evaluated on a strict binary subset of the Kaggle Rotten Tomatoes dataset (76,478 total reviews), achieving highly balanced performance across both classes.

* **Overall Accuracy:** 83.41%
* **F1-Score (Positive):** 0.86
* **F1-Score (Negative):** 0.80

### Confusion Matrix
*(Placeholder: Drag and drop your confusion_matrix.png file right here in the GitHub editor to display it!)*

## 🚀 How to Run Locally

1. **Clone the repository:**
   `git clone https://github.com/NotVr17/movie-review-sentiment-analysis.git`
2. **Install Dependencies:**
   `pip install pandas scikit-learn numpy matplotlib seaborn joblib`
3. **Dataset:** Ensure the `train.tsv` file is in the root directory.
4. **Execute:** Run the `sentiment_model.ipynb` notebook to see the data cleaning, model training, and evaluation process.
