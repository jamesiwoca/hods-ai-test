# Case Study: Lead Scoring

## A note on the data

The dataset is synthetic — we generated it for this exercise. However, the business names are real UK companies and the scenario is representative of problems we actually work on.

## Background

Six months ago, we started buying leads from a third-party provider. Each month they send us a batch of businesses that might be interested in a loan. For each lead, they provide some basic information about the business and a `lead_score` — their proprietary assessment of how valuable the lead is.

We've been using `lead_score` to decide which leads to market to. Generally, the higher the score, the more likely we are to reach out. For leads we did market to, we tracked whether they converted (took a loan), and for those who did, we recorded the loan terms and our risk assessment at point of issuance.

The data is in `leads.csv`.

## Your Task

We want to move beyond relying on the provider's score. Your job is to:

1. **Explore the data** and assess how well the current approach (using `lead_score` to prioritise leads) is working.
2. **Build a better model** for deciding which leads to market to.
3. **Present your recommendation** — what should we do differently, and why?

You have 60 minutes to work, then 15-30 minutes to walk us through your findings.

## What You Have Access To

- The dataset (`leads.csv`)
- A laptop with internet access
- Any tools or software you'd like to use, including AI assistants

We actively encourage you to use whatever tools you want, including AI and external data sources. There are no restrictions.

## Column Descriptions

| Column | Description |
|---|---|
| `lead_id` | Unique identifier |
| `business_name` | Name of the business |
| `business_description` | Short description of what the business does (may be empty for some rows) |
| `postcode` | UK postcode of the business |
| `lead_score` | Provider's assessment of lead value (1-100) |
| `years_in_business` | How long the business has been operating |
| `annual_revenue_band` | Revenue bracket |
| `employee_count_band` | Employee count bracket |
| `contact_method` | How the lead prefers to be contacted |
| `date_acquired` | Date we received the lead |
| `was_marketed` | Whether we marketed to this lead |
| `converted` | Whether the lead took a loan (null if not marketed) |
| `amount_taken` | Loan amount at issuance (null if not converted) |
| `duration_months` | Loan term in months (null if not converted) |
| `monthly_margin` | Monthly margin rate (null if not converted) |
| `clv` | Customer lifetime value: amount x duration x margin (null if not converted) |
| `risk_score` | Our internal risk assessment at issuance, 1-10 (null if not converted) |
