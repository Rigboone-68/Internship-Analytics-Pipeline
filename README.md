# 🚀Internship Analytics Pipeline
A centralized analytics and reporting system designed to automate data consolidation, visualization, and weekly reporting across multiple internship programs.
Built using Python (pandas, gspread, Google Sheets API) for backend automation and Looker Studio for real-time performance insights.

🧩 Problem Statement

Managing several internship programs through individual Google Sheets makes monitoring and reporting inefficient.
This project solves that by creating a single data pipeline that merges all tracking sheets, generates analytics dashboards, and automatically produces weekly reports for management review.

🧠 Solution / Implementation

The system extracts and merges data from multiple internship tracking sheets using Python and Google Sheets API, writes the consolidated data into a Master Sheet, and connects it to a Looker Studio dashboard.
Weekly performance reports are generated automatically using Python and exported as PDFs for department heads.

🎯 Objectives

Automate data consolidation from multiple internship trackers

Build a unified analytics dashboard for all programs

Generate weekly performance and engagement reports

Enable data-driven decision-making within internship management

⚙️ Tech Stack

Languages: Python
Libraries: pandas, gspread, google-auth, reportlab/pdfkit, matplotlib
Visualization: Google Looker Studio
Storage: Google Sheets (Master Data)
Automation: Cron / Python schedule library

🗂️ Project Structure
internship-analytics/
│
├── scripts/              # Python scripts for ETL and report generation
├── data/                 # Test or exported data (gitignored)
├── dashboard/            # Looker Studio design docs and screenshots
├── docs/                 # Project documentation
├── config/               # Sheet registry & credentials (gitignored)
├── requirements.txt
└── README.md

📊 Dashboard Overview

A dynamic Looker Studio dashboard connected to the master dataset displays:

Active interns & submission rates

Week-wise and team-wise trends

Country-level participation

Defaulters and late submissions

📅 Automation Workflow

Data Sync: Python merges internship data → updates Master Sheet.

Analytics: Looker Studio auto-refreshes metrics.

Reports: Python generates weekly PDFs with key highlights.

Delivery: Reports emailed automatically to department heads.

🧾 License

This project is licensed under the MIT License — you’re free to use, modify, and build upon it with proper credit.
