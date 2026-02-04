## Pricing Scraper Challenge

Our competitor just launched a new store. We need to monitor their pricing, but they don't have a public API. We managed to save a copy of their search results page, and now we need to extract the data programmatically to feed into our pricing engine.


### Your Task
Write a Python script that reads `fake_store_page.html` and uses **BeautifulSoup** to parse product information and calculate pricing statistics.

### Rules
- **Required library:** `beautifulsoup4`
- Read from the local file `fake_store_page.html`
- Find all product cards
- Extract the product **Title**
  - Titles may contain extra whitespace or newlines
  - You must call `.strip()` on the title text
- Extract the **Price**
  - Price is split across multiple elements
  - Combine dollars and cents into a single `float`
- Check **Availability**
  - Ignore products marked `"Out of Stock"`
- Calculate the **average price** of in-stock items
  - Round the result to **2 decimal places**

### Goal
Correctly compute the average price of all **in-stock** items from the page.


### How to Run
```bash
python your_script_name.py
