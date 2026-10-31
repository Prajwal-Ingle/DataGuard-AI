# Deployment Guide

This Streamlit app is ready to deploy online. The recommended path is Streamlit Community Cloud because this project already uses Streamlit and has a simple file structure.

## Recommended: Streamlit Community Cloud

1. Push this project to a GitHub repository.
2. Go to `https://share.streamlit.io`.
3. Create a new app.
4. Select the GitHub repository and branch.
5. Set the app entrypoint file to:

```text
app.py
```

6. Deploy the app.

Streamlit Community Cloud will install packages from `requirements.txt` and run the app automatically.

## Alternative: Render

This project also includes `render.yaml` and a `Procfile`.

1. Push this project to GitHub.
2. Create a new Render web service from the repository.
3. Render can use the included `render.yaml`, or you can enter these manually:

```text
Build Command: pip install -r requirements.txt
Start Command: streamlit run app.py --server.port=$PORT --server.address=0.0.0.0 --server.headless=true
```

## Files Required for Deployment

```text
app.py
requirements.txt
data/sample_customer_data.csv
.streamlit/config.toml
```

## Notes

Do not commit `.streamlit/secrets.toml` if you add private credentials later. This app currently uses only local sample data and uploaded CSV files, so no secrets are required.
