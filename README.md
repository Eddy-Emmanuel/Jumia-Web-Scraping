# Jumia Web Scraper for Product Information

This Python script utilizes web scraping techniques to extract product information from Jumia, a popular e-commerce platform. The script scrapes details such as product name, old and current prices, discounts, ratings, and the number of votes for a given keyword search.

## Prerequisites

- Python 3.x
- Required Python libraries: `numpy`, `pandas`, `chromedriver_binary`, `beautifulsoup4`, `selenium`

## Setup

1. Install the required libraries:

   ```bash
   pip install numpy pandas chromedriver-binary beautifulsoup4 selenium
   ```

2. Ensure you have Chrome installed, as the script uses ChromeDriver for web scraping.

## Usage

```python
from jumia_web_scraper import main

# Specify the keyword, number of pages to scrape, and discount threshold
keyword = "Iphone case"
pages_to_scrape = 5
discount = 10

# Run the main function to get the scraped data
result_df = main(keyword, pages_to_scrape, discount)

# Display the resulting DataFrame
print(result_df)
```

## Parameters

- `keyword`: The search term for Jumia products.
- `pages_to_scrape`: The number of pages to scrape for each search term.
- `discount`: The discount threshold for filtering products.

## Output

The script returns a Pandas DataFrame containing the extracted product information. The DataFrame includes columns for product name, old price, current price, discount, rating, number of votes, and image link.

## Disclaimer

Web scraping may violate the terms of service of the targeted website. Ensure compliance with Jumia's policies when using this script.

## Contribution Guidelines

If you encounter issues or want to contribute to the project, follow these guidelines:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and ensure code quality.
4. Submit a pull request with a clear explanation of the changes.

## License

This project is licensed under the MIT License.

## Acknowledgments

- The script uses BeautifulSoup and Selenium for web scraping, providing a convenient way to extract product information from Jumia for analysis or research purposes.
