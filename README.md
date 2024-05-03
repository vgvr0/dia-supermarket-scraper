# Web Scraping Dia Supermarket

This Python script utilizes web scraping techniques to extract product information from the DIA supermarket website.

---

## Requirements
- Python 3
- Selenium
- BeautifulSoup
- Chrome Web Driver
- SeleniumBase
---

#### Usage
1. Install the required Python packages.
2. Download and install the Chrome Web Driver. Make sure the Chrome Web Driver executable is in your system's PATH.
3. Run the script using Python.
4. 
---

#### Code Explanation

1. **Importing Libraries**: 
- The script imports necessary libraries such as `os`, `re`, `csv`, `time`, `random`, `sqlite3`, `keyboard`, `funcionesAux` (assumed to be a custom module), `datetime`, `BeautifulSoup`, and `seleniumbase`.

2. **Function Definition**:
- `dia_csv`: This function saves data to a CSV file.

3. **Setting Up WebDriver**:
- The script initializes a Chrome WebDriver instance.

4. **Scraping DIA Website**:
- The script navigates to the DIA website and accepts cookies.
- It scrapes product categories and subcategories, storing their URLs for further scraping.
- For each subcategory, it scrapes product details such as name, image, and link.

---

#### Example

Here's an example demonstrating how to use the script:

```python
from seleniumbase import Driver

driver = Driver(
 browser="chrome",
 uc=True,
 headless2=False,
 incognito=False,
 agent='Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36',
 do_not_track=True,
 undetectable=True
)

driver.maximize_window()

# Run web scraping script
# (Add web scraping code here)

driver.close()


