# Amazon Web Scraper Using Python

# [Publication](https://aljocastro.github.io/AmazonWebScrapper/)

In this project, I built a Python-based Amazon price tracker that automatically monitors a product’s price and sends an alert when it drops below a set threshold.
Using BeautifulSoup and Requests, the scraper connects to the product’s Amazon page, retrieves key details, cleans and structures the data, and logs timestamps for historical tracking. The script can run at scheduled intervals, making it a simple yet effective automation tool for deal hunting.

* Data Source: Amazon product pages
* Libraries Used: BeautifulSoup, Requests, smtplib (for email alerts)
* Functionality: Price scraping, timestamp logging, threshold-based email notifications
* Goal: Amazon Price Tracker to automate the process of tracking price drops for specific products
* Write-up: The complete walkthrough and code are published here

## Result: Amazon Price Tracker
This Amazon Price Tracker is a Python automation tool that monitors Amazon product prices and sends an email alert when the price drops below a defined threshold.
It uses BeautifulSoup and Requests to scrape live product data, logs each check with a timestamp for historical tracking, and leverages smtplib to deliver instant notifications.

Key Highlights:
  🔍 Web Scraping – Extracts product title, price, and other key details directly from Amazon product pages.
  ⏱ Scheduled Checks – Can run at set intervals to keep price data up to date.
  📊 Data Logging – Saves timestamps and price history, can be used for trend analysis.
  📧 Email Alerts – Notifies you instantly when the price drops below your desired limit.
  🛠 Tech Stack – Python, BeautifulSoup, Requests, smtplib
