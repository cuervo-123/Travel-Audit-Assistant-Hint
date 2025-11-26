# Travel Audit Assistant — Tech Blue+

> Static GitHub Pages app for CSV ingestion, rule-based findings & PDF exports — built for Gaven’s company.

![Banner](assets/banner.svg)

**Launch the app:**  
👉 [https://cuervo-123.github.io/Travel-Audit-Assistant/](https://cuervo-123.github.io/Travel-Audit-Assistant/)

## Features
- CSV **Data Ingestion** (local, private — no server)
- **Rules** engine (JSON) with default checks:
  - `HOTEL_CAP` (USD per night limit)
  - `FLIGHT_CLASS` (allowed economy classes; approval exception)
  - `DUPLICATE_INVOICE` (duplicate invoice_id detection)
- **Findings** table + **Dashboard** KPIs
- **PDF** export (jsPDF)
- **Dark / Dark+** theme toggle
- **Contextual Help** buttons per section (modal overlay)

## Suggested CSV columns
**expenses.csv**
```
id,trip_id,category,amount,currency,date,vendor,invoice_id,justification_url,approved,nights,flight_class
```
**trips.csv**
```
id,employee,destination,start_date,end_date,flight_class,booked_fare
```

## Quick Start (local)
1. Download repo and open `index.html` in your browser.
2. Go to **Ingestion** → upload `expenses.csv` (and optional `trips.csv`).
3. Check **Findings** and **Dashboard**.
4. Open **Rules** to edit JSON and re-apply.
5. **Reports** → Generate PDF.

## Credits
- Branding: **Cuervo‑Inc / Tech Blue+**
- Built with PapaParse + jsPDF (CDN)

## License
MIT
