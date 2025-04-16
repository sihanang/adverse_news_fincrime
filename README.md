# Adverse News for Financial Crime Risk Detection

**Adverse News for Financial Crime Risk Detection** is a project aimed at leveraging Natural Language Processing (NLP) and Machine Learning (ML) techniques to detect and analyze adverse news articles that may indicate potential financial crimes. This tool is particularly useful for financial institutions and compliance teams to enhance their risk assessment processes.

## Table of Contents

- [Project Overview](#project-overview)
- [Features](#features)
- [Data](#data)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Contributing](#contributing)
- [License](#license)

## Project Overview

This project focuses on the automated detection of adverse news related to financial crimes. By processing and analyzing news articles, the system identifies entities and categorizes the content to assist in risk management and compliance efforts.

## Features
- **Gnews API calls + Webscraping**: Extracting news from gnews API and doing webscraping in an attempt to obtain more information on the articles.
- **Data Preprocessing**: Cleaning and preparing news data for analysis.
- **Named Entity Recognition (NER)**: Identifying and extracting relevant entities from text.
- **Topic Modeling**: Uncovering hidden thematic structures in news articles.
- **Classification Models**: Implementing models to classify news articles based on risk levels.
- **Visualization**: Generating insightful visual representations of data and model outputs.

## Data

The dataset comprises news articles that have been preprocessed and labeled for training and evaluation purposes. Key data files include:

- `final_cleaned_news_data_sampled.parquet`: Sampled and cleaned news data.
- `named_entities.parquet`: Extracted named entities from the articles.
- `linked_entities.parquet`: Entities linked to external knowledge bases.

*Note: Ensure compliance with data usage policies when utilizing the provided datasets.*

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/sihanang/adverse_news_fincrime.git
   cd adverse_news_fincrime
   ```

2. **Create a Virtual Environment**:
   ```bash
   python3 -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

*Note: Ensure that you have Python 3.7 or higher installed.*

## Usage

The project includes several Jupyter notebooks demonstrating various components:

- `Data_Loading_Final.ipynb`: Loading and exploring the dataset.
- `Data_Preprocessing_Final.ipynb`: Data cleaning and preprocessing steps.
- `NER_final.ipynb`: Performing Named Entity Recognition and Entity Linking.
- `Local_DS_Modelling.ipynb`: Building and evaluating classification models.
- `MetaClassifier_of_LLM_outputs.ipynb`: Combining outputs from multiple LLMs.
- `Visualisations.ipynb`: Visualizing data and model results.

To run a notebook:

1. Activate the virtual environment:
   ```bash
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

2. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

3. Open the desired notebook and execute the cells sequentially.

## Project Structure

```
adverse_news_fincrime/
├── categories_pred/                 # Predicted categories
├── evaluation/                      # Evaluation metrics and results
├── llm/                             # Large Language Model outputs
├── sample_labelled/                 # Sample labeled data
├── *.ipynb                          # Jupyter notebooks for various tasks
├── *.parquet                        # Processed data files
├── *.png                            # Visualizations
├── requirements.txt                 # Project dependencies
└── README.md                        # Project documentation
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m 'Add your message here'
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

Please ensure that your code adheres to the project's coding standards and includes appropriate tests.
