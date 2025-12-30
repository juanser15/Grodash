# GroWise Dashboard (Streamlit) — Railway Deploy

## Run locally
```bash
pip install -r requirements.txt
streamlit run app.py
```

## Deploy on Railway (recommended)
1) Push this folder to GitHub as its own repo (or a subfolder repo).
2) In Railway: New Project → Deploy from GitHub → select the repo.
3) Ensure Railway detects Python (Nixpacks). This project includes `railway.json` that sets the start command automatically.
4) Once deployed, open the generated Railway URL.

### Notes
- Railway sets the port via the `$PORT` env var. The start command uses it.
- If you remove `data.xlsx` from the repo, the app will prompt users to upload NAV data in the sidebar.
- `Trades_2023__IBkr.xlsx` is optional; remove if you don't want it in the repo.
