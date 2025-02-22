# Daily Pennsylvanian Sports Headline Scraper

A Python-based web scraper that automatically collects the top sports headline daily from The Daily Pennsylvanian's sports section.

## Overview

This project modifies the [basic-git-scraper-template](https://github.com/jlumbroso/basic-git-scraper-template) to specifically track sports coverage from Penn's student newspaper. While the original scraper collected main headlines, this version focuses on sports content, providing a way to monitor Penn's athletic coverage over time.

## Modifications Made

1. **URL Modification**:
   - Original: `https://www.thedp.com`
   - Modified: `https://www.thedp.com/section/sports`

2. **HTML Element Targeting**:
   - Original: `find("a", class_="frontpage-link")`
   - Modified: `find("h3", class_="standard_link")`

## Key Features

- Daily automated scraping of top sports headlines
- JSON-based storage for historical tracking
- Logging system for monitoring scraper performance
- Error handling for reliable operation

## Technical Implementation

The scraper uses:
- BeautifulSoup4 for HTML parsing
- Requests library for web scraping
- Loguru for comprehensive logging
- JSON for data storage

## Getting Started

1. Clone this repository
2. Install requirements:
   ```bash
   pip install -r requirements.txt
