# 📈 Stock Scraper

A Python-based tool that scrapes historical stock data for a list of symbols from a finance website and calculates the **top 10 percentage gain days**. The results are saved directly into an Excel sheet.

---

## 🧠 Features

- 🌐 Scrapes publicly available stock data
- 🛡️ Cloudflare bypass using `cloudscraper`
- 📊 Calculates % gains over time
- 📁 Outputs top 10 gainers into Excel
- 📎 Supports bulk symbols via `.xlsx` file
- 💬 Beginner-friendly logs & structure

---

 ## 📦 Project Structure 
 ``` stock-scraper/ 

├── scraper.py # Main scraping script
├── stock_list.xlsx # Excel input file (auto-created if missing)
├── requirements.txt # Required Python packages
└── README.md # You're here! 

 ``` 
---

## 📥 Installation & Usage

 **1️⃣ Install Dependencies**

```bash
pip install -r requirements.txt
 ```
## 2️⃣ Add Stock Symbols

Open or edit the auto-generated Excel file stock_list.xlsx:
| Symbol |
|--------|
| AAPL   |
| MSFT   |
| TSLA   |
Place symbols in Column A, starting from row 2.

## 3️⃣ Run the Scraper
```bash
python scraper.py
 ```
This will fetch historical data, calculate gain %, and write top 10 gainers next to each symbol.

## 🖥️ Example Output (Excel)

| Symbol | Date 1     | Gain 1 | Date 2     | Gain 2 | ... |
|--------|------------|--------|------------|--------|-----|
| AAPL   | 2024-03-15 | 18.3%  | 2024-01-21 | 15.7%  | ... |
| MSFT   | 2024-02-10 | 16.1%  | 2024-01-05 | 14.4%  | ... |
| TSLA   | 2024-03-03 | 20.5%  | 2024-02-14 | 19.2%  | ... |

## ⚙️ Technologies Used

- **Python** – Core language
- **cloudscraper** – Bypass Cloudflare for scraping
- **beautifulsoup4** – HTML parsing and data extraction
- **openpyxl** – Excel file read/write

## ✅ Legal & Ethical Notes

> ⚠️ **Disclaimer:**  
> This script uses publicly available data from a generic finance website and is intended for **educational and personal use only**.  
> It is **not affiliated with, endorsed by, or connected to any official financial platform**.  
> Please ensure you comply with the website's terms of use and avoid overloading or violating any access rules.  
> Always use scraping tools responsibly.


## ⭐️ Support

If you liked this project:

- ⭐️ Star this repository  
- ✅ Follow me on [GitHub](https://github.com/Daud-Nisar)  
- 💬 Share your feedback or suggestions
