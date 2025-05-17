# Amazon Product Scraper & Review Analyzer

## Description

This project scrapes product information and customer reviews from Amazon. 
It can extract detailed reviews for a specific product URL or search for products by keyword, gathering general product data and their reviews.
The collected review text is then cleaned and analyzed for common phrases (n-grams) and prepared for sentiment analysis.

## Core Features

* **Targeted Review Scraping**: Extracts customer name, date, rating, title, and content for a given Amazon product.
* **Keyword-Based Product Search**: Fetches product details (title, price, rating, availability) and reviews based on a search term.
* **Data Output**: Saves scraped product data to a Pandas DataFrame and optionally to a CSV file (`amazon_data.csv`).
* **Text Preprocessing**: Cleans review text by removing HTML, URLs, punctuation, and converting to lowercase.
* **N-gram Analysis**: Identifies common bi-grams and tri-grams in reviews.
* **Sentiment Analysis Ready**: Includes functions and library imports (TextBlob, NLTK VADER) for sentiment classification.

## Key Libraries

* `pandas`: For data manipulation.
* `requests`: For HTTP requests.
* `BeautifulSoup4`: For HTML parsing.
* `nltk`: For text processing (stopwords, sentiment).
* `textblob`: For text processing and sentiment.
* `scikit-learn`: For `CountVectorizer` (n-grams).
* `seaborn`/`matplotlib`: For plotting (used for n-gram visualization).
