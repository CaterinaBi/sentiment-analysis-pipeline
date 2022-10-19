#  😞 Pipeline for sentiment analysis (TensorFlow) 😊

End-to-end data preprocessing pipeline and sequential modelling in RNN intended for sentiment analysis. The pipeline is an implementation of this [pipeline](https://www.kaggle.com/code/thebratattack/sentiment-analysis-pipeline-with-tensorflow/notebook) by Satya Mishra (@Satyabratam945), whose model we re-trained using a different dataset.

The dataset used is the [Stanford Sentiment Treebank](https://nlp.stanford.edu/sentiment/code.html). The dataset — which is free to download and doesn’t require registration of any sorts — contains 10,605 processed snippets from a pool of Rotten Tomatoes HTML files. The dataset includes sentiment annotations and derives from the following paper:

> Recursive Deep Models for Semantic Compositionality Over a Sentiment Treebank, Socher et al., Conference on Empirical Methods in Natural Language Processing (EMNLP, 2013).

To have a dataset with the same structure as the one used in the original pipeline, I created `dataset.csv`, a file that maps all snippets from our chosen dataset to their corresponding score. I did so with the code in `dataset_file_creation.ipynb`. 