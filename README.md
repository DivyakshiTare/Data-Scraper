# Data-Scraper - EDGAR Collector

This project provides a Python script to collect company filings from the SEC EDGAR database. The script searches for companies based on specified keywords, retrieves their filings, and saves the data in a CSV file.

# Features

Search for companies on the SEC EDGAR database using keywords.

Retrieve recent filings (e.g., 10-K, 10-Q) for specified companies.

Rate-limited requests to comply with SEC guidelines.

Save the retrieved data to a CSV file for further analysis.

# Requirements

Python 3.7 or later

Libraries:

requests

pandas

dataclasses

typing

json

logging

time

datetime

pathlib

# Installation

Open Google Colab in your browser.

Upload the script to your Colab environment.

Install the required libraries by running the following commands in a Colab cell:

!pip install requests pandas

# Usage

Replace the email placeholder in the EDGARCollector initialization with your email address (e.g., example@gmail.com).

Update the search_terms and filing_types in the main function to suit your requirements.

Run the script.

# Steps to Run in Google Colab:

Upload the script file to your Colab environment.

Open the file in Colab.

Execute each cell sequentially, ensuring all dependencies are installed.

# Example Output

The script will save the collected filings in a CSV file in the output directory. The file name will include the current date, e.g., sec_filings_YYYYMMDD.csv.

# Notes

This script uses a 100ms rate limit to comply with SEC guidelines. Do not reduce the rate_limit below 0.1 seconds.

Ensure your User-Agent in the headers includes a valid email address to avoid request rejection by the SEC.

# Troubleshooting

If you encounter issues with dependencies, install them using !pip install commands in Colab.

Ensure your internet connection is stable.

Check the logs for detailed error messages if the script fails to fetch data.
