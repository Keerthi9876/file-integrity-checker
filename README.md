# 🛡️ File Integrity Checker with Email Alerts

This project is a File Integrity Checker built using Python. It helps keep track of any changes (like if a file is added, modified, or deleted) in a folder on your computer. If any change happens, it shows it in the terminal with color highlights and also sends you an email alert!

## 👩‍💻 Developer Info

 Name: Keerthi Atthur
 Intern ID:CT06DG1276
 Internship Domain: Cyber Security & Ethical Hacking  
 Company: CodTech IT Solutions  
 Mentor: Neela Santosh  
 Internship Duration: 6 Weeks  

## 📌 What Does This Project Do?

This tool checks the files in a folder and makes sure they are not changed or deleted without permission. It uses something called SHA-512 hashing** to remember the original state of the files. If anything changes later, it will let you know through an email alert and also keeps a log in a file.

## 🔍 Main Features

  ✅ Shows files that are added, changed, or deleted
  ✅ Uses colors to highlight the changes in the terminal
  ✅ Sends an email alert when a file is modified
  ✅ Saves all events in a log file
  ✅ Easy to use with a simple menu



## 🔧 Tools & Requirements

You need the following:
   Python 3
 A few Python libraries:
    bash
  pip install colorama

  🛠️ Setup

Clone the repo

git clone https://github.com/keerthi9876/file-integrity-checker.git cd file-integrity-checker Configure email credentials Edit the top of integrity_checker.py:

EMAIL_ADDRESS = "keerthiatthur@gmail.com" EMAIL_PASSWORD = "lnmbycobsqxtekyg" EMAIL_TO = "keerthreddy7@gmail.com"

📌 Gmail Users: Create an App Password here:

https://myaccount.google.com/apppasswords

(Optional) Customize the monitored directory Default is ./Files, but you can change it in the code.

🚀 Usage
Run the script:
python integrity_checker.py Menu options:
Generate baseline
Check file integrity
Exit 1: Creates baseline.txt storing file hashes
2: Checks directory for changes, logs results, sends email alerts

3: Exits the script

📁 Output Files

integrity_checker.py: Main script

baseline.txt: Stores initial file hashes

integrity_log.txt: Change logs

./Files/: Default monitored folder

📩 Email Alerts

Triggers: File added, modified, or deleted
Email Subject: File Integrity checker 
Email Body: Affected file path

🔐 Security Tips

Do not commit your email credentials to GitHub
Use .env files or OS environment variables for safety
Use TLS with port 587 when using SMTP

🧠 Future Enhancements

Add dark mode for GUI
Integrate with Telegram alerts
Upload logs to Google Drive or Dropbox
Add hash comparison history
