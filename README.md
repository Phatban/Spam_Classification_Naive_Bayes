# 📚 Spam Message Classification using Naive Bayes

This project implements a simple and interpretable text classification model to detect spam messages using the **Naive Bayes** algorithm. It is part of the AI VIETNAM AIO 2024 program.

## 🔍 Project Objective

Classify SMS messages as either **ham** (legitimate) or **spam** (unsolicited/advertising) based on their content.

## 📁 Dataset

The dataset contains two columns:
- `Category`: either `ham` or `spam`
- `Message`: the SMS text

Example:
```
| Category | Message                                        |
|----------|------------------------------------------------|
| ham      | Ok lar... Joking wif u oni...                 |
| spam     | FreeMsg Hey there darling it’s been 3 weeks...|
```

Dataset source: [Kaggle - SMS Spam Collection](https://www.kaggle.com/datasets/team-ai/spam-text-message-classification)

## 🔧 Features

- Text preprocessing: lowercasing, punctuation removal, tokenization, stopword removal, stemming
- Bag-of-words feature extraction based on word frequencies
- Label encoding (`ham` → 0, `spam` → 1)
- Train/test/validation split
- Model training using **Gaussian Naive Bayes**
- Evaluation using **accuracy score**
- Prediction function for new user-defined messages

## 🛠️ Requirements

- Python 3.x
- pandas
- numpy
- scikit-learn
- nltk
- matplotlib (optional, for visualization)

Install dependencies:

```bash
pip install pandas numpy scikit-learn nltk matplotlib
```

## 🚀 How to Run

1. Clone this repository and open the Jupyter notebook (`.ipynb`) file.
2. Run the notebook step-by-step. It will automatically download the dataset using `gdown`.
3. The model will be trained and ready to make predictions on new messages.


## 🧠 Sample Prediction

```python
predict("Win a free ticket to Bahamas now!", model, dictionary)
# Output: 'spam'
```


## 📊 Visualization

This project includes several helpful visualizations to better understand the dataset and model behavior:

- **🔍 Label Distribution:** Shows the number of spam vs. ham messages.
- **📝 Message Length Distribution:** Histogram showing how long typical SMS messages are.
- **🚨 Most Frequent Words in Spam:** Top 20 most commonly used words in spam messages, helping interpret the model's focus.
- **📈 Training vs Validation Accuracy:** Bar chart comparing model performance across validation and test sets.


These visualizations can guide both preprocessing decisions and model evaluation.


## 📄 License

This project is for educational purposes under the AIO2024 course.

