# PROJECT-1
Automated Invoice Processing System
Ever been buried under a pile of invoice PDFs from vendors?  
This Python-powered tool fetches them straight from your email, extracts the details, and logs them into a structured format like CSV — so you can stop copy-pasting and start analyzing.


BRAIN BEHIND :
Automated Invoice Processing System is designed to:
- 📥 Download invoice PDFs from your Gmail inbox
- 🔍 Extract key fields (Invoice Number, Date, Vendor, Amount)
- 🖼️ Display everything in a GUI table
- 📊 Export to CSV for bookkeeping, analysis, or audits
- 🧠 Handle duplicates and errors with built-in logging

TECH STACK:

| Purpose               | Tech Used              |
|-----------------------|------------------------|
| Language              | Python 3.x             |
| PDF Text Extraction   | PyPDF2                 |
| Pattern Matching      | `re` (Regular Expressions) |
| GUI                   | Tkinter & ttk          |
| Email Access          | `imaplib`, `email`     |
| Data Handling         | pandas                 |
| Excel Export (option) | openpyxl               |
| Logging               | logging module         |
| Async UI              | threading module       |
| (Optional) DB Storage | SQLite (via `sqlite3`) |


What's Inside?
📁 attachments/ # Auto-created to store downloaded PDFs
📄 ui.py # Main GUI logic
📄 regex.py # Field normalization logic
📄 sql_connection.py # DB interaction logic
📄 invoice_app.log # Log file with every action/error
📄 extracted_data.csv # Output of extracted invoice data












