Job Lister fetches real job listings in India from the Adzuna Jobs API, saves them to an Excel file, and lets you browse, filter and save them in a Streamlit web app.

Built as a hands-on project to learn Python, Streamlit, Git and working with real APIs.

Features
Real job data: pulls Indian listings from Adzuna's official API (no risky scraping of job sites)
Excel storage: all listings are saved to jobs.xlsx
No duplicates: already-seen jobs are tracked in seen_jobs.txt, so only new jobs are added
Reset option: run with --reset to clear seen jobs and fetch everything again
Email notifications: get alerted about new listings

Tech Stack
Area	Tool
Language	Python
Frontend	Streamlit
Data source	Adzuna Jobs API
Storage	Excel (jobs.xlsx) via pandas / openpyxl
Config	.env file for secrets


Project Structure
job-lister/
├── scraper.py        # Fetches jobs from Adzuna and saves to jobs.xlsx
├── app.py            # Streamlit frontend
├── jobs.xlsx         # Generated job listings
├── seen_jobs.txt     # Tracks jobs already processed
├── requirements.txt  # Python dependencies
├── .env              # Your secret keys (NOT committed)
└── README.md
