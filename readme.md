# OliSalesTrack

> **Formerly: refund-tracker** — renamed to OliSalesTrack to reflect the full scope of the tool.

Track sales, refunds, and expenses with real-time **correlation analysis**. Know exactly how refunds and costs are eating your profit — daily, weekly, monthly, and yearly.

## What's Inside

| Page | Description |
|---|---|
| `refund-tracker/` | Main PWA application (React 18 + htm, single-file, no build step) |

## Key Features

- **📊 Correlation Analysis** — Pearson r coefficient between sales/refunds/expenses/profit
- **📅 Time periods** — Today, Week, Month, Year views on all charts and KPIs
- **↩️ Refund tracking** — Rate monitoring with alert thresholds, dispute portal links
- **💰 Sales tracking** — CSV import from Shopify, WooCommerce, Stripe
- **💸 Expense tracking** — Category breakdown, ROI by expense type
- **📈 Reports** — Monthly P&L table with margin and refund rate
- **⭐ Upgrade** — Links to Pro ($19/mo) and Lifetime ($149) plans
- **🔒 Privacy-first** — All data stored locally in the browser

## Running Locally

```bash
# Any static file server works:
npx serve refund-tracker/
# or
python3 -m http.server --directory refund-tracker/ 8080
```

Then open `http://localhost:8080`.

## Pricing

| Plan | Price | Notes |
|---|---|---|
| Free | $0 | Full tracking, basic charts |
| Pro | $19/mo or $148/yr | Correlations, AI insights, PDF reports |
| Lifetime | $149 one-time | Everything in Pro, forever |

See [olisalestrack/buy/](https://workitlikeapro.com/olisalestrack/buy/) for checkout.

## Changelog

- **v2** — Renamed to OliSalesTrack. Added Correlations page (Pearson r analysis), Upgrade page, improved NAV.
- **v1** — Initial release as refund-tracker.
