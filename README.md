
# 📚 Book Scraper

A web scraping project built in Python to extract detailed information about books from [Books to Scrape](https://books.toscrape.com). This site is specifically designed as a sandbox for practicing web scraping. The project demonstrates how to use `requests`, `urllib`, and `BeautifulSoup` to extract, parse, and structure data from web pages.

---

## 🧾 Project Overview

This project:
- Connects to the main page of the site.
- Extracts book entries (title, URL).
- Navigates to individual product pages.
- Parses and extracts key book details:
  - 📘 Title
  - 💰 Price
  - ⭐ Rating (converted from text to integer)
  - 📦 Availability
  - 📝 Product Description

---

## 🔧 Technologies Used

- **Python 3**
- `requests` – for sending HTTP requests
- `urllib` – for opening URLs
- `BeautifulSoup` – for parsing HTML content

---

## 📁 Project Structure

```
book-scraper/
│
├── books.ipynb          # Jupyter notebook containing the scraping logic
├── README.md            # Project documentation
└── books_details.csv    # output csv file
```

---


## 🧪 Sample Output

Here is an example of the kind of structured data you'll get from a book page:

```python
{
  "title": "A Light in the Attic",
  "price": "£51.77",
  "stars": 3,
  "availability": "In stock",
  "description": "It's hard to imagine a world without A Light in the Attic..."
}
```

---

## 📝 Notes

- Star ratings on the website are given as text classes (e.g., `"Three"`), which are converted to numeric (e.g., `3`) for easier analysis.
- The scraper only parses books listed on the homepage. You can expand it to include pagination and scraping across all categories.

---

## 📌 Legal & Ethical Disclaimer

This project is for **educational purposes only**. The website [books.toscrape.com](https://books.toscrape.com) is a dedicated test environment for web scraping and does not represent a real online bookstore.

---



