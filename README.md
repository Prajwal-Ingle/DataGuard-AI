# DataGuard AI
# Intelligent Data Quality Monitoring Dashboard

DataGuard AI is a Python-based data quality monitoring dashboard developed using Streamlit and Pandas. It helps users identify, analyze, and understand common data quality issues in customer datasets through automated validation checks, interactive visualizations, and actionable recommendations.

The application provides an overview of dataset health, making it easier to identify data problems before using information for business reporting, CRM operations, marketing campaigns, and data analysis.

## 1. Business Problem

Customer datasets frequently contain data quality issues such as missing values, duplicate records, invalid contact details, and inconsistent dates.

These issues can lead to inaccurate reports, unsuccessful customer communication, and unreliable business decisions.

DataGuard AI addresses this problem by automating common data validation checks and presenting the results through an interactive dashboard.

## 2. Key Features

- **CSV File Upload:** Upload customer datasets directly through the Streamlit sidebar.
- **Automatic Dataset Loading:** Loads a sample customer dataset when no file is uploaded.
- **Dataset Overview:** Displays total rows, columns, duplicate records, missing values, and an overall data quality score.
- **Missing Value Detection:** Identifies missing values across individual columns.
- **Duplicate Detection:** Detects duplicate records in the dataset.
- **Email Validation:** Identifies invalid email formats when an email column is available.
- **Phone Validation:** Checks phone number formats when a phone column is available.
- **Date Validation:** Identifies invalid or missing dates when a date column is available.
- **Interactive Visualizations:** Presents data quality issues through charts and visual summaries.
- **Quality Monitoring:** Provides a quality score and issue-focused dashboard views.
- **Actionable Recommendations:** Suggests cleanup steps based on detected data issues.
- **Modern Dashboard Interface:** Features a dark navy and teal interface with tabs, score panels, issue filters, and cleanup playbook cards.

## 3. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Streamlit | Dashboard development and user interface |
| Pandas | Data processing and analysis |
| CSV | Dataset input format |

## 4. Project Structure

```text
DataGuard-AI/
│
├── app.py
├── data/
│   └── sample_customer_data.csv
│
├── .streamlit/
│   └── config.toml
│
├── requirements.txt
└── README.md
```

## 5. Installation and Setup

### Prerequisites

- Python 3.10 or later
- pip package manager
- Git

### Step 1: Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/DataGuard-AI.git
cd DataGuard-AI
```

### Step 2: Create a virtual environment

```bash
python -m venv .venv
```

### Step 3: Activate the virtual environment

**Windows:**

```bash
.venv\Scripts\activate
```

**Linux / macOS:**

```bash
source .venv/bin/activate
```

### Step 4: Install dependencies

```bash
pip install -r requirements.txt
```

### Step 5: Run the application

```bash
streamlit run app.py
```

Open the local URL displayed in your terminal, usually:

```text
http://localhost:8501
```

## 6. Sample Dataset

The project includes a sample customer dataset containing 1,000 rows with intentionally introduced data quality issues.

This dataset allows users to explore the dashboard and understand its validation capabilities without uploading their own data.

Users can also upload their own CSV files through the application sidebar.

## 7. Deployment

DataGuard AI can be deployed using Streamlit Community Cloud.

1. Push the project files to a GitHub repository.
2. Sign in to Streamlit Community Cloud.
3. Connect your GitHub account.
4. Select the DataGuard AI repository.
5. Set `app.py` as the application entry point.
6. Deploy the application.

## 8. Future Enhancements

- Automated data cleaning and correction.
- Downloadable data quality reports.
- Additional configurable validation rules.
- Support for Excel and other data formats.
- Historical data quality monitoring.
- AI-assisted data quality recommendations.

## 9. Acknowledgements

This project is adapted from the open-source data quality monitoring dashboard:

Original repository: https://github.com/gabinthelab/data-quality-monitoring-dashboard

The application has been modified with a redesigned interface and additional presentation features. Refer to the original project's license for applicable usage and attribution requirements.

---

**DataGuard AI — Making customer data more reliable, one dataset at a time.**
