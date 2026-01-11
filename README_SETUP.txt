CUSA FINAL BUNDLE

1) Install:
   pip install streamlit openpyxl bcrypt python-dateutil

2) IMPORTANT: configure email
   Open .streamlit/secrets.toml and replace:
   - SMTP_USER
   - SMTP_PASS (Gmail requires an App Password)
   - FROM_EMAIL

   Gmail App Password:
   - Enable 2-Step Verification on your Google account
   - Create an App Password for "Mail"
   - Put it into SMTP_PASS

3) Run the web app (from this folder):
   python -m streamlit run CUSA.py

4) Reminders (24h + 1h):
   Run reminder.py every 10 minutes using Task Scheduler (Windows) or cron (Mac/Linux):
   python reminder.py

Notes:
- Keep the Excel file CLOSED while the app is running (Excel locks the file).
- The app writes reservations into the same columns you already have, and adds tracking columns if missing.
