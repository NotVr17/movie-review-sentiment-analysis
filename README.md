# Movie Review Sentiment Analysis

This project implements a machine learning pipeline to classify movie reviews as either positive or negative. The model utilizes a Multinomial Naive Bayes algorithm combined with TF-IDF vectorization. Hyperparameter tuning was performed using GridSearchCV to achieve an optimal accuracy of 83.41%.

## Package Requirements

The following libraries are required to run this project. 

* pandas
* scikit-learn
* numpy
* matplotlib
* seaborn
* joblib

You can install all dependencies via pip:
`pip install pandas scikit-learn numpy matplotlib seaborn joblib`

## Run Instructions

1.  **Extract the Zip File:** Unzip `Group_71.zip` into your desired working directory.
2.  **Dataset Setup:** Ensure that the Kaggle dataset file named `train.tsv` is placed in the exact same directory as the code file. 
3.  **Execute the Code:** * If using the Python script: Run `python sentiment_model.py` in your terminal.
    * If using Jupyter/Colab: Run all cells in the provided notebook.
4.  **View Results:** The code will automatically load the data, clean the text, train the tuned Naive Bayes model, and output the Accuracy Score (83.41%) and Classification Report.
5.  **Outputs:** The script will automatically generate and save a visual `confusion_matrix.png` and export the trained model weights as `.pkl` files to the local directory.