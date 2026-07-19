# NoCloud

NoCloud is an offline-first Windows desktop business hub for small businesses.
It brings clients, inventory, invoicing, estimates, receivables, expenses,
rent collection, notes, reporting, and backups into one application. Business
data stays in a local SQLite database on the user's computer.

This public repository contains the downloadable NoCloud installers and update
manifests. The source code is maintained separately in a private repository.

## Latest release

**Current version: [NoCloud v1.2.2](https://github.com/GLevek89/NoCloud-Releases/releases/tag/v1.2.2)**

- [Open the latest release](https://github.com/GLevek89/NoCloud-Releases/releases/latest)
- [Download NoCloud-Setup-1.2.2.exe](https://github.com/GLevek89/NoCloud-Releases/releases/download/v1.2.2/NoCloud-Setup-1.2.2.exe)
- Windows 10 or Windows 11, 64-bit
- Installer SHA-256: `111556001de7c6993f1d2f054e3f307c4cff3a53c07bb77e08fab99ac209f475`

NoCloud v1.2.2 adds an invoice design workspace in Settings with a live preview,
four templates, fifteen bundled offline fonts, custom colours, logo and paper
options, footer controls, and reusable design presets. The release did not add
a database schema migration, so existing v1.2.1 databases remain compatible.

> **Windows SmartScreen:** The installer is not code-signed yet. Windows may
> display “Windows protected your PC.” Choose **More info → Run anyway** only
> after confirming the installer came from this repository.

## Installation

1. Download `NoCloud-Setup-1.2.2.exe` from the release link above.
2. Run the installer.
3. Launch NoCloud and enter your license key.
4. Complete the setup wizard and choose the business model that matches your
   work.

## What NoCloud includes

- **Invoicing and estimates:** payments, HST, due dates, overdue tracking,
  deposits, holdback/progress billing, counter sales, and estimate conversion.
- **Invoice design:** four PDF layouts, live preview, bundled fonts, custom
  colours, logo placement, paper settings, footers, and saved presets.
- **Inventory:** products, materials, services, stock movements, low-stock
  alerts, kits, spreadsheet import, and optional parts starter catalogs.
- **Excavation and parts sales:** tailored inventory groups, service presets,
  receiving workflows, and parts-focused starter catalogs.
- **Rental locations:** properties and units, tenant assignment, monthly or
  weekly rent schedules, due/late status, and rent-payment recording.
- **Expenses and transactions:** HST extraction, vendor memory, quick entry,
  stock-receipt expense linking, and a combined transaction ledger.
- **Receivables and reports:** aging, revenue, HST, rental income, printable
  summaries, and date-range reporting.
- **Exports:** CSV list exports, client statements, batch invoice PDFs,
  accountant-ready XLSX packages, and full-data exports.
- **Multiple business profiles:** keep separate businesses in one installation
  and switch between them.
- **English and French (Canada):** full bilingual interface.
- **Light and dark appearance:** selectable themes, density, and a rerunnable
  guided tour.

## Automatic updates

NoCloud checks this repository for updates at startup and periodically while the
application is running. Update packages download in the background and install
only after the user accepts the restart prompt. Automatic update checks can be
disabled from **Settings → About**.

Each published release should contain:

- `NoCloud-Setup-<version>.exe`
- `NoCloud-Setup-<version>.exe.blockmap`
- `latest.yml`

## Data protection

NoCloud is designed around a local, user-owned database:

- SQLite transactions and write-ahead logging protect normal saves.
- Rolling automatic backups and manual backups are supported.
- Backups are validated before restore.
- Restore takes a safety snapshot first and rolls back if validation fails.
- Database migrations require a pre-update snapshot and restore the previous
  database if migration fails.
- Existing invoices, clients, payments, stock movements, and expenses are not
  stored in this repository.

NoCloud is offline-first. Network access is limited to update checks, license
activation, opt-in multi-device features on the user's own network, and feedback
or crash reports only when the user chooses to send them.

## Release policy

A feature is not available to users until a versioned release with all three
required update assets is published here. Development branches and draft source
pull requests are not release builds.

## License

[Apache-2.0](./LICENSE)
