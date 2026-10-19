# Finance Tracker

A personal budget app that runs entirely in your browser. Import CSV files from your banks, auto-categorize transactions, set monthly limits per category, and see clear dashboards and reports.

## Open it
Double-click **`index.html`** (Chrome or Edge recommended). Nothing to install.
The first open needs internet to load the CSV parser and chart library; after that your data loads from the browser.

## Monthly routine (5 minutes)
1. Download each account's CSV from your bank (see the **Import** page for where to find it).
2. **Import** → drop all the files at once. Overlapping dates are fine: duplicates are skipped.
3. Fix anything that landed in "Other". When you change a category, choose **Always** to create a rule so it's automatic next time.
4. Check the **Dashboard** alerts and **Budget** page. Adjust limits if needed.

## Tips
- **Import every account you use**: checking, savings, the GMR account and each credit card. Transfers between your own accounts and credit card payments are recognized and excluded from spending. If an account isn't imported, money sent to it looks like "saved" and the spending behind it is missing.
- **Back up** from Settings → *Download backup* now and then. Data lives only in this browser on this computer; clearing browser data erases it.
- Supported automatically: Chase checking/savings, Chase credit cards, Capital One, Discover. Any other bank works too: you match the columns once and it's remembered.

## Files
- `index.html`: the app
- `css/styles.css`: styles (light and dark themes)
- `js/`: storage (`db.js`), bank formats (`parsers.js`), auto-categorizing (`categorize.js`), calculations (`analytics.js`), and one file per page in `js/views/`
- `samples/`: made-up example CSVs for testing
