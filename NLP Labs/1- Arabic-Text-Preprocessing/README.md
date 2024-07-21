# Lab : Get familiar with Scraping and NLP Pipeline ( Arabic Text )

Tools : Google colab, github, NLTK, Farasa API

## Table of contents
 - [Introduction](https://github.com/aymanboufarhi/Arabic-Text-Preprocessing?tab=readme-ov-file#introduction)
 - [Data Acquisition](https://github.com/aymanboufarhi/Arabic-Text-Preprocessing?tab=readme-ov-file#data-acquisition)
 - [Text Cleaning](https://github.com/aymanboufarhi/Arabic-Text-Preprocessing?tab=readme-ov-file#text-cleaning)
 - [Text Preprocessing](https://github.com/aymanboufarhi/Arabic-Text-Preprocessing?tab=readme-ov-file#text-preprocessing)
 - [Synthesis](https://github.com/aymanboufarhi/Arabic-Text-Preprocessing?tab=readme-ov-file#synthesis)

## Introduction
In this lab, we delved into the realms of web scraping and Natural Language Processing (NLP) to extract insights from Arabic web sources. Leveraging tools such as Beautiful Soup, MongoDB, NLTK, and Farasa API, our objective was to scrape data, store it in a NoSQL database, and apply various NLP techniques for analysis. Through this report, we document our journey, challenges faced, and insights gained, contributing to the broader understanding of these powerful methodologies.

## Data Acquisition
In this section, we acquired raw content from the website "mawdoo3.com" regarding general culture about Morocco. We used Python's requests library to fetch the HTML content, then parsed it using BeautifulSoup for readability. After establishing a connection to MongoDB Atlas, we stored the parsed HTML content along with the URL in a MongoDB collection named "web_data_collection." This step lays the groundwork for subsequent analysis and processing in our NLP pipeline.

## Text Cleaning
In the text cleaning process, we began by retrieving the raw data stored in MongoDB. After obtaining the HTML content, we used BeautifulSoup to parse the content and extract the text. Following this extraction, we implemented a cleaning function to remove HTML tags, non-Arabic characters, and extra spaces from the text. This function ensured that our data remained focused on the Arabic language, essential for subsequent NLP tasks.

Next, we defined a function to extract and clean text from specific HTML tags such as headers (h1) and paragraphs (p). This function iterated through these tags, concatenated the text, and applied the previously defined cleaning procedure.

Additionally, we included a step for correcting word spellings using a contextual corrector. However, in our case, since we extracted text from a professional website, we opted not to utilize this step, as the text is expected to have correct spelling.

By executing these steps, we obtained a cleaned text corpus ready for further processing in our NLP pipeline.

## Text Preprocessing
In our journey to prepare Arabic text for advanced language processing, we've been working hard to get it right from the start. First, we made sure all the text was encoded consistently using Unicode normalization. This helped fix any issues with how the text was represented. Then, we moved on to tokenization, which means breaking the text into smaller parts called tokens. This makes it easier to analyze and pick out specific features.

As we delved deeper into our text processing journey, we carefully refined the text by removing common stop words using NLTK's Arabic corpus. This helped us focus more on the main content. We also paid close attention to stemming and lemmatization, important steps where we looked into various algorithms like ISRIStemmer, SnowballStemmer, and ARLSTem. Additionally, we used the Farasa API for advanced lemmatization capabilities. By comparing these methods, we understood the balance between making words smaller and keeping their meaning intact, which helped us make better decisions for our language processing goals.

During our journey, we encountered real-life examples that showed the importance of lemmatization and stemming in refining Arabic text. For example, when we used lemmatization with the Farasa API, it accurately transformed words into their base forms. For instance, "والبرتغال" (meaning 'and Portugal') became "برتغال," keeping its meaning intact. Similarly, "إسبانيا" (meaning 'Spain') stayed the same, showing how the Farasa API effectively preserves meaning.

On the other hand, stemming algorithms like ISRIStemmer, SnowballStemmer, and ARLSTem showed their ability to reduce words to their basic forms. However, at times, they produced stems that didn't match valid Arabic words. For example, when stemming the word "والبرتغال," they gave "رتغال" instead of the accurate base form "برتغال" provided by the Farasa API. Similarly, for "إسبانيا," the stemming algorithms gave "سبن," which might not be a valid Arabic word, unlike the Farasa API's ability to keep the original form.

These examples clearly show the subtle differences between lemmatization and stemming methods. Lemmatization, as demonstrated by the Farasa API, prioritizes keeping the meaning of words accurate by considering their context. On the other hand, stemming algorithms mainly focus on simplifying words based on their structure, sometimes sacrificing accuracy to save computing resources. So, the choice between lemmatization and stemming depends on the specific needs of the language processing task, with lemmatization being preferred when preserving meaning is crucial.

Our exploration didn't stop there; we also delved into the complex field of Parts of Speech (POS) tagging. Here, we identified the grammatical structures of Arabic using both rule-based and machine learning methods. Using detailed rules and regular expressions, we developed a system to assign grammatical categories to words. At the same time, we employed machine learning techniques with NLTK's pre-trained statistical model to recognize parts of speech, drawing on patterns learned from annotated data to achieve accurate categorization. This comprehensive approach not only shed light on the intricacies of Arabic grammar but also highlighted the effectiveness of both rule-based and machine learning approaches in addressing linguistic challenges.

Bringing our journey to a close, we ventured into Named Entity Recognition (NER), a crucial task for identifying important entities in unstructured text. Using both NLTK and the Farasa API, we explored how to pinpoint proper nouns, locations, organizations, and other significant elements within the text. This comprehensive approach not only deepened our understanding of entity recognition methods but also revealed the semantic richness present in Arabic text.

In essence, our journey through text preprocessing represents a thorough exploration, employing various techniques and tools to refine raw text into a structured and insightful dataset. By addressing Unicode normalization, tokenization, stop word removal, stemming, lemmatization, POS tagging, and NER, we've established a solid groundwork for future NLP tasks. This positions us well to extract meaningful insights and tap into the hidden potential within Arabic text.

## Synthesis
Throughout the lab, I gained valuable insights into web scraping, data preprocessing, and natural language processing (NLP) techniques.

Firstly, I learned how to use Beautiful Soup to extract data from various Arabic websites efficiently, allowing me to gather valuable information.

Secondly, I explored storing the scraped data in a NoSQL database like MongoDB, both locally and on MongoDB Atlas (Cloud). This hands-on experience introduced me to new types of databases.

In the realm of NLP, I understood the importance of text cleaning, tokenization, and normalization in preparing textual data for analysis. Techniques like removing stop words, punctuation, and special characters helped improve the quality of subsequent analyses.

I also delved into stemming and lemmatization, which provided insights into different ways to normalize words. While stemming was quicker and lighter, lemmatization preserved the meaning of words at a slightly higher computational cost.

Furthermore, I explored parts-of-speech (POS) tagging using both rule-based and machine learning approaches. Rule-based tagging allowed for explicit rule definitions, while machine learning-based tagging used annotated data to identify language usage patterns.

Additionally, I experimented with named entity recognition (NER) using NLTK and the Farasa API, which helped identify and categorize entities like names, organizations, and locations in Arabic text. This experience broadened my understanding of using REST APIs for NLP tasks.

Overall, this lab provided me with a comprehensive understanding of data acquisition, preprocessing, and the NLP pipeline, setting a strong foundation for future endeavors in data science and text analysis.
