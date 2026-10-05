# SVF–NPU Friendship Initiative

GitHub Pages frontend + Google Apps Script + protected Google Sheet.

## Setup
1. Create a Google Sheet in the secure NPU Drive/Shared Drive.
2. Extensions → Apps Script. Paste `apps-script/Code.gs`.
3. Replace `REPLACE_WITH_YOUR_GOOGLE_SHEET_ID`.
4. Run `setup()` once and authorize it.
5. Deploy → New deployment → Web app. Execute as **Me**. Choose the least-open access setting that works for both SVF and NPU students.
6. Copy the `/exec` URL.
7. In `index.html`, replace `YOUR_GOOGLE_APPS_SCRIPT_WEB_APP_URL` with that URL.
8. Push the repository to GitHub.
9. Repository → Settings → Pages → Source → GitHub Actions.

Student data is not stored in GitHub. The repository contains only frontend code. Staff matching data stays in the Google Sheet.

Before collecting real student data, have NPU IT/privacy/data-governance staff review access, retention, consent, and the Apps Script deployment settings.
