# Web-Crawling-Scraping

This Python script is designed to extract company information, image URLs, and descriptions from a specific website. It performs web scraping and crawling operations to collect the data, saves it into a Pandas DataFrame, and then stores it as a local file.

## Libraries Used

+ **requests:** Used for making HTTP requests.
+ **os:** Used for file and directory operations.
+ **io:** Used for input/output operations.
+ **pandas:** Used for data processing and analysis.
+ **PIL (Python Imaging Library):** Used for image processing.
+ **BeautifulSoup:** Used for parsing HTML and XML files.

## Script Workflow

+ **Collecting URLs and Extracting Company Information:** In the first step, requests and BeautifulSoup are used to collect company URLs from a specific website. Then, necessary information for each company (e.g., name, address, phone number) is extracted and stored in a dictionary data structure.

+ **Downloading Company Images:** Necessary URLs to access each company's image are identified. Subsequently, these images are downloaded using requests and saved to a specific folder.

+ **Creating a Data Frame:** The collected company information is transformed into a data frame. This data frame is used to store company information sequentially.

+ **Data Processing and Editing:** Some columns in the data frame are edited, and data types are processed. For example, phone numbers are formatted, and city/district information is separated.

+ **Data Storage:** Processed data is written to a Parquet file, and company images are saved to a specific folder.

## Sample Usage

To run the script, follow the steps below:

+ Execute the script file.
+ Specify the URL from which you want to fetch company information and images.
+ The script will retrieve, process, and save the data from the specified website into a Parquet file and folder.
