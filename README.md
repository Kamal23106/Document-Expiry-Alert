# 📧 Document Expiry Alert System

A Python automation tool that reads vehicle, license, and medical certificate expiry data from Word documents and sends email alerts **30 days before** the expiry date.


## 📌 Overview

The **Document Expiry Alert System** is a Python-based automation project that helps organizations track and manage important document expiry dates related to:

- ✅ Vehicle-related documents (Road Tax, Fitness, Permit, Pollution, Insurance)
- ✅ Driving License renewals
- ✅ Medical certificate validity (Eye, Fitness, Audiometry)

It scans structured `.docx` files, identifies dates that are either *about to expire* or *already expired*, and sends a categorized email alert to the concerned person.


## 🎯 Purpose

Managing expiry dates manually is time-consuming and error-prone. This tool automates the process and ensures that no document goes unnoticed by sending reminders in advance.


## ⚙️ Key Features

- 📂 Reads structured data from Word files (`.docx`)
- ⏳ Automatically checks for upcoming and expired dates
- 📧 Sends categorized summary email
- 🔒 Can be kept private or made public for reference
- 🕒 Customizable alert period for each document type


## 💼 Ideal Use Case

This tool is ideal for:

- 🏢 Transport & logistics companies
- 🚛 Fleet managers
- 👨‍💼 HR teams managing driver/employee certifications
- 📅 Any organization dealing with regular renewals


## 🛠 Technologies Used

- Python 3.x
- Libraries:
  - `python-docx` – to parse Word documents
  - `smtplib`, `email` – for sending emails
  - `datetime`, `re` – for date handling


## 📂 Folder Structure

document-expiry-alert/
├── main.py
├── requirements.txt
├── README.md
└── sample_data/
    ├── Driver_License_Record.docx
    ├── Driver medical, eye, Fitness Certificate.docx
    └── Due Date Taxes for vehicle.docx


## ▶️ How to Run

1. Install dependencies:
   	bash
   pip install -r requirements.txt
   
2. Update your email credentials in `main.py`

3. Run the script:
      bash
   python main.py
   

## 📬 Sample Email Output

🛑 Document Expiry Summary 🛑

🟡 Vehicle Documents Expiring in 30 Days:
• UP80BT1359 (Fitness): 30-06-2025

❌ Already Expired:
• UP80FT7375 (Insurance): 01-06-2024

🔵 License Expiring Soon:
• MR. VIKRAM (License No: UP8019750000500): 10-07-2025

🩺 Medical Certificates Expiring:
• Mr. RAJESH (Eye): 05-07-2025


## 👤 Author

  Kamal Kant Sharma
📧 kamalkant23105@gmail.com  
🌐 [GitHub Profile](https://github.com/Kamal23106)


## 📝 License

This project is open-source and free to use for personal or professional purposes.
