# [Amazon Web Scraper Using Python](https://aljocastro.github.io/AmazonWebScrapper/)

In this project, I built a Python-based Amazon price tracker that automatically monitors a product’s price. Using BeautifulSoup and Requests, the scraper connects to an specific web page, retrieves key details, cleans and structures the data. The script can run at scheduled intervals, making it a simple yet effective automation tool.

  * Data Source: Amazon product pages.
  * Libraries Used: BeautifulSoup, Requests.
  * Functionality: Web scraping, data extraction, data analysis.
  * Goal: Amazon Price Tracker to automate the process of tracking price drops for specific products.
  * Write-up: The complete walkthrough and code are published here


## Result: Amazon Price Tracker
This Amazon Price Tracker is a Python automation tool that monitors Amazon product prices and sends an email alert when the price drops below a defined threshold.
It uses BeautifulSoup and Requests to scrape live product data, logs each check with a timestamp for historical tracking, and leverages smtplib to deliver instant notifications.

Key Highlights:  
🔍 Web Scraping – Extracts product title, price, and other key details directly from Amazon product pages.  
⏱ Scheduled Checks – Can run at set intervals to keep price data up to date.  
📊 Data Logging – Saves timestamps and price history, can be used for trend analysis.  
📧 Email Alerts – Notifies you instantly when the price drops below your desired limit.  
🛠 Tech Stack – Python, BeautifulSoup, Requests, smtplib.

Flowchart:
    

  Start Price Tracker      ─▶ Send GET request to Amazon product page  ─▶  Parse HTML with BeautifulSoup  ─▶   Extract title & price 

                                                                                   Price < Threshold?
                                                                                      ┌─────┴─────┐
                                                                                     Yes          No
                                                                                      ▼           ▼
                                                                               ┌────────────┐   ┌─────────────────────┐
                                                                               │ Send Email │   │ Wait & Run Again    │
                                                                               │ Alert      │   │ (Scheduled Check)   │
                                                                               └────────────┘   └─────────────────────┘

