# Elegant Web Scraper Example (Scrapy)

This repository contains a simple yet powerful web scraping spider built with the Scrapy framework. It is designed to demonstrate an elegant and pythonic way to handle common scraping tasks, particularly automatic pagination.

The spider is configured to scrape quotes from the website `quotes.toscrape.com`.

## Key Features & Concepts Demonstrated

*   **Structured Data Extraction:** Utilizes Scrapy's powerful CSS selectors to precisely extract structured data (text, author, tags) from each page.
*   **Automatic Pagination Following:** Instead of manually constructing URLs for each page, the spider intelligently finds the "Next" page link and uses `response.follow` to create a new request, continuing the crawl automatically until the last page is reached. This creates a clean, robust, and scalable solution for multi-page websites.
*   **Declarative Approach:** The code embodies Scrapy's philosophy of "write the rules, not the process." The developer only needs to declare what to extract and how to find the next page, while the Scrapy engine handles all the complex underlying machinery like asynchronous requests, scheduling, and error handling.
*   **Clean & Readable Code:** The entire logic is contained within a single, easy-to-understand Spider class, making it a perfect example for learning and best practices.
