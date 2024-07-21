# Lab : Get familiar with NLP Rule based, Regex and NLP Word embedding

Tools : Google colab, github, NLTK, Sklearn.

## Table of contents
 - [Lab Overview](https://github.com/aymanboufarhi/Rule-based-Regex-and-NLP-Word-embedding?tab=readme-ov-file#lab-overview)
 - [Part 1](https://github.com/aymanboufarhi/Rule-based-Regex-and-NLP-Word-embedding?tab=readme-ov-file#part-1)
 - [Part 2](https://github.com/aymanboufarhi/Rule-based-Regex-and-NLP-Word-embedding?tab=readme-ov-file#part-2)
 - [Evaluation and Conclusion](https://github.com/aymanboufarhi/Rule-based-Regex-and-NLP-Word-embedding?tab=readme-ov-file#evaluation-and-conclusion)
 - [Key Learnings](https://github.com/aymanboufarhi/Rule-based-Regex-and-NLP-Word-embedding?tab=readme-ov-file#key-learnings)

## Lab Overview
The project delved into the realms of Natural Language Processing (NLP) and word embedding techniques to enhance understanding and processing of textual data. It aimed to explore various methodologies for extracting structured information from unstructured text and representing words in a numerical vector space. The project was divided into two main parts: NLP Rule-Based and Regex, and Word Embedding Techniques.

## Part 1
In this part, we focused on utilizing regular expressions (Regex) to extract structured information from unstructured text data. We developed a function, generate_bill, which employed Regex patterns to identify and extract product names, quantities, and prices from a given text input representing a bill. This approach proved effective in scenarios where the text followed a specific format or pattern.

## Part 2
We explored various word embedding techniques to represent words in a numerical vector space, enabling machines to understand and process textual data effectively.

- One-Hot Encoding, Bag of Words, TF-IDF : Traditional techniques to convert text data into numerical vectors, capturing word frequency and importance.

- Word2Vec (Skip-gram, CBOW) : Neural network-based models to learn distributed representations of words, capturing semantic relationships.

- GloVe and FastText : Techniques leveraging co-occurrence statistics and subword information, respectively, to generate word vectors.

## Evaluation and Conclusion
Visualizations using t-Distributed Stochastic Neighbor Embedding (t-SNE) provided insights into the performance and effectiveness of encoded word vectors. While traditional techniques like one-hot encoding and Bag of Words offer simplicity, they may lack in capturing semantic relationships. Neural network-based methods like Word2Vec, GloVe, and FastText provide more nuanced representations, enabling better understanding of word semantics and relationships.

In conclusion, the project highlighted the importance of NLP rule-based methods, Regex, and word embedding techniques in processing and representing textual data effectively. Each technique has its strengths and weaknesses, and selecting the appropriate approach depends on the specific task requirements. Understanding and leveraging these techniques empower various NLP applications, including information extraction, sentiment analysis, and more.

## Key Learnings
- Regular expressions (Regex) are powerful tools for extracting structured information from unstructured text data.
- Word embedding techniques enable effective representation of words in a numerical vector space, facilitating semantic understanding.
- Evaluating techniques through visualizations such as t-SNE provides insights into their performance and effectiveness.
- Choosing the right technique depends on the task requirements and the desired level of semantic understanding.

By combining NLP rule-based methods, Regex, and word embedding techniques, this project laid the groundwork for understanding and processing textual data effectively, paving the way for more advanced applications in natural language understanding and processing.
