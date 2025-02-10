# Web Scraper for UDN Money News

## Overview
This Python script scrapes the latest financial news from the UDN Money website and saves the news content, including text and images, in a structured folder format.

## Features
- Extracts the latest news titles and links from UDN Money.
- Downloads and saves the full article text into a `contents.txt` file.
- Downloads and saves images from the article.
- Organizes news content in a folder named after the article title.

## Requirements
Ensure you have the following installed before running the script:

- Python 3.x
- Required Python libraries:
  - `requests`
  - `beautifulsoup4`
  - `re`
  - `urllib`
  - `os`
  - `time`

You can install the necessary packages using:
```bash
pip install requests beautifulsoup4
```

## Usage
1. Run the script in a Jupyter Notebook environment.
2. The script will scrape the latest financial news from UDN Money and save them in a `news/` directory.
3. Each news article will have its own folder named after its title, containing:
   - `contents.txt`: The full article text.
   - Image files: All images from the article.

## Notes
- The script includes a delay (`sleep(2)`) to prevent excessive requests.
- If an article title contains special characters, they may be removed to avoid file system errors.
- Ensure the target website's structure has not changed, as modifications may require updating the selectors.

## Disclaimer
This script is for educational purposes only. Scraping websites without permission may violate their terms of service. Always check the website's `robots.txt` file before scraping.

