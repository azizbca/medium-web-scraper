# medium-web-scraper
A scraper that collects articles from Medium using Selenium and BeautifulSoup

This project demonstrates a robust and dynamic web scraping workflow to extract article data from a continuously loading webpage, process the content, and store it in a structured format. Below are the key features and highlights of this project:

  Key Features:
  
Dynamic Content Handling:
The target page is dynamically loaded, requiring a scrolling mechanism to load all articles. Using Selenium, the script scrolls to the end of the page multiple times to ensure all content is fetched.

Multi-Link Data Extraction:
After extracting all article links from the page, the script iterates through each link to scrape the article content. BeautifulSoup is used to parse the HTML and extract the relevant information.

Automated Data Storage:
The scraped articles are saved as .docx files, with each file containing the article's paragraphs neatly formatted. The documents are organized into a dedicated folder for easy access and management.

Scale of Operation:  
The script successfully scraped 510 articles, showcasing its efficiency and ability to handle a large-scale scraping operation.


  Technologies Used:
  
Selenium: To handle JavaScript-heavy content and simulate user interactions like scrolling.
BeautifulSoup: For HTML parsing and data extraction.
Requests: To fetch HTML content from individual article links.
Python-docx: To create and save articles in .docx format.

  Challenges Addressed:

Dynamically loading pages required an effective scrolling mechanism to load new content incrementally.
Multiple article links were processed, with robust error handling to manage failed requests or unexpected content structures.
