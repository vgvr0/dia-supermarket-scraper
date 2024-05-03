# Project Overview

This project is designed to scrape product information from the Spanish supermarket chain Dia's website, specifically from the "Charcuterie and Cheeses" category. The script uses Selenium WebDriver to interact with the website and BeautifulSoup for parsing HTML content.

## Script Functionality
The script starts by initializing a Selenium WebDriver instance with specific browser settings and then navigates to the specified URL. It then accepts cookies and iterates over each category, clicking on each one and extracting the subcategories. For each subcategory, it extracts the product links and then navigates to each product page to gather information such as title, image URL, and prices.

## Script Output
The script outputs a list of product links, along with their corresponding information, in the console. The output includes the title, image URL, and prices for each product.

## Script Configuration
The script can be configured by modifying the following variables at the top of the script:
browser: The browser to use for the script. Currently set to "chrome".
uc: Whether to use an incognito browser session. Currently set to True.
headless2: Whether to run the browser in headless mode. Currently set to False.
agent: The user agent string to use for the browser. Currently set to a generic Chrome user agent.
do_not_track: Whether to set the browser's do not track preference. Currently set to True.
undetectable: Whether to set the browser's undetectable preference. Currently set to True.

## Script Execution
To run the script, simply execute the Python file. The script will output the product information to the console.

## Script Limitations
The script is designed to work with the specific website and category specified in the URL. It may not work with other websites or categories without modification.

## Script Maintenance
The script is designed to be easy to maintain and update. Simply modify the script configuration variables or update the script to work with new website changes.
