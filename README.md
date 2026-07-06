# NoCloud

**Offline desktop business hub for small businesses** — manage clients,
inventory, invoicing, estimates, expenses, and reporting, all from one app.
Your data stays on your computer.

This repository hosts the **downloadable installers** for NoCloud. The source
code lives in a separate, private repository.

## Download & install

1. Open the **[latest release](https://github.com/GLevek89/NoCloud-Releases/releases/latest)**.
2. Download **`NoCloud-Setup-<version>.exe`** (Windows 10/11, 64-bit).
3. Run it and follow the installer. On first launch, enter your license key,
   then a short setup wizard collects your business details (name, HST/tax
   number, logo, payment instructions) and lets you pick a business type.

> **SmartScreen note:** the installer isn't code-signed yet, so Windows may
> show a "Windows protected your PC" warning. Click **More info → Run
> anyway** to continue.

## Automatic updates

NoCloud checks here for new versions automatically — daily and at launch.
When an update is ready it downloads in the background; just click **Restart
now** when prompted. You can also check manually from **Settings → Software
Updates → Check for Updates**.

## What's inside

- **Dashboard** — at-a-glance revenue, outstanding balances, and recent
  activity for your business.
- **Clients** — contacts, per-client billing history, and a detail view for
  every account.
- **Invoicing** — invoices and estimates in one page (switch with a tab):
  payments, HST, due dates, overdue tracking, deposits, and one-click
  convert-estimate-to-invoice.
- **Counter Sale** — a fast, till-style checkout for walk-in or over-the-
  counter sales that still produces a proper invoice.
- **Inventory** — materials and service items with stock tracking, low-stock
  alerts, kit/bundle building, spreadsheet import, and — for parts-focused
  businesses — optional starter catalogs (U-bolts, center bolts, bushings,
  leaf springs).
- **Expenses & Transactions** — track outgoing expenses and see them combined
  with invoices in one transactions ledger.
- **Receivables** — an aging view of everything owed to you.
- **Reports** — revenue, HST charged, and receivables aging for any date
  range.
- **Notes** — a built-in notebook for anything that doesn't belong on an
  invoice.
- **Right-click actions everywhere** — right-click any row in any list
  (invoices, estimates, clients, inventory, expenses, notes, and more) for
  quick View, Edit, Print, Export, and Delete — no need to open the record
  first.
- **Bulk export** — filter invoices by status and export several as PDFs at
  once from **Send Invoices**.
- **Multiple business profiles** — run more than one business from the same
  install and switch between them.
- **Custom fields** — add your own fields to invoices, estimates, and
  products where the built-in ones aren't enough.
- **PDF invoice templates** — several layouts and accent colors, with a live
  preview before you send or print.
- **Light & dark themes**, adjustable density, and a rerunnable guided tour.
- **Bilingual** — full English and French (Canada) interface.
- **Backups & recovery** — automatic local backups plus one-click restore
  (see below).

## Security & data protection

NoCloud is built offline-first, and the data protections underneath it go
beyond "your data doesn't leave the machine":

- **Crash-safe saves.** The database runs in SQLite's write-ahead-log (WAL)
  journal mode, so every save is atomic — a crash or power loss mid-write
  cannot leave your database half-written or corrupted.
- **Automatic, validated backups.** A rolling backup is taken every time the
  app launches, in addition to on-demand manual backups. Every backup file is
  verified — integrity check, referential-integrity check, and a check that
  all required tables are present — before it's ever offered for restore.
- **Self-healing restore.** Restoring a backup first snapshots your current
  database; if the restored file fails validation or the app can't start
  from it, NoCloud automatically rolls back to exactly what you had before,
  rather than leaving you with a broken database.
- **Protected upgrades.** Every database schema upgrade (shipped with new
  app versions) takes an automatic safety snapshot first and rolls back
  automatically if the upgrade fails partway through.
- **Hardened app process.** The UI runs sandboxed and isolated from Node.js
  and the file system — it has no direct OS access. Every action it takes is
  routed through a narrow, explicitly whitelisted bridge to the app's backend.
- **Locked-down file access.** Internal guards block any in-app file
  operation from ever touching the live database, its journal files, or your
  license file outside of the intended backup/restore flow.
- **No plaintext license keys.** The app never stores or transmits your
  license key as plain text — only a one-way cryptographic hash of it is
  checked against an embedded allowlist.

## Privacy

NoCloud is offline-first. Your business data (clients, inventory, invoices,
estimates, expenses, notes) lives in a local database on your machine and is
never sent to a server. The app's outbound network calls are limited to:
checking this page for updates, a one-time license-activation ping, and —
only when you choose to send them — in-app feedback and crash reports.

## License

[Apache-2.0](./LICENSE).
