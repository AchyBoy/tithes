# Tithe Ledger

A one-page site for working out the tithe from a bank statement.

Paste a Chase activity export, it reads the rows, classifies each one against a
set of keyword rules, and works out what is owed. Months are kept on the JobHub
backend (`/api/tithes`) rather than in the browser, so a phone and a laptop see
the same ledger.

Everything is behind a password. Forgetting it mails a six digit code to the one
address the server knows.

- **Site:** achyboy.github.io/tithes
- **API:** `https://api.jobhubgo.com/api/tithes` (source in `jobhub-backend/src/routes/tithes.ts`)
- **Deploy:** a push to `main` publishes it. There is no build step.
