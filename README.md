# Christmas do pre-order

## 1. Google side (once)
1. Create a new Google Sheet.
2. Extensions > Apps Script, replace the code with `Code.gs`, and change `KEY` to something random.
3. Deploy > New deployment > type **Web app**. Execute as: **Me**. Who has access: **Anyone**. Authorise when prompted.
4. Copy the web app URL (ends in `/exec`).

If you edit the script later: Deploy > Manage deployments > edit > Version: New version. A "New deployment" gives you a new URL instead.

## 2. GitHub side
1. Paste the URL into `SCRIPT_URL` in `index.html`.
2. Push `index.html` to a new repo (`Code.gs` and this README can stay local).
3. Settings > Pages > Deploy from branch > `main` / root.
4. Submit a test order and check it lands in the Sheet, then delete that row.

## 3. Getting the data
- Use the Sheet directly, or File > Download > CSV.
- JSON: open `<web app url>?key=<your KEY>`.
