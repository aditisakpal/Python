# F1 Champions Web Scraping & SEO Word Storage Tool

##  Overview
This project is a **Python-based web scraping tool** that extracts data from Wikipedia's *List of Formula One World Champions* page. The script scrapes the F1 champions' data, stores it in a **SQLite database**, and provides **data visualization**. Additionally, it extends SEO capabilities by storing a dictionary of words from the scraped content in a database for analysis.

##  Features
- **Web Scraping**: Uses `BeautifulSoup` to extract F1 championship data from Wikipedia.
- **Data Storage**: Saves extracted data into a SQLite database for easy retrieval.
- **SEO Word Storage**: Extracts and stores unique words from the page for SEO analysis.
- **Data Export**: Option to save data as a CSV file.
- **Error Handling**: Implements exception handling for connection errors.
- **Data Visualization**: Uses `matplotlib` to generate bar charts of wins per season.
- **Scalability**: Can be extended to scrape additional F1-related statistics.

##  Installation

### 1️⃣ **Clone the Repository**
```sh
git clone https://github.com/yourusername/F1-Scraper.git
cd F1-Scraper
```

### 2️⃣ **Install Required Dependencies**
Make sure you have Python installed (`python --version` to check). Then, install dependencies:
```sh
pip install -r requirements.txt
```

**Requirements:**
- `beautifulsoup4`
- `requests`
- `pandas`
- `matplotlib`
- `sqlite3`

## 📜 Usage
### **Scraping and Visualization**
Run `scraping.ipynb` to scrape F1 champions' data from Wikipedia, store it in a SQLite database, and visualize the results.

### **SEO Keyword Extraction and Storage**
Run `seo_dict.ipynb` to extract unique keywords from the scraped content and store them in a SQLite database for SEO analysis.

### **Jupyter Notebook Usage**
If using Jupyter Notebook (`.ipynb`):
```python
!pip install -r requirements.txt
!jupyter notebook
```
Then open `scraping.ipynb` or `seo_dict.ipynb` and run the cells.

##  Data Visualization
The script generates a **bar chart** showing the number of wins per season for each champion.

##  SEO Word Storage
The tool extracts **unique words** from the Wikipedia page and stores them in a SQLite database. This can be used for **SEO keyword analysis**.

### **How It Works:**
1. The script extracts text from the Wikipedia page.
2. It **cleans** the text by removing stop words and special characters.
3. The **unique words** are stored in a SQLite database for analysis.

##  Error Handling
The script handles:
- Connection errors (`requests.exceptions.RequestException`)
- HTML structure changes (checks table headers dynamically)
- Empty data handling (skips invalid rows)

##License
This project is licensed under the **MIT License**.

##  Contributing
Pull requests are welcome! Feel free to improve functionality or optimize the script.


