# GetMyCv Invoice Studio

Create, track and share invoices, quotations and receipts for GetMyCv, in the same navy and teal theme as [getmycv.github.io](https://getmycv.github.io).

- Overview dashboard with billed, collected, outstanding and overdue figures
- Editor with a live A4 preview, four templates, QR code, signature and PDF export
- Clients, and a service catalogue that matches the website's pricing (USD):
  - Packages: Starter ($14), Professional ($26), Premium ($53)
  - Add-ons: Express delivery ($9), Custom domain setup ($8), Extra revision round ($5), Portfolio maintenance for 1 year ($18)
- GetMyCv contact details, Sampath Bank account, payment terms and refund policy (from the website's Terms page) are filled in
- Numbering follows `GMC-INV-2026-0001`, `GMC-QUO-…` and `GMC-RCT-…`, in line with the website's `GMC-` order references
- Advance payments:
  - Record an advance on a quotation (25%, 50% or the full balance in one tap). The quotation is marked accepted and shows the advance and the balance payable
  - Converting the quotation to an invoice carries the advance over and deducts it from the balance due
  - Mark any invoice payment as an Advance or a Payment; documents show "Advance received" on its own line
  - Advance receipts, an "Advance received, not invoiced yet" reminder on the dashboard, and an Advance column in the CSV export
  - Advances count once in "Collected", even after they move from a quotation to its invoice
- Payments (card through Stripe, bank transfer and more), receipts, JSON backup/restore and CSV export

Everything is a single `index.html`, with the logo and icons in `brand/` (copied from the website). Data is stored in the browser only, so export a backup from Settings to move to another device.

Enable GitHub Pages on this repository (Settings → Pages → deploy from the default branch) and it will be served at https://getmycv.github.io/Invoice/.
