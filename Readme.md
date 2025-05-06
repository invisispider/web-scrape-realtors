# Realtor.com Agent Scraper


A Python **Python web scraping tool** with two ETL scripts that collect, clean, and export real estate agent data for a specified US state (Arizona in this example) from two sources: **Realtor.com** (via web scraping) and **eXp Cloud** (via API).

It navigates the site, extracts agent names, brokerage info, contact details, and compiles everything into a **structured Pandas DataFrame** or CSV for further analysis or outreach.

![realtor.com agent search](images/Screenshot_realtor.png)
---

## Features

✅ Scrape paginated agent listings across all AZ zip codes from Realtor.com  
✅ Extract agent names, contact details, and other metadata  
✅ Fetch agent data from the eXp Cloud API  
✅ Export cleaned, structured CSV files  
✅ Simple, modular scripts with clear outputs

---

## ⚙️ Tech Stack

- Python (BeautifulSoup, Requests)  
- Pandas (for data cleaning and export)  
- CSV / Excel export modules

---

## Requirements

- Python 3.x  
- Virtual environment (`venv`) or similar recommended

---

## Setup

1️⃣ Clone the repository:
```bash
git clone https://github.com/invisispider/web-scrape-realtors.git
cd web-scrape-realtors
```

2️⃣ Create and activate a virtual environment:
```bash
python -m venv myenv
source myenv/bin/activate  # Linux/macOS
myenv\Scripts\activate     # Windows
```

3️⃣ Install dependencies:
```bash
pip install -r requirements.txt
```

---


## Usage

### Realtor.com Scraper

This script loops through all Arizona zip codes and scrapes agent listings.

```bash
python az_realtors.py
```

- **Input:** List of AZ zip codes  
- **Process:** Paginated scrape → raw agent text → parsed fields  
- **Output:** `output_2nd_quest.csv`

⚠ **Note:** This script may no longer work if Realtor.com has updated its website or blocked automated scraping.

---

### eXp Cloud API Script

This script queries the eXp Cloud API and parses agent data.

```bash
python expcloud_az_realtors.py
```

- **Input:** eXp Cloud API endpoint  
- **Process:** API request → JSON response → parsed fields  

---

## 💼 Freelancing Demo

I build **custom data scraping solutions** for small businesses and professionals who need:  
- Bulk contact or listing data from public websites  
- Structured data feeds from online directories or marketplaces  
- Tools for market research, outreach, or competitive analysis

If you need to **turn web data into business insights**, I can design tools to automate and streamline the process.

---

## Contact

Want to collaborate or learn more?

- **GitHub:** [invisispider](https://github.com/invisispider)  
- **Upwork:** [My Upwork Profile](https://www.upwork.com/freelancers/~01527a09cdcfd75500)  
- **Website:** [steinunlimited.com](https://steinunlimited.com/)

---

## 🌐 My GitHub Portfolio

Check out my other highlighted projects:  
- [pdf-coa-to-csv](https://github.com/invisispider/pdf-coa-to-csv) – Python tools that read PDF test certificates  
- [web-scrape-realtors](https://github.com/invisispider/web-scrape-realtors) – Python web scraper for US realtors  
- [mfa-metrc-login](https://github.com/invisispider/mfa-metrc-login) – Automates Metrc MFA login with backup codes  
- [python-google-sheets-server](https://github.com/invisispider/python-google-sheets-server) – Flask server with Google API integration  
- [Stein-Unlimited](https://github.com/invisispider/Stein-Unlimited) – Personal Vue 3 web app with advanced features  
- [invisispider.github.io](https://github.com/invisispider/invisispider.github.io) – My portfolio site on GitHub Pages

--- 

## License

This project is for educational and personal portfolio purposes only. Be respectful of site terms and scraping ethics when using or modifying these scripts.

---
