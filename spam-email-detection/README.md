# Email Spam Classification Project

A machine learning system designed to analyze and classify text messages or emails into two categories: **Spam** or **Ham** (Legitimate). 

---

## 📝 Project Overview
This project converts raw, unstructured textual data into meaningful numerical representations, resolves common pipeline bugs like feature mismatches, and applies a binary classifier to predict the nature of incoming messages with high precision.

---

## 🛠️ Tools & Technologies
*   **Python:** The core programming language used for script execution and model design.
*   **Scikit-Learn:** Used for feature extraction (text vectorization) and training the machine learning pipeline.
*   **Pandas & NumPy:** Utilized for structured data loading, matrix reshaping, and preprocessing arrays.
*   **Jupyter Notebook:** The interactive environment used for prototyping, debugging, and visualization.

---

## 🤖 The Model
*   **Algorithm:** `Logistic Regression`
*   **Type:** Binary Classification (Output: `0` for Spam, `1` for Ham).
*   **Feature Extraction:** Term Frequency-Inverse Document Frequency (`TfidfVectorizer`) or `CountVectorizer`. 
*   **Pipeline Strategy:** The text vectorizer learns vocabulary strictly from the training dataset (`.fit_transform()`) and merely projects test/live samples onto that fixed vocabulary (`.transform()`). This strict design prevents data leakage and ensures feature shape consistency.

---

## 📊 The Dataset
*   **Content:** A collection of labeled text messages/emails containing both legitimate communications and junk/phishing texts.
*   **Target Variables:**
    *   **Text/Message:** The raw text string containing the email subject line or body content.
    *   **Category/Label:** The target label identifying the message type (typically mapped numerically where Spam = 0 and Ham = 1).
