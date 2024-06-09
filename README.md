# COVID-19 Articles Analysis Project
This repository contains a Jupyter Notebook for analyzing articles related to the coronavirus. The notebook includes data preprocessing, exploration, and modeling to analyze trends, sentiments, and key topics within the collected articles.

## Project Overview

The main objectives of this project are:
- **Data Preprocessing**: Clean and prepare the dataset for analysis.
- **Exploratory Data Analysis (EDA)**: Gain insights from the data through visualization and statistical analysis.
- **Natural Language Processing (NLP)**: Apply NLP techniques to extract meaningful information.
- **Modeling**: Build and evaluate models for tasks such as topic modeling and clustering.

## Getting Started

### Prerequisites

To run this notebook, you need to have the following software installed:
- Python 3.x
- Jupyter Notebook
- Required Python libraries (see below)

### Installation

1. Clone this repository to your local machine:

   ```bash
   git clone https://github.com/maryamjbr/article_analysis.git
   ```

2. Navigate to the project directory:

   ```bash
   cd article_analysis
   ```

3. Install the required Python libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn nltk spacy plotly langdetect
   ```

4. Download the required NLTK and SpaCy data:

   ```python
   import nltk
   nltk.download('punkt')
   nltk.download('wordnet')
   nltk.download('stopwords')
   ```

   ```bash
   python -m spacy download en_core_sci_lg
   ```

### Running the Notebook

1. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

2. Open the notebook file:

   ```bash
   DataMining_Project3_HSM.ipynb
   ```

3. Run the cells in the notebook sequentially to reproduce the analysis and results.

## Notebook Contents

The notebook includes the following sections:

1. **Introduction**: Overview of the project and objectives.
2. **Data Loading**: Load the dataset and necessary libraries.
3. **Data Preprocessing**: Clean and prepare the data for analysis, including text cleaning and normalization.
4. **Natural Language Processing (NLP)**: Apply NLP techniques such as tokenization, stemming, lemmatization, and stopwords removal.
5. **Feature Extraction**: Use TF-IDF to extract features from the text data.
6. **Dimensionality Reduction**: Apply PCA to reduce the dimensionality of TF-IDF features.
7. **Clustering**: Perform K-means clustering to group similar articles.
8. **Cluster Evaluation**: Evaluate the clusters using metrics like Silhouette Score and Davies-Bouldin Index.
9. **Visualization**: Visualize the clusters using t-SNE and create an interactive plot using Plotly.
10. **Topic Modeling**: Apply LDA to extract topics from the clusters.

## Data

The dataset consists of articles related to the coronavirus. It includes various features such as the publication date, article content, and metadata. The data preprocessing section involves cleaning the text data, handling missing values, and normalizing the text for analysis.

## Results

### Key topics discussed in the articles example
Cluster 1:
Topic 1: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo
Topic 2: lncrnas, cis, utr, noncod, rnas, outdoor, neighbor, nest, enforc, pol
Topic 3: cell, mice, express, immun, respons, activ, infect, ace, lung, cytokin
Topic 4: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo
Topic 5: lncrnas, rbd, revert, apelin, nasopharyng, pairwis, dish, adam, bronchoscopi, tokyo

Cluster 2:
Topic 1: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag
Topic 2: sirna, pdcov, knockdown, rnai, silenc, appendix, mainland, los, stream, organell
Topic 3: sequenc, genom, virus, use, rna, sampl, gene, assay, primer, strain
Topic 4: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag
Topic 5: sirna, appendix, mainland, knockdown, stream, organell, rnai, silenc, mab, languag

## t-SNE Visualization of TF-IDF Features with Cluster Labels
![DataMining_Project1](https://github.com/maryamjbr/article_analysis/assets/135154626/14504be4-c7f7-418e-943e-24ff8b6cade5)

## Cluster Visualization
![DataMining_Project2](https://github.com/maryamjbr/article_analysis/assets/135154626/ad47f80d-045c-4899-b783-0db107a004c1)
