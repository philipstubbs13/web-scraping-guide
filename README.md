# Web Scraping Guide

- YouTube Video: <https://www.youtube.com/watch?v=XMu46BRPLqA>

* What is Web Scraping?

  - The process of extracting data from a website. When can use tools to automate this process. It is commonly used for research, analysis or any other purpose.

* Legal and Ethical Considerations

  - Web scraping can be a conversational topic. When scraping a website, you should consider the terms of that website. Some fully allow it. Some have stipulations and some do not allow it.

* History of Web Scraping

  - In 1993, the World Wide Web Wanderer was created, which was a bot that would go from link to link and index content.
  - This laid the groundwork for search engine web crawlers and data collection, which then led to web scrapers like Beautiful Soup in 2004.

* Why Use Web Scrapers?

  - Data Collection: Collect data from websites for research or analysis.
  - Price Monitoring: Monitor prices on e-commerce websites.
  - Content Aggregation: Aggregate content from blogs, news articles, etc.
  - Lead Generation: Collect contact info from websites for sales, marketing.
  - Market Research
  - Social Media Monitoring

* How Do Web Scrapers Work?

  - Web scrapers generally work by sending an HTTP request, downloading the HTML content and extracting the data that you want. You need to examine the HTML structure to get the dataa using a headless browser.

* Tools & Libraries

  - Puppeteer
  - Cheerio
  - Beautiful Soup

  * Scrapy
  * Selenium

* Basic Steps To Web Scraping

  - Identify the Website
    - Find the website and data that you want to scrape. Check legal considerations.
    * Inspect the Page
      - Inspect page with browser/devtools and examine the HTML structure around the data you want.
    * Write the Code
      - Write code to send a request and download the HTML and parse through and extract the data.
    * Run Code and Save Data
      - Run your code to extract data and save to a file or database for further consideration.

* Additional Steps and Considerations

  - Handle Pagination
    - If there is pagination, automate the process of clicking the links and scrape each page.
  - Dynamic Content
    - Some content is generated with JS. You can use tools like Puppeteer with headless browsers to handle this.
  - Handle Errors
    - Scraping can be error-prone, so you need to handle errors and make sure that your scraper runs smoothly.
  - Respect Robots.txt
    - Many websites use a robots.txt file which specifies which pages can be scraped and which can not.
    * Rate Limiting
      - To avoid overloading a website, you should add rate limiting to your scraper to limit the number of requests you send.

* Example site to scrape: <https://books.toscrape.com/>

```bash
python3 -m venv env
source env/bin/activate
pip install requests beautifulsoup4
python3 scrape.py
```
