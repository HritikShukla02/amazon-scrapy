# amazon-scrapy


## **Project Description: Web Scraper for Amazon.in**

This web scraper is designed to extract comprehensive information on products listed on "https://www.amazon.in/" for a *particular searched keyword*. The main goal is to gather detailed data on listed products, including prices, URLs, ratings, brand, and special features listed. 


**Technologies Used:**
- **Scrapy**: A robust web scraping framework used to extract the data efficiently.

**Implementation Overview:**
- **Scrapy** is employed to structure the scraping process, define data extraction rules, and save the gathered information into a structured format like JSON or CSV.

**Benefits:**

- **Automated Data Collection**: Saves time and effort by automating the data extraction process.
- **Up-to-Date Information**: Ensures that the data is current, reflecting the latest prices and reviews.
- **Comprehensive Dataset**: Provides a detailed overview of hotels, aiding in market analysis, travel planning, or competitive research.

This web scraper is a powerful tool for anyone needing detailed and current information about hotel accommodations in a specific city from Booking.com.

### How to run:

- **Download the repository**:  
    - use command "git clone https://github.com/HritikShukla02/amazon-scrapy.git".

- **Create a virtual environment**
    - install virtualenv package: "pip3 install virtualenv"
    - creating a virtual env: "python3 -m  venv [name for your venv folder]"

- **Activate the virtual environment**:
    - Enter the folder *amazon-scrapy*.
    - if you are on Windows, run the command: "source [name for your venv folder]/Scripts/activate".
    - if you are on Linux or Mac, run the command: "source [name for your venv folder]/bin/activate".

- **Adding the API key to handle proxy**
    - You need to create an account on ScrapeOps.io and get your own API key to handle proxy.
    - Install python-dotenv package: pip3 install python-dotenv
    - create a file at the base directory of your project and name it **".env" **
    - Copy your API key from ScrapeOps.io and store it in this file in format: API_KEY="[YOUR API KEY]"
    - Save the file

-  **Enter the required details**: 
    - cd into amazon_scraper/amazon_scraper/spiders
    - Open amazon_spider.py
    - Update the *Keywords list* in start_request function.
    - Update the variable n_pages to specify number of pages you want to scrape the website for.
    - Save the file.

- **Run Spider**:
    - cd into the *spiders* folder.
    - run command: "scrapy crawl amazon_spider"


- **Output**:
    - This spider genetares a json file as the output that you can find in amazon_scraper folder..
    - Sample Output file "results.json" is also included in the repository.
