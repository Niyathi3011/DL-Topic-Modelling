# DL-Topic-Modelling
1. To run DL_Project_Final.ipynb please install these dependencies.

```
pip install spacy-langdetect
pip install language-detector
pip install symspellpy
pip install sentence-transformers
pip install tensorflow --upgrade
pip install umap-learn
pip install stop-words
```

2. To run BERTopic.ipynb please install these dependencies.
```
pip install bertopic
pip install umap-learn
```

3. Please refer to DL_Project_Final.ipynb to reproduce Figures 1, 2, 3, 4, and Figures 6, 7. 
4. Please refer to BERTopic.ipynb to reproduce Figure 8, 9, 10 after data pre-processing.

5. README

Description:
This project aims to compare the performance of four prominent topic modeling methods: TF-IDF, BERT, LDA (Latent Dirichlet Allocation), and a combination of BERT and LDA known as BERT+LDA. The objective is to explore the effectiveness of combining traditional topic modeling methods with advanced language models to extract meaningful topics from a dataset of research paper abstracts.

Methods:
1. TF-IDF: Term Frequency-Inverse Document Frequency is a classic weighting scheme that represents the importance of a term in a document within a collection of documents. It assigns higher weights to terms that appear frequently in a document but are relatively rare in the corpus.

2. BERT: Bidirectional Encoder Representations from Transformers is a state-of-the-art language model that captures contextual and semantic information from text. It encodes documents into meaningful vector representations and has achieved excellent performance in various natural language processing tasks.

3. LDA: Latent Dirichlet Allocation is a generative probabilistic model widely used for topic modeling. It assumes that documents are generated from a mixture of topics, with each topic characterized by a distribution over words.

4. BERT+LDA: This method combines the strengths of BERT and LDA. It utilizes BERT for document encoding to capture contextual and semantic information, and then applies LDA to estimate the topic-word and document-topic distributions. The fusion of these techniques aims to enhance topic modeling results.

Observations:
The project compares the performance of these methods on a dataset of research paper abstracts. Several observations and evaluations were made:

1. Coherence Score: The coherence score, which measures the semantic similarity between words within a topic, was used to evaluate the quality and interpretability of the topics generated by each method. Higher coherence scores indicate more meaningful and coherent topics.

2. Silhouette Score: The silhouette score, a metric used to evaluate the quality of clusters in unsupervised learning tasks, was calculated to assess the quality of the topic clusters generated by each method.

3. Experimental Setup: The experiments were conducted on Google Colab using a sample size of 1000 abstracts and 12 topics. Preprocessing techniques were applied to clean the text data and ensure optimal results.

Tech Stack:
The following technologies and libraries were used in the project:

- Python: The programming language used for implementing the topic modeling methods and analysis.
- Google Colab: The platform utilized for executing the code and running the experiments.
- NLTK (Natural Language Toolkit): A library used for text preprocessing, including removing punctuation, filtering words, assigning POS tags, and correcting typos.
- Hugging Face Transformers: A library used for leveraging pre-trained language models such as BERT for document encoding and semantic understanding.
- Scikit-learn: A machine learning library used for implementing the LDA algorithm and evaluating the topic modeling results.
- Pandas: A data manipulation library used for handling and analyzing the dataset of research paper abstracts.
- NumPy: A library used for numerical computations and array operations.

This project provides valuable insights into the effectiveness of different topic modeling techniques and their potential to uncover hidden patterns and gain insights from vast document collections. The comparative analysis serves as a foundation for developing more efficient and accessible topic modeling methods and driving data-informed decision-making in various domains.
