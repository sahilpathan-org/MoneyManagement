# Paisa

Paisa is a private, browser-only personal expense tracker built with HTML, CSS, vanilla JavaScript, Chart.js, and jsPDF.

## Run in VS Code

Open `index.html` directly in a browser, or use the VS Code Live Server extension for a smoother development workflow. No backend, build step, or installation is required. Chart.js and jsPDF load from CDN, so charts and PDF export need an internet connection the first time they are used.

## LocalStorage

Expenses are saved under `paisa_expenses`, budgets under `paisa_budgets`, the light/dark preference under `paisa_theme`, and your display name under `paisa_user_name`. Data belongs to the current browser profile and never leaves the device unless you export it.

## Customize

- Categories and payment methods live in `script.js`.
- Main colors and responsive layout rules live at the top of `style.css` as CSS variables.
- Dashboard, reports, and PDF behavior live in `script.js`.

## Backup and restore

Open **Settings**, choose **Export JSON**, and keep the downloaded file somewhere safe. Choose **Import JSON** to restore it later. Importing replaces the current expenses and budgets with the backup contents.

## PDFs

Open **Settings & data** and choose Today's, Monthly, Yearly, or Custom range PDF. The generated report includes the selected period, totals, and an expense table. Custom reports ask for dates in `YYYY-MM-DD` format.