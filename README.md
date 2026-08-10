<div align="center">

# NoCloud

### A practical Windows workspace for small businesses.

This is the official download page for NoCloud. The application keeps
day-to-day business records in one place and stores them on the Windows
computer where NoCloud is used.

### [Download NoCloud for Windows](https://github.com/GLevek89/NoCloud-Releases/releases/latest)

Windows 10 or Windows 11 · 64-bit · A NoCloud license key is required

</div>

[![NoCloud dashboard](assets/screenshots/dashboard-dark.png)](assets/screenshots/dashboard-dark.png)

*NoCloud shown with fictional demonstration data.*

## New in NoCloud 1.8.3

NoCloud 1.8.3 makes routine attention messages calmer and keeps stock tools
focused on items that are actually kept in stock.

- **Calmer attention messages:** overdue balances, rent due, and stock that
  needs attention use subtle amber markers and clear wording instead of turning
  whole amounts or messages red. Red remains reserved for errors and
  destructive actions.
- **Clearer item setup:** Add Item opens the complete form, returns you to where
  you started, and asks you to choose when a group allows several item types.
- **Safer stock updates:** Stock Update shows only stock-tracked items and uses
  plain actions: Receive, Correct count, and Remove manually. NoCloud also
  explains that invoices and counter sales already reduce stock.
- **Stock tools stay with stock items:** services, rental units, deposits, and
  other items not kept in stock no longer show stock controls or count toward
  stock value or stock alerts.
- **Simpler inventory:** the main filters focus on stock that needs attention,
  value at cost includes stock-tracked items only, and unused setup groups stay
  out of the way.
- **Clearer report reminder:** Reports quietly explains that its totals depend
  on the records entered in NoCloud and should be reviewed before filing or
  making a business decision.

Updating from 1.8.2 keeps your activation, businesses, records, document
numbers, backups, settings, inventory quantities, and stock-movement history.
This update does not rewrite existing inventory records or change the database
schema, local data location, or invoice, payment, HST, expense, or profit
calculations.

## What NoCloud does

NoCloud keeps related work together. A client can move from estimate to invoice
and payment without entering the same details again. Expenses, inventory,
amounts owed, and reports remain available from the main menu.

- **Sales and clients:** client records, estimates, invoices, counter sales,
  payments, statements, and customizable invoice PDFs.
- **Profit estimates:** a monthly estimate on Dashboard and Reports, plus an
  internal estimated gross profit on each invoice when costs are entered.
  These figures are not shown on customer PDFs.
- **Expenses and HST:** single expense entry, multi-receipt entry, receipt
  totals, amounts before HST, HST, vendor memory, and a combined transaction
  list.
- **Money owed:** outstanding and overdue invoices, aging, balances, printable
  summaries, and client statements.
- **Inventory and services:** products, materials, services, quantities, stock
  movements, low-stock notices, kits, receiving, and spreadsheet imports.
- **Reports and exports:** revenue, receivables, expenses, HST, rental income,
  invoice PDFs, CSV files, and accountant-ready Excel packages.
- **Different business setups:** separate workspaces for General Business,
  Excavation and Parts Sales, and Rental Locations. The interface is available
  in English and French.

## Search and filters

Search and filters are available throughout the main workspaces. Inventory can
be narrowed by stock condition, category, type, and business-specific group.
Invoices and estimates can be filtered by status, and rental units by occupancy.
Filtered lists can be exported where an export option is shown.

## SuperBatch (Beta)

SuperBatch is for importing a large table of expenses or deposits:

- Paste a table from Excel or select an XLSX, CSV, or TSV file.
- Review the columns NoCloud recognizes and correct the mapping when needed.
- Keep every source row visible, including malformed, ambiguous, ignored, and
  excluded rows.
- Resolve repeated category and account values once.
- Review possible duplicates before anything is saved.
- Compare row counts, totals with HST, amounts before HST, and HST with the
  source.
- Save the import as one batch and undo the complete batch afterward if needed.

SuperBatch is marked **Beta** in NoCloud. Its reconciliation totals should be
checked before committing a live import.

## More screens

These screens also use fictional demonstration data.

| Invoicing | Expenses |
| --- | --- |
| [![NoCloud invoicing](assets/screenshots/invoices-dark.png)](assets/screenshots/invoices-dark.png) | [![NoCloud expenses](assets/screenshots/expenses-dark.png)](assets/screenshots/expenses-dark.png) |

### Rental locations

Rental workspaces keep unit details, tenants, lease information, rent status,
payments, and unit history together.

[![NoCloud rental unit workspace](assets/screenshots/rental-unit-workspace-dark.png)](assets/screenshots/rental-unit-workspace-dark.png)

## Data and backups

Business records are stored on the Windows computer where NoCloud is used.
Normal daily work is local and does not depend on a browser session or permanent
internet connection.

- NoCloud supports automatic and manual backups.
- Backups can be verified before they are needed.
- A backup is checked before restore, and a safety copy is made first.
- Each business profile keeps its own clients, invoices, expenses, and other
  records separate.
- The backup folder can be placed on another drive or in a synchronized folder
  chosen by the user.

Business records are not uploaded to this repository.

## Installation

1. Open the [latest NoCloud release](https://github.com/GLevek89/NoCloud-Releases/releases/latest).
2. Download the Windows file whose name starts with `NoCloud-Setup-` and ends
   with `.exe`, then run it.
3. Open NoCloud, enter the supplied license key, and complete the guided setup.

> **Windows SmartScreen:** NoCloud's installer is not code-signed yet. Windows
> may display “Windows protected your PC.” Confirm that the installer came from
> this repository, then choose **More info → Run anyway**.

## Updates

NoCloud checks for updates while the application is running. When an update is
ready, the user chooses when to restart and install it. Normal updates keep the
existing activation, business profiles, and records in place. Update checks can
be turned off from **Settings → About**.

<div align="center">

### [Download NoCloud for Windows](https://github.com/GLevek89/NoCloud-Releases/releases/latest)

[License](LICENSE)

</div>
