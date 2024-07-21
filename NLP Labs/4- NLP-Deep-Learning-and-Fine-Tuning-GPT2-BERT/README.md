# Lab : Get familiar with NLP language models using Pytorch library

Tools: Kaggle, github, NLTK, Pytorch.

# Summary of Learning from Lab 4: NLP Language Models using Pytorch

### Objective :
The primary goal of Lab 4 was to become acquainted with Natural Language Processing (NLP) models using the Pytorch library. This involved tasks ranging from text data collection to model training and evaluation.

## Part 1 : Classification Regression


1. Data Collection :
    * Utilized web scraping libraries (Scrapy/BeautifulSoup) to gather Arabic text data from various websites centered on a specific topic.
    * Prepared a dataset where each text had an associated relevance score (0-10).
    
    
2. Data Preprocessing :
    * Established an NLP preprocessing pipeline involving tokenization, stemming, lemmatization, stop-word removal, and text discretization.
    * Implemented text cleaning functions to remove HTML tags, non-Arabic characters, and unnecessary spaces.


3. Model Training :
    * Trained several models including RNN, Bidirectional RNN, GRU, and LSTM architectures.
    * Tuned hyperparameters to enhance model performance.
    * Developed a custom dataset class for handling text and score data, leveraging Word2Vec embeddings for text representation.
    
    
4. Model Evaluation :
    * Evaluated models using standard metrics like accuracy, loss, and additional metrics like BLEU score.
    * Implemented a training loop to compute Mean Squared Error (MSE) loss and track model performance over epochs.


## Part 2 : Transformer (Text Generation)


1. Model Setup:
    * Installed Pytorch-transformers and loaded the pre-trained GPT2 model.
    
    
2. Fine-Tuning:
    * Fine-tuned the GPT2 model on a customized dataset.
    
    
3. Text Generation:
    * Used the fine-tuned model to generate new paragraphs based on given sentences, enhancing understanding of transformer-based text generation.


## Part 3 : BERT


1. Model Establishment:
    * Used the pre-trained bert-base-uncased model.
    * Adapted the BERT embedding layer to fit the dataset.
    
    
2. Data Preparation and Fine-Tuning:
    * Prepared data and fine-tuned the BERT model by selecting optimal hyperparameters.
    
    
3. Model Evaluation:
    * Evaluated the fine-tuned BERT model using standard metrics (accuracy, loss, F1 score) and additional metrics such as BLEU score and BERT-specific metrics.
    
    
4. Conclusion:

    * Provided a general conclusion on the efficacy of using pre-trained BERT models for NLP tasks.


## Key Learnings :

   * Data Preprocessing : Gained hands-on experience with Arabic text data preprocessing, including tokenization, stop-word removal, stemming, and lemmatization.
   * Model Training : Learned to implement and train various RNN-based models and transformers like GPT2 and BERT.
   * Fine-Tuning : Understood the process of fine-tuning pre-trained models on custom datasets.
   * Evaluation Metrics : Became proficient in evaluating models using both standard and advanced NLP metrics.
