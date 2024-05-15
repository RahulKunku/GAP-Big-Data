README: SEC 10-K Filing Scraper
This Python script is designed to scrape 10-K filings from the U.S. Securities and Exchange Commission (SEC) website for a list of company names. It utilizes the requests library to fetch web pages, pandas for data manipulation, and randomization techniques to mimic human-like browsing behavior. Before running the script, make sure you have installed the required libraries such as pandas, numpy, and requests.

Prerequisites
Before using this script, ensure you have the following prerequisites:

Python 3.x installed.
Required Python libraries installed (pandas, numpy, requests).
How to Use
Follow these steps to use the script:

Update the name_of_stock list with the names of the companies for which you want to scrape 10-K filings.

Customize the headers_list with User-Agent headers to mimic different web browsers and improve the scraping process.

Run the script using Python:

bash
Copy code
python your_script_name.py
The script will fetch 10-K filings for the specified companies, scrape relevant information, and save it to a CSV file named '10K Links.csv' in the same directory.
Script Overview
Here's a brief overview of what the script does:

Constructs URLs for each company in the name_of_stock list.

Randomly selects User-Agent headers to mimic human-like browsing behavior.

Fetches the initial web page for each company and extracts relevant information such as filing types, dates, company names, and links to the 10-K filings.

If the 10-K filings are not found on the initial page, it follows the link to the documents page and extracts the link to the first document.

The script saves the collected data into a pandas DataFrame and exports it to a CSV file.

The script also incorporates random sleep intervals to avoid overloading the SEC website and being blocked.

Caution
Please be mindful of the SEC's terms of use and scraping policies when using this script. Excessive or unauthorized scraping may lead to IP blocking or other restrictions.

Note
This script was created based on the knowledge available up to September 2021. Any changes to the SEC website or its structure may require adjustments to the script.

Always ensure that your web scraping activities comply with legal and ethical standards and respect the website's terms of service.

Make sure to handle any potential errors or exceptions gracefully, especially if running the script on a large list of companies, as network issues or website changes can lead to unexpected behavior.

This script is a basic example and can be extended or improved for more robust web scraping tasks.