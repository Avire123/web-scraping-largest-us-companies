# Web Scraping: Largest Companies in the United States by Revenue

A beginner-friendly Python web scraping project that extracts company information from a Wikipedia table and organizes the results into a Pandas DataFrame and CSV file.

## Project Overview

This project demonstrates an end-to-end web scraping workflow:

1. Send an HTTP request to a public webpage.
2. Parse the returned HTML with BeautifulSoup.
3. Locate and extract tabular company data.
4. Store the extracted records in a Pandas DataFrame.
5. Export the cleaned table to a CSV file.

## Data Source

**Source:** Wikipedia — List of largest companies in the United States by revenue

The notebook uses the public webpage as the source for the scraped table.

## Technologies Used

- Python
- Requests
- BeautifulSoup
- Pandas
- Jupyter Notebook

## Data Fields

The extracted dataset contains the following fields:

- `Rank`
- `Name`
- `Industry`
- `Revenue (USD billions)`
- `Employees`
- `Headquarters`

## Project Workflow

### 1. Import libraries

```python
from bs4 import BeautifulSoup
import requests
```

### 2. Request the webpage

A browser-style User-Agent is supplied with the request before downloading the webpage.

### 3. Parse HTML

BeautifulSoup is used with Python's `html.parser` to process the HTML returned by the website.

### 4. Extract table data

The relevant table rows and cells are extracted and converted into Python lists.

### 5. Create a DataFrame

The scraped records are stored in a Pandas DataFrame for structured analysis.

### 6. Export the data

The final dataset is exported as:

```text
Companies.csv
```

## Repository Structure

```text
web-scraping-largest-us-companies/
│
├── Scraping_Data_from_Website_Pandas.ipynb
├── Companies.csv
├── requirements.txt
├── README.md
└── .gitignore
```

## How to Run

### Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/web-scraping-largest-us-companies.git
cd web-scraping-largest-us-companies
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Launch Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
Scraping_Data_from_Website_Pandas.ipynb
```

and run the cells from top to bottom.

## Skills Demonstrated

This project demonstrates practical skills in:

- Web scraping
- HTTP requests
- HTML parsing
- BeautifulSoup
- Pandas
- DataFrame creation
- Data extraction
- Basic data engineering
- CSV data export
- Reproducible Python workflows

## Important Note

Web pages can change over time. Because this project extracts data from a live webpage, the scraped results may differ from the results obtained when the notebook was originally created.

Please respect the website's terms, robots.txt, rate limits, and applicable policies when adapting the scraper for other websites.

## Author

**Isaac Mcharo**

Data Analyst | Data Science Enthusiast

---

If you find this project useful, feel free to ⭐ the repository.
