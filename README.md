
# 📬 Smart Invoice Extractor

**Automated Python App to Extract PDF Invoices from Gmail and Save to CSV**

---

## 🔧 Tech Stack

**Language:** Python 3.x  
**PDF Reader:** PyPDF2  
**Regex Parser:** re (Regular Expressions)  
**GUI:** Tkinter & ttk  
**Email Access:** imaplib, email  
**Data Handling:** pandas  
**Excel Writer (optional):** openpyxl  
**Logging:** logging module  
**Async Processing:** threading  
**Optional DB:** SQLite via sqlite3  

---

## 📁 Folder Structure

```
InvoiceExtractor/
│
├── ui.py                  # Main GUI application
├── invoice_app.log        # Auto-generated log file
├── extracted_data.csv     # Output CSV with parsed invoices
├── attachments/           # Folder to store PDF attachments
├── regex.py               # (Optional) key normalization logic
├── sql_connection.py      # (Optional) SQLite DB logic
├── README.md              # This file!
└── images/                # Screenshots for README (optional)
```

---

## 📦 Features

**✅ Secure email login using Gmail App Password**  
**✅ Downloads PDF invoices from inbox automatically**  
**✅ Extracts Invoice Number, Date, Vendor, Amount**  
**✅ Displays invoices in a table (Tkinter GUI)**  
**✅ Export extracted data to CSV**  
**✅ Error logging and duplicate detection**  
**✅ Optional SQLite support**  

---

## 🚀 How to Run

**1. Clone or Download the Repo**  
```bash
git clone https://github.com/yourusername/InvoiceExtractor.git
cd InvoiceExtractor
```

**2. Install Required Libraries**  
```bash
pip install pandas PyPDF2 openpyxl
```

**3. Setup Gmail App Password**  
For security, enable 2-Step Verification on Gmail and [generate an App Password](https://myaccount.google.com/apppasswords) to use in this app.

---

## 💻 How It Works

**1.** User enters Gmail and app password in GUI  
**2.** App connects to Gmail via IMAP and filters subject "invoice"  
**3.** PDF attachments are downloaded  
**4.** PyPDF2 extracts text → Regex extracts key data  
**5.** Data is shown in a table and saved to `extracted_data.csv`  

---

## 🖼️ Screenshot (Optional)

> *(Insert your screenshot image here)*

```markdown
![App Screenshot](images/app_ui.png)
```

---

## 📊 Optional: Report Generator

Use `pandas` to group data by month or vendor and generate:
- `monthly_summary.csv`
- `vendor_summary.csv`

Just ask if you want built-in code for this!

---

## 🪵 Logs

All actions and errors are saved in:

```bash
invoice_app.log
```

---

## 🙋‍♀️ Author

**Vishwa Vardhini**  
Open to collaborations | Drop a ⭐ if this helped you!

---

## 📄 License

**MIT License — Use it, modify it, ship it!**
