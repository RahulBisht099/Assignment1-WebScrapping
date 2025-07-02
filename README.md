# 📅 CodeChef Upcoming Contests Scraper

This project scrapes upcoming contest information from [CodeChef](https://www.codechef.com/contests), stores it in a PostgreSQL database (such as [Neon.tech](https://neon.tech)), and exports the data to a CSV file. It handles JavaScript-rendered content using Selenium and BeautifulSoup.

---

## 🚀 Features

- Scrapes **dynamic data** (JavaScript-loaded) using Selenium
- Parses HTML content with **BeautifulSoup**
- Stores contests in a **PostgreSQL database** (Neon-compatible)
- Exports contest data to a **CSV file**
- Prints upcoming contests to the terminal

---

## 🔧 Tech Stack

- Python 3
- Selenium
- WebDriver Manager
- BeautifulSoup (bs4)
- psycopg2 (PostgreSQL connector)
- CSV module
- Jupyter Notebook / Python script

---

## 📦 How to Run

# 1. Clone the repository
git clone https://github.com/your-username/codechef-contest-scraper.git
cd codechef-contest-scraper

# 3. Install dependencies
pip install selenium webdriver-manager beautifulsoup4 psycopg2-binary

# 4. Run the scraper
python scraper.py

---

## 🛠️ How It Works

1. Launches a Chrome browser using Selenium
2. Navigates to `https://www.codechef.com/contests`
3. Waits for the page to fully load JavaScript
4. Parses the first table (upcoming contests) using BeautifulSoup
5. Prints the data on the screen
6. Saves the data to a PostgreSQL database (optional)
7. Exports the contest data to a CSV file

---

## 📝 Output Example

```
📅 Upcoming CodeChef Contests:

Name: CodeChef Starters 193 (Rated for all) (START193)
Start: 02 Jul 2025 | End: 02 Jul 2025
--------------------------------------------------
Name: Weekend Dev Challenge 05: JavaScript Projects (DEVWEEKEND05)
Start: 05 Jul 2025 | End: 06 Jul 2025
--------------------------------------------------
```

---

## 🛢️ PostgreSQL (Neon) Integration

Update your connection string in the script:

```python
dsn = "postgresql://<username>:<password>@<host>/<dbname>?sslmode=require"
```

---

## 📄 CSV Export

After scraping, a file named:

```
codechef_upcoming_contests.csv
```

will be generated in your current directory.

---

## 📁 Folder Structure

```
.
├── WebScrapping.ipynb
├── codechef_upcoming_contests.csv
├── README.md
```

---

## 🙋‍♂️ Author

**Rahul Singh Bisht**  
Built for learning and showcasing real-world Python web scraping.

---
