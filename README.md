# PDFWorld

A light-theme PDF and document tools website built with Flask.

## Run locally

```bash
python -m pip install -r requirements.txt
python app.py
```

Open http://127.0.0.1:5000

## Publish free on Render

This project includes a Dockerfile that installs LibreOffice inside the server container, so users do **not** need to install LibreOffice and you do not need to keep your computer running.

1. Create a GitHub repository and upload the contents of this folder.
2. On Render choose **New → Web Service**.
3. Connect the GitHub repository.
4. Choose the **Docker** runtime / use the included Dockerfile.
5. Choose the **Free** plan.
6. Deploy.

Render gives the service a public `onrender.com` URL.

## Important free-tier notes

- Free Render web services sleep after inactivity and may take about a minute to wake.
- The filesystem is temporary, so this app treats uploads and generated files as temporary.
- Do not use the free tier for sensitive or high-volume production workloads without adding appropriate security, storage, and monitoring.

## Source code

- `app.py`: backend and conversion logic
- `templates/index.html`: homepage
- `templates/tool.html`: tool interface
- `static/style.css`: visual design
- `requirements.txt`: Python dependencies
- `Dockerfile`: production container, including LibreOffice
