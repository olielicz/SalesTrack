# OliSalesTrack

> **Formerly: refund-tracker** — renamed to OliSalesTrack to reflect the full scope of the tool.

Track sales, refunds, and expenses with real-time **correlation analysis**. Know exactly how refunds and costs are eating your profit — daily, weekly, monthly, and yearly.

## What's Inside

| Page | Description |
|---|---|
| `refund-tracker/` | Main PWA application (React 18 + htm, single-file, no build step) |

## Key Features

- **📊 Correlation Analysis** — Pearson r coefficient between sales/refunds/expenses/profit
- **🤖 AI-generated insights** — a real, optional AI narrative of your correlation/P&L numbers, grounded strictly in figures this app already computed (never raw transactions), with a numeric honesty guard that rejects any AI response citing a number outside that real dataset. Without an AI key, a real, deterministic rule-based narrative is used instead — this tier always works.
- **📄 PDF report export** — a real, dependency-free, hand-built PDF export of the Correlations page, generated entirely client-side.
- **🏢 Multiple business profiles** — real, separate `localStorage`-scoped datasets per business, with a switcher in Settings.
- **📅 Time periods** — Today, Week, Month, Year views on all charts and KPIs
- **↩️ Refund tracking** — Rate monitoring with alert thresholds, dispute portal links
- **💰 Sales tracking** — CSV import from Shopify, WooCommerce, Stripe
- **💸 Expense tracking** — Category breakdown, ROI by expense type
- **📈 Reports** — Monthly P&L table with margin and refund rate
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

**Free.** Correlation analysis, AI-generated insights, PDF report export, multiple
business profiles, refund/expense tracking, dispute portal links, and CSV import are
all included in the base app — none of them are gated behind a paid tier.

The `UpgradePage` previously advertised $19/mo Pro and $149 Lifetime tiers gating
exactly these four features; since they're now genuinely built into the free app,
that page has been corrected to state honestly that everything is included. If a
real paid tier with a genuinely different feature set is introduced in the future,
document that feature set specifically rather than re-gating what's already free.

## Changelog

- **v3** — Added real AI-generated insights (grounded, honesty-guarded, with a
  deterministic rule-based fallback), real PDF report export, and real multiple
  business profiles. Corrected `UpgradePage` to stop gating these now-free features
  behind a paid tier.
- **v2** — Renamed to OliSalesTrack. Added Correlations page (Pearson r analysis), Upgrade page, improved NAV.
- **v1** — Initial release as refund-tracker.
