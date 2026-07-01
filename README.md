# NoCloud

**Offline desktop business hub for small businesses** — manage clients,
inventory, invoicing, estimates, and reporting, all from one app. Your data stays
on your computer.

This repository hosts the **downloadable installers** for NoCloud. The source code
lives in a separate repository.

## Download & install

1. Open the **[latest release](https://github.com/GLevek89/NoCloud-Releases/releases/latest)**.
2. Download **`NoCloud-Setup-<version>.exe`** (Windows 10/11, 64-bit).
3. Run it and follow the installer. On first launch, a short setup wizard collects
   your business details.

> **SmartScreen note:** the installer isn't code-signed yet, so Windows may show a
> "Windows protected your PC" warning. Click **More info → Run anyway** to continue.

## Automatic updates

NoCloud checks here for new versions automatically — daily and at launch. When an
update is ready it downloads in the background; just click **Restart now** when
prompted. You can also check manually from **Settings → Software Updates → Check
for Updates**.

## What's inside

- **Clients** — contacts and per-client billing history
- **Inventory** — materials and service items with stock tracking and low-stock alerts
- **Invoices** — payments, HST, due dates, and overdue tracking
- **Estimates** — deposits and one-click convert-to-invoice
- **Reports** — revenue, HST charged, and receivables aging for any period
- **Backups & export** — automatic local backups and CSV export for your accountant
- **Light & dark themes**

## Privacy

NoCloud is offline-first. Your business data (clients, inventory, invoices,
estimates) lives in a local database on your machine and is never sent to a
server. The app's outbound network calls are limited to: checking this page for
updates, a one-time license-activation ping, and — only when you choose to send
them — in-app feedback and crash reports.

## License

[Apache-2.0](./LICENSE).
