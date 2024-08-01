# Hybrid Sentiment Analysis Model

This project aims to enhance the efficiency of sentiment analysis by combining the BERT and VADER models to create a hybrid model. By leveraging the strengths of both models, the hybrid model aims to improve sentiment classification performance.

## Table of Contents
- [Introduction](#introduction)
- [Directory Structure](#directory-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Files Overview](#files-overview)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The project combines BERT, a transformer-based model for natural language understanding, with VADER, a rule-based model for sentiment analysis. The hybrid model aims to improve sentiment analysis by leveraging the contextual understanding of BERT and the simplicity and efficiency of VADER.

## Directory Structure
```
.
├── BERT_sentiment.py
├── VADER_sentiment.py
├── data_preprocessing.py
├── target.py
├── classifier.py
├── hybrid_sentiment.py
├── hybrid_function.py
├── final_model.joblib
├── README.md
└── research_paper.pdf
```

## Prerequisites
- Python 3.x
- Transformers library (Hugging Face)
- NLTK
- scikit-learn
- joblib
- pandas

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/hybrid-sentiment-analysis.git
   cd hybrid-sentiment-analysis
   ```

2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
1. Preprocess the dataset:
   ```bash
   python data_preprocessing.py
   ```

2. Generate BERT sentiment scores:
   ```bash
   python BERT_sentiment.py
   ```

3. Generate VADER sentiment scores:
   ```bash
   python VADER_sentiment.py
   ```

4. Create the training dataset:
   ```bash
   python target.py
   ```

5. Train the hybrid model:
   ```bash
   python classifier.py
   ```

6. Compare the models:
   ```bash
   python hybrid_sentiment.py
   ```

7. Test the hybrid function:
   ```bash
   python hybrid_function.py
   ```

## Files Overview
- **BERT_sentiment.py**: Script to generate sentiment scores using the BERT model.
- **VADER_sentiment.py**: Script to generate sentiment scores using the VADER model.
- **data_preprocessing.py**: Script for preprocessing the dataset from Kaggle.
- **target.py**: Script to create the training dataset combining BERT and VADER scores.
- **classifier.py**: Script for training the hybrid sentiment analysis model.
- **hybrid_sentiment.py**: Script to compare the performance of BERT, VADER, and the hybrid model.
- **hybrid_function.py**: Script to test the hybrid function using the trained model (`final_model.joblib`).

## Contributing
Contributions are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

For more details, refer to the accompanying research paper (`research_paper.pdf`). If you encounter any issues or have any questions, please open an issue in the repository or contact the project maintainers.

Happy coding!
