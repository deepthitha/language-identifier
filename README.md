# Text Classification Project

This project involves building and evaluating machine learning models for text classification. The primary objective is to identify the language of given text inputs.

## Table of Contents

- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Evaluation](#model-evaluation)
- [Predictions](#predictions)
- [Contributing](#contributing)

## Project Overview

This project aims to classify text into different languages using various machine learning models. It includes data preprocessing, training multiple models, evaluating their performance, and making predictions on new text data.

## Dataset

The dataset used in this project includes text samples in various languages. The text data is preprocessed to remove noise and converted into a suitable format for model training.

## Installation

To run this project, you need to have Python and Jupyter Notebook installed. You can install the required libraries using the following command:

```bash
pip install -r requirements.txt
```

## Usage

To use this project, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/your-username/your-repo-name.git
    ```
2. Navigate to the project directory:
    ```bash
    cd your-repo-name
    ```
3. Open the Jupyter Notebook:
    ```bash
    jupyter notebook Project.ipynb
    ```

## Model Evaluation

The notebook evaluates the performance of different machine learning models using accuracy scores and confusion matrices. The following models are evaluated:

- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)

The confusion matrices for each model are displayed to provide insights into their performance.

## Predictions

To make predictions on new text data, use the `prediction` function defined in the notebook. Here's an example:

```python
def prediction(text):
    x = CV.transform([text]).toarray()
    lang = model.predict(x)
    lang = encoder.inverse_transform(lang)
    print("This word/sentence contains {} word(s).".format(lang[0]))

# Example usage
prediction("Your sample text here")
```

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss your ideas or improvements.
