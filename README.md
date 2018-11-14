Women's Clothing E-Commerce Reviews-NLP

==================================================================================

<h1>Women's Clothing E-Commerce Reviews</h1>

==================================================================================

<h3>Overview</h3>

<p>The objective of this project is to determine the rating for the product of an e-commerce website. The dataset was obtained from Kaggle.</p>

==================================================================================

<h3>Dataset</h3>

The dataset contains 9 features

| Feature                 | Description                                               |
| ----------------------- | --------------------------------------------------------- |
| Age                     | Age of the women customer                                 |
| Title                   | Title of the review                                       |
| Review Text             | Customer Review                                           |
| Rating                  | Rating given by customer                                  |
| Recommended IND         | Whether the product is recommended or not by the reviewer |
| Positive Feedback Count | Number of positive feedback on the review                 |
| Division Name           | Name of the division, the product belongs                 |
| Department Name         | Name of the department, the product belongs               |
| Class Name              | Type of product                                           |

==================================================================================

<h3>Preprocessing</h3>


<p ALIGN=JUSTIFY>The preprocessing involve handling high values which was handled using min-max scaler.  The title and the review text was combined to get full text data.  The processing on the text data involves removing punctuations, lemmatization and tokenization. Only words were used for the analysis purpose, and words with less than 3 characters are removed. Moreover, the words which are rare that is frequency less than 5 was also removed. TF-IDF was used to vectorize the text data. In addition to this, length of the review, percentage of punctuations, sentiment of the data and the polarity of the data was added to the dataset for analysis purpose. The data was found to unbalanced hence SMOTE was used for over sampling. </p>

==================================================================================

<h3>Result</h3>

<p>The model was created using KNN classifier as this model provided the best result. The details of the model are given below:</p>



| Metrics           | Value                                                    |
| ----------------- | -------------------------------------------------------- |
| Training Accuracy | 79.769%                                                  |
| Testing Accuracy  | 77.381%                                                  |
| F1 Score          | [0.97980553 0.97165384 0.8712424  0.68621876 0.10812721] |
| Precision         | [0.96678967 0.95533407 0.80688767 0.56159687 0.75369458] |
| Recall            | [0.99317665 0.98854087 0.94675227 0.88192308 0.05824134] |

==================================================================================









