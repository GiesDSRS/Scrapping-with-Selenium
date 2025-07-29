# Scrapping-with-Selenium

## Overview

This repository contains a Jupyter notebook for automating web scraping of educational policy documents from Nexis Uni using Selenium WebDriver. The notebook is designed to search for educational policies related to Illinois, authenticate using UIUC credentials, and download the search results.

## Features

- Automated login to Nexis Uni using UIUC credentials
- Search functionality for educational policies in Illinois
- Automated selection and download of search results
- Rate limiting to respect Nexis Uni's usage policies
- Support for 2-factor authentication

## Files

- `Selenium-Scrapping.ipynb`: Main Jupyter notebook containing the scraping logic
- `requirements.txt`: Python package dependencies
- `Nexis-Scrapping.zip`: Archive of downloaded files (generated during execution)
- `Pdfs - Educational Policies Illinois/`: Directory containing downloaded PDFs

## Requirements

You will need to have/install Chrome for testing (https://googlechromelabs.github.io/chrome-for-testing/), as it is required for this automation.

For notebook `Selenium-Scrapping.ipynb` to run properly, it is necessary to create a `.env` file and add:

- **usr**: Illinois email you normally use to log in to UIUC
- **psw**: Password for UIUC

** -or- ** hard-code these in the notebook (handle your credentials with caution!).

### Libraries needed:

- selenium
- python-dotenv

You can install these libraries in the notebook using pip install, or by running in the terminal:

```
pip install -r requirements.txt
```

## Usage

1. Clone this repository
2. Install the required dependencies
3. Create a `.env` file with your UIUC credentials
4. Open and run the `Selenium-Scrapping.ipynb` notebook
5. Monitor the download process and approve 2FA when prompted

## Important Notes

- The script assumes you have access to UIUC's Nexis Uni subscription
- This script respect Nexis Uni's terms of service and usage limits
- The script includes rate limiting to avoid overwhelming the service
- Handle your credentials with caution - consider using environment variables!
