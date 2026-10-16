# Orbit trading demonstration
A static, responsive trading dashboard. All prices, orders, balances, and profits are simulated. The baseline is an illustrative $68,432.50, not today's live BTC price. No APIs, database, real account, or exchange integrations.

Run locally with `python3 -m http.server 8000` from this directory, then open the local server in a browser. No installation or build step is needed.

The demo account starts with 20,000 USDT. An active timer alternates buys and sells every 60 seconds; sales are scripted to be profitable. Realized profits increase account equity. Prices stay between -5% and +10% of the baseline and return to it every five active minutes. The cycle preserves profits and history; Reset clears the session. Pause freezes the simulation. Refresh starts a new session. No data is saved. The chart updates each second; timeframe buttons aggregate display candles. Amounts and returns are illustrative, not investment results.

## GitHub Pages
The included workflow deploys pushes to `main`. In repository Settings → Pages, choose GitHub Actions as the source if deployment is not enabled automatically. The expected project URL is https://widchy95.github.io/3in1-Extract-Tool/ once deployment succeeds.
