# Amazon Best Seller Book Web Scraping Project

## Project Description
This project demonstrates the process of scraping Amazon's best-selling books list using Python. The script utilizes web scraping techniques with libraries such as `requests`, `BeautifulSoup`, and `pandas` to gather data on the top-selling books from Amazon.

### Key Steps:
1. **Web Scraping**: The script sends HTTP requests to the Amazon Best Seller page using the `requests` library. The page's HTML content is then parsed using `BeautifulSoup`, which allows us to extract specific data points such as book titles, authors, ratings, review counts, prices, and product links.

2. **Data Extraction**: 
   - The script targets specific HTML elements (such as divs, spans, and anchors) that contain relevant product information.
   - Data is collected for each book displayed in the "Best Sellers" section and includes essential details like:
     - **Title**: The name of the book.
     - **Author**: The author(s) of the book.
     - **Rating**: The average customer rating of the book.
     - **Number of Reviews**: The total number of reviews the book has received.
     - **Price**: The price of the book.
     - **Product Link**: A direct link to the Amazon product page.

3. **Data Cleaning and Processing**: 
   - The extracted data is processed using `pandas` to handle missing values, convert numerical data to appropriate formats, and ensure the dataset is structured for easy analysis.
   
4. **Data Export**: 
   - After processing, the data is saved in a CSV file, making it easy to analyze, visualize, or use for further research.

### Use Cases:
- **Market Research**: Analyze trends in the book industry by looking at best-selling books, most popular genres, and customer reviews.
- **Price Comparison**: Compare prices of popular books over time.
- **Customer Sentiment Analysis**: Scrape customer reviews to analyze sentiment on best-selling books.

This project serves as a basic example of how web scraping can be utilized to extract meaningful data from popular e-commerce platforms, and it can be adapted to scrape other categories or even different websites entirely.

The data extracted includes:
- Book Title
- Author
- Rating
- Number of Reviews
- Price
- Product Link

The final output is saved as a CSV file for further analysis and reporting.

## Features
- Web scraping of Amazon's Best Sellers page
- Data extraction and processing using Python libraries
- Automated saving of data in a structured CSV format

## Technologies Used

The following technologies were utilized in this project:

### 1. **Python**
   - The primary programming language used to build the web scraper.
   
### 2. **BeautifulSoup**
   - A Python library used for web scraping purposes to parse HTML and XML documents. It is used here to extract the product data from Amazon's Best Seller page.
   
### 3. **Requests**
   - A simple HTTP library for Python that is used to send requests to the Amazon webpage and retrieve the HTML content.

### 4. **Pandas**
   - A data analysis and manipulation library for Python, used to store, manage, and export the scraped data in CSV format.

### 5. **Jupyter Notebook**
   - An open-source web application used to run Python code interactively and showcase the web scraping project in a structured notebook format.

### 6. **CSV**
   - The format used for saving the scraped data, allowing easy export and use for further analysis.

### 7. **GitHub**
   - The platform used to host the project code, share it with others, and enable version control.


## Installation

To run the project, you need to install the required libraries. You can install them using pip:

```bash
pip install requests beautifulsoup4 pandas
```

## Usage

1. Clone the repository or download the notebook.
2. Run the notebook in a Jupyter environment.
3. Execute the code cells to:
   - Install dependencies
   - Import necessary libraries
   - Scrape Amazon's Best Seller Book list
4. The results will be saved in `amazon_products.csv`.

### Sample Output (CSV Format):

| Title | Author | Rating | Reviews | Price | Product Link |
|-------|--------|--------|---------|-------|--------------|
| Example Book 1 | Author 1 | 4.5 | 1000 | $19.99 | [Link] |
| Example Book 2 | Author 2 | 4.7 | 5000 | $24.99 | [Link] |

## Project Structure

```
Amazon-Best-Seller-Book-Scraper/
│
├── Best_Seller_Book_Amazon_Web_Scrapping_project.ipynb  # Jupyter notebook with the web scraping code
├── amazon_products.csv                                  # The CSV file with the scraped product data
├── README.md                                            # Project documentation
└── requirements.txt                                     # List of required Python packages
```

## Contributing

Feel free to fork the repository, create an issue, or submit a pull request. Contributions are welcome!


