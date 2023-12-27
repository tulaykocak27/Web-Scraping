# Web-Scraping
Python, bs4, Numpy, os

1.Import Libraries:

requests: For making HTTP requests to fetch web pages.
BeautifulSoup: For parsing HTML content.
pandas: For handling and manipulating data in tabular form.
os: Provides a way of using operating system-dependent functionality.
itertools.zip_longest: Groups the elements of several lists into tuples.

2.User-Agent Header:

HEADERS: A dictionary containing the User-Agent header to simulate a web browser request.

3.Scraping Image URLs:

Loops through 10 pages of the website, extracts image URLs and product names from the HTML, and appends them to the link_details list.
The image URLs are modified to ensure they start with 'https:'.

4.Downloading Images:

Currently commented out, but the code is prepared to download images. It iterates through the image URLs, fetches the images, and saves them to a local directory.

5.Scraping Product Details:

Iterates through the collected link_details and fetches additional details such as product names, prices, and brands.
Appends the information to separate lists (product_names, product_prices, product_brands).

6.Creating a DataFrame:

Uses pandas to create a DataFrame from the collected information.
The DataFrame has columns: "Product Name," "Product Brand," and "Product Price."

7.Saving to CSV:

Writes the DataFrame to a CSV file named "laptopsfirst10page_info.csv."

8.Notes:

The script assumes a specific HTML structure on the website, and class names may change over time.
Some parts of the code, like image downloading, are commented out and can be uncommented if needed.
