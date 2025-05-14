# Hybrid Sentiment Analysis Model

This project enhances sentiment analysis by combining two powerful models: **BERT** and **VADER**. The hybrid approach leverages BERT’s deep contextual understanding with VADER’s rule-based efficiency to improve sentiment classification accuracy.

> Two classifiers were tested: **Logistic Regression** and **Random Forest**.  
> ✅ **Random Forest** provided better overall performance and is used in the final model.

---

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Files Overview](#files-overview)
- [Contributing](#contributing)
- [License](#license)

---

## Introduction

Sentiment analysis is a crucial NLP task, and this hybrid model seeks to boost performance by combining:
- **BERT**: A transformer-based model from Hugging Face's `transformers` library for understanding deep language context.
- **VADER**: A lexicon and rule-based sentiment analysis tool, ideal for social media and short texts.

The hybrid model uses sentiment scores from both models as features to train a meta-classifier.

---

## Prerequisites

- Python 3.x
- Hugging Face Transformers
- NLTK
- Scikit-learn
- Pandas
- Joblib

---

## Installation

1. Clone the repository:

```bash
git clone https://github.com/mhdatheek136/NLP_Project.git
cd NLP_Project
````

2. Install required libraries:

```bash
pip install -r requirements.txt
```

If `requirements.txt` is missing, manually install:

```bash
pip install transformers nltk scikit-learn pandas joblib
```

---

## Usage

1. **Preprocess the dataset**

   ```bash
   Open and run: data_preprocessing.ipynb
   ```

2. **Generate sentiment scores**

   * BERT:

     ```bash
     Open and run: BERT_sentiment.ipynb
     ```
   * VADER:

     ```bash
     Open and run: VADER_sentiment.ipynb
     ```

3. **Create training dataset**

   ```bash
   Open and run: target.ipynb
   ```

4. **Train classifiers**

   * Logistic Regression:

     ```bash
     Open and run: classifier.ipynb
     ```
   * Random Forest (preferred):

     ```bash
     Open and run: random_forest.ipynb
     ```

5. **Compare model performance**

   ```bash
   Open and run: hybrid_sentiment.ipynb
   ```

6. **Predict sentiment using the trained hybrid model**

   ```bash
   Open and run: hybrid_function.ipynb
   ```

---

## Files Overview

| File                       | Description                              |
| -------------------------- | ---------------------------------------- |
| `BERT_sentiment.ipynb`     | Generate sentiment using BERT            |
| `VADER_sentiment.ipynb`    | Generate sentiment using VADER           |
| `data_preprocessing.ipynb` | Clean and prepare dataset                |
| `target.ipynb`             | Create combined target features          |
| `classifier.py`            | Train Logistic Regression                |
| `random_forest.ipynb`      | Train and evaluate Random Forest model   |
| `hybrid_sentiment.ipynb`   | Model comparison and analysis            |
| `hybrid_function.ipynb`    | Final testing using `final_model.joblib` |
| `final_model.joblib`       | Trained Random Forest classifier         |
| `research_paper.pdf`       | Methodology and background               |

---

## Contributing

Contributions are welcome! Please feel free to fork the repository, create a branch, and submit a pull request. Refer to the [CONTRIBUTING.md](CONTRIBUTING.md) for detailed guidelines.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

``

For more details, refer to the accompanying research paper (`research_paper.pdf`). If you encounter any issues or have any questions, please open an issue in the repository or contact the project maintainers.

Happy coding!
