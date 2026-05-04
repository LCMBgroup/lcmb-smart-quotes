# Upload LCMB V7 Dashboard Estimator

1. Open the folder named `OPEN_THIS_FOLDER_UPLOAD_CONTENTS_TO_GITHUB`.
2. Upload the contents of that folder to the root of the GitHub repo, not the folder itself.
3. Commit message: `Upgrade LCMB smart selector to V7 dashboard estimator`.
4. Wait a few minutes for GitHub Pages to update.
5. Test: `https://lcmbgroup.github.io/lcmb-smart-quotes/smart-selector.html`.

## Important files

- `smart-selector.html` is the new app-style smart estimator.
- `assets/dashboard-v7.css` is the premium dashboard styling.
- `assets/dashboard-v7.js` is the interactive estimate logic.
- `assets/job-photos/` contains web-optimised LCMB photos.

## Current limitations

This is still a static GitHub Pages prototype. It can show the experience, calculate indicative ranges, build a summary and open an email, but it cannot securely save floor plans, send SMS, update GHL, update ServiceM8 or run AI by itself. Those steps should be added through GHL/Make/Zapier or a backend later.
