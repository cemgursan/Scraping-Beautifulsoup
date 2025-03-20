# BBC News Scraping Tutorial

This project demonstrates how to scrape news data from the BBC website using Python. It extracts news headlines, descriptions, timestamps, and locations (or news types) from the BBC News homepage, saves the data into an Excel file, and then processes the file with pandas to search for specific keywords.

## Overview

The notebook performs the following steps:

- **Web Scraping:**  
  Uses BeautifulSoup and urllib to fetch and parse the HTML content from [BBC News](https://www.bbc.com/news). It locates news elements by their HTML classes and extracts:
  - News Header
  - News Description (with a fallback if unavailable)
  - News Time (with error handling for missing timestamps)
  - News Type/Location

- **Data Storage:**  
  Saves the scraped news into an Excel file (`BBC News Scraping Tutorial.xlsx`) using the `openpyxl` library.

- **Data Processing:**  
  Loads the Excel file into a pandas DataFrame for further analysis. For instance, the notebook demonstrates how to search for news headlines containing a specific keyword.

## Features

- **Dynamic Scraping:**  
  Retrieves up-to-date news data from BBC News.
- **Error Handling:**  
  Accounts for missing descriptions, timestamps, or location data.
- **Excel Integration:**  
  Exports the scraped data to an Excel file and then imports it for processing.
- **Data Search:**  
  Provides an example of how to search the DataFrame for news items containing a specified keyword.

## Installation

### Prerequisites

- Python 3.7 or higher

### Dependencies

Install the required packages using pip:

```bash
pip install beautifulsoup4 openpyxl pandas
