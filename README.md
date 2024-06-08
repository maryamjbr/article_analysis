# COVID-19 Articles Analysis Project
This repository contains a Jupyter Notebook for analyzing articles related to the coronavirus. The notebook includes data preprocessing, exploration, and modeling to analyze trends, sentiments, and key topics within the collected articles.
## The main objectives of this project are:
- Introduction: Overview of the project and objectives.
- Data Loading: Load the dataset and necessary libraries.
- Data Preprocessing: Clean and prepare the data for analysis, including text cleaning and normalization.
- Natural Language Processing (NLP): Apply NLP techniques such as tokenization, stemming, lemmatization, and stopwords removal.
- Feature Extraction: Use TF-IDF to extract features from the text data.
- Dimensionality Reduction: Apply PCA to reduce the dimensionality of TF-IDF features.
- Clustering: Perform K-means clustering to group similar articles.
- Cluster Evaluation: Evaluate the clusters using metrics like Silhouette Score and Davies-Bouldin Index.
- Visualization: Visualize the clusters using t-SNE and create an interactive plot using Plotly.
- Topic Modeling: Apply LDA to extract topics from the clusters.
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
