# DataGuard AI – Deployment Guide

This guide explains how to deploy **DataGuard AI**, an intelligent data quality monitoring dashboard, using Streamlit Community Cloud.

## 1. Deployment Platform

**Recommended Platform:** Streamlit Community Cloud

Streamlit Community Cloud provides a straightforward way to deploy Streamlit applications directly from GitHub.

Platform: https://share.streamlit.io

## 2. Prerequisites

Before deployment, ensure that your GitHub repository contains the following files:

```text
DataGuard-AI/
│
├── app.py
├── requirements.txt
├── README.md
│
├── data/
│   └── sample_customer_data.csv
│
└── .streamlit/
    └── config.toml
```

## 3. Deploy Using Streamlit Community Cloud

Follow these steps to publish the application online.

### Step 1: Open Streamlit Community Cloud

Visit:

https://share.streamlit.io

Sign in using your GitHub account.

### Step 2: Create a New App

1. Click **Create app**.
2. Select **Deploy a public app from GitHub** or the equivalent repository deployment option.

### Step 3: Connect Your Repository

Select the following:

- **Repository:** Your DataGuard-AI GitHub repository.
- **Branch:** `main`.
- **Main file path:** `app.py`.

### Step 4: Configure and Deploy

1. Select Python 3.12 if the deployment settings offer a Python version selector.
2. Confirm the repository and entry-point details.
3. Click **Deploy**.

Streamlit Community Cloud will install the dependencies listed in `requirements.txt` and launch the application.

### Step 5: Access Your Application

Once deployment is successful, Streamlit will provide a public application URL.

You can share this URL with others to access DataGuard AI through a web browser.

## 4. Required Deployment Files

| File | Purpose |
|---|---|
| `app.py` | Main Streamlit application |
| `requirements.txt` | Python dependencies |
| `data/sample_customer_data.csv` | Default sample dataset |
| `.streamlit/config.toml` | Streamlit application configuration |

## 5. Important Notes

- Keep all required project files in their correct directory structure.
- Do not upload the `.venv` virtual environment folder.
- Do not commit `.streamlit/secrets.toml` or other files containing private credentials.
- Ensure that `requirements.txt` contains all required Python packages.
- The sample dataset is used when no CSV file is uploaded through the application.
- Changes pushed to the connected GitHub branch can be deployed through Streamlit Community Cloud.

**Free Hosting Note:** Streamlit Community Cloud applications may go to sleep after a period without traffic. This means free hosting does not guarantee uninterrupted 24/7 availability.

---

**DataGuard AI – Making customer data more reliable, one dataset at a time.**
