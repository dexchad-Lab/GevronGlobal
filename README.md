# Gevron Quote Builder

A self-contained, single-file web app for building and exporting Gevron Global Limited power system quotations.

## Use it

Open `index.html` directly in a browser, or serve the folder with any static file host (e.g. GitHub Pages). No build step, no backend — all data (product catalog, quotes, templates, workspace PIN) is stored in the browser's `localStorage`.

## Features

- **Dashboard** — quick stats and shortcuts.
- **Quote Builder** — add one or more packages, pick line items from your catalog (or type custom ones), quantities and costs recalculate totals live. Exports to a client-ready PDF via the browser's print dialog (`Export to PDF`), matching the Gevron document template.
- **Product Catalog** — manage inverters, batteries, panels and accessories with pricing and VAT-ability once, reused across every quote.
- **Templates** — save a package configuration and reload it into a future quote.
- **Settings** — bank details, contact info, default timeline and VAT note applied to every quote automatically.
- Responsive layout (off-canvas navigation on small screens, horizontally-scrollable tables) and a lightweight PIN gate to keep casual visitors out.

## Notes

- VAT is calculated per line item at 7.5%, only for items marked VATable — core solar equipment (panels, inverters, batteries) is VAT-exempt by default, matching Gevron's standard quote terms.
- The workspace PIN is a single shared passcode, not real authentication — it deters casual access only.
