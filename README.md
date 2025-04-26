📚 Fellowship.ai Cohort 35 Submission _(NLP)_

Welcome to my repository made for the Fellowship.ai Cohort 35 submission, focused on NLP task. 

The task given was to perform sentiment analysis on the `IMDb Dataset of 50K Movie Reviews` dataset.

---

## 🌟 Project Overview
This repository showcases sentiment analysis on IMDb datasets obtained from Kaggle.  
The project follows a traditional machine learning approach using Logistic Regression for classification after text preprocessing and feature extraction (TF-IDF Vectorization).

---

## 💾 Dataset Access
The IMDb dataset used in this project can be downloaded from Kaggle. You must have Kaggle API credentials set up to access the dataset programmatically. You can find the dataset at the following link:

🔗 [IMDb Dataset of 50K Movie Reviews](https://www.kaggle.com/datasets/lakshmi25npathi/imdb-dataset-of-50k-movie-reviews/data)
To download the dataset using Kaggle's API, include the following script at the top of your notebook:
```python
!pip install kaggle
!mkdir ~/.kaggle
!echo '{"username":"YOUR_USERNAME","key":"YOUR_KEY"}' > ~/.kaggle/kaggle.json
!chmod 600 ~/.kaggle/kaggle.json
!kaggle datasets download -d lakshmi25npathi/imdb-dataset-of-50k-movie-reviews --unzip
```
Replace `YOUR_USERNAME` and `YOUR_KEY` with your Kaggle username and API key.

---

## 📂 Notebook

### 📈 Traditional Method: Logistic Regression
- Notebook: [task_fellowship.ipynb](./task_fellowship.ipynb)
- Model: Logistic Regression
- Description:  
  - Preprocesses movie reviews by cleaning text (removing HTML tags and punctuations).
  - Converts cleaned text into numerical features using TF-IDF vectorization.
  - Splits the data into training and testing sets.
  - Trains a Logistic Regression model to predict whether a review is positive or negative.
  - Evaluates the model's performance using accuracy, classification report, and confusion matrix.
  - Predicts sentiments for some custom movie reviews and displays confidence scores.
  - Visualizes results using Seaborn (Sentiment distribution, Correlation heatmap, Confusion matrix).

- Metrics:
    - Accuracy: 0.90
    - Sample Confusion Matrix:
    ```plaintext
                   precision    recall  f1-score   support

        Negative       0.90      0.88      0.89      4961
        Positive       0.89      0.91      0.90      5039

        accuracy                           0.90     10000
        macro avg       0.90      0.89     0.90     10000
        weighted avg    0.90      0.90     0.90     10000
    ```

---

## ⚙️ How to Run:

1. Clone the repository:
    ```bash
    git clone https://github.com/coder-swastik/Sentiment_Analysis_IMDB.git
    ```
2. Navigate to the project directory:
    ```bash
    cd Sentiment_Analysis_IMDB
    ```
3. Install the required libraries:  
   Make sure you have Python 3.8+ installed. Then run:
    ```bash
    pip install -r requirements.txt
    ```
4. Run the notebook:
    ```bash
    jupyter notebook
    ```

---

## ☕ Requirements

- Python 3.8+

- Jupyter Notebook

- Required Python libraries:
    - pandas
    - numpy
    - seaborn
    - matplotlib
    - scikit-learn
    - re (built-in)
    - kaggle (for dataset download)



---

## ✅ Features

- Preprocessing pipeline to clean real-world noisy text data.

- TF-IDF feature extraction for effective text representation.

- Logistic Regression model for binary sentiment classification.

- Custom predictions on unseen movie reviews with confidence probabilities.

- Detailed evaluation and visualization (heatmaps, confusion matrix, distribution plots).

- Clean and beginner-friendly implementation.

---
