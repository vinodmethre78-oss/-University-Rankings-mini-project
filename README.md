# Top University Rankings 2024

A Flask web application for browsing, searching, and managing university ranking data. The project uses SQLite for storage and HTML/CSS/JavaScript for the interface.

## Requirements

- Python 3.10 or newer
- Git (for GitHub upload)

## Run locally on Windows (VS Code)

1. Extract this folder and open it in VS Code. Make sure the folder containing `app.py` is open.
2. Open **Terminal → New Terminal**.
3. Create a virtual environment:

   ```powershell
   python -m venv .venv
   ```

4. Activate it:

   ```powershell
   .\.venv\Scripts\Activate.ps1
   ```

   If PowerShell blocks activation, use Command Prompt and run `.venv\Scripts\activate.bat`.

5. Install dependencies:

   ```powershell
   python -m pip install --upgrade pip
   python -m pip install -r requirements.txt
   ```

6. Start the application:

   ```powershell
   python app.py
   ```

7. Open http://127.0.0.1:5000 in your browser. Stop the server with `Ctrl+C`.

## Project structure

- `app.py` — Flask application
- `requirements.txt` — Python dependencies
- `data/university_rankings.db` — SQLite database
- `templates/` — HTML templates
- `static/` — CSS, JavaScript, and images

## Upload to GitHub

Create a new **empty** repository on https://github.com/new (do not initialize it with a README). Then open a terminal in this project folder and run:

```powershell
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPOSITORY.git
git push -u origin main
```

Replace the URL with the HTTPS URL of your own GitHub repository. GitHub may ask you to sign in in a browser.

For later changes, run:

```powershell
git add .
git commit -m "Update project"
git push
```

## Notes

- `.gitignore` excludes virtual environments, local `.env` files, and Python cache files.
- The SQLite database is included so the project can use its existing data.
- Do not commit passwords, API keys, or real secret values.
