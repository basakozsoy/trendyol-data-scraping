# Trendyol Data Scraping

## Overview
This project is designed to scrape data from Trendyol to analyze top sellers' review information with a given URL. The data collected includes various details about products, reviews, and sellers, providing a comprehensive dataset for further analysis. 

## Features
- **Product Information:** Includes product prices and ratings.
- **Review Information:** Captures total rating counts, star ratings and their respective counts, text and images of reviews, and review dates.
- **Seller Information:** Collects details about the sellers.

It is possible to add more information by inspecting the website and the contents in HTML. However, additional information hasn't been included in the current implementation since it wasn't required.

## Implementation
The project was initially implemented using a Colab notebook, but this method has become outdated. A local script is now available, which utilizes parallel processing for improved performance. The local script is in the form of an IPython Notebook (.ipynb) file.

## Requirements
- Python 3.x
- Required libraries: BeautifulSoup, requests, pandas, numpy, concurrent.futures

## Installation
1. Clone the repository:
    ```bash
    git clone https://github.com/basakozsoy/trendyol-data-scraping.git
    ```
2. Run the local or Colab(Outdated) script.

## Usage
1. **Local Script (IPython Notebook):**
    - Ensure all dependencies are installed.
    - Open the local IPython Notebook file (`.ipynb`) in Jupyter Notebook or JupyterLab.
    - Define the base URL as `"https://www.trendyol.com/laptop-x-c103108?sst=BEST_SELLER&pi="`, set the end page variable like `end_page = 3`. You can also change the number of total workers for parallel processing by changing the `num_workers` parameter. 
    - Follow the instructions within the notebook to execute the cells and perform the scraping.

2. **Colab Notebook (Outdated):**
    - Open the Colab notebook provided in the repository.
    - Follow the instructions to run the cells and perform the scraping.

## To-Do List
- Add README and function descriptions
- Optimize infinite scroll function
- Perform sentiment analysis on comments

## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any enhancements or bug fixes.
