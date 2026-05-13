# Amazon Air Facility List

## File
`amazon_air_facilities.csv` — hand-compiled list of known Amazon Air facilities (snapshot 2026-05-12).

## Schema

| Column | Description |
| --- | --- |
| `airport_id` | FAA 3-letter code (e.g., CVG) |
| `airport_icao` | ICAO 4-letter code (e.g., KCVG) |
| `airport_name` | Full airport name |
| `role` | One of: `primary_hub`, `regional_hub`, `polar_gateway`, `gateway`, `mini_station` |
| `opened_year` | Year Amazon Air operations began at this facility |
| `status` | `active`, `announced`, or `closed` |
| `city`, `state` | Location |
| `latitude`, `longitude` | Decimal degrees |
| `source_url` | Primary citation for this entry |
| `snapshot_date` | Date this snapshot was compiled |

## Role definitions

- **primary_hub** — central sortation facility (only KCVG)
- **regional_hub** — major regional sortation, multi-aircraft daily ops
- **polar_gateway** — Anchorage; used for transpacific transit and engine swaps
- **gateway** — significant Amazon Air daily flight activity, dedicated Amazon ramp space
- **mini_station** — smaller operation, limited daily flights, often shared facilities

## Methodology

This list is compiled from public sources. There is no single authoritative published list of Amazon Air facilities — even the Chaddick Institute's annual report (the most cited academic source) is itself compiled from FAA filings, press releases, and direct observation.

This compilation prioritizes facilities that are:
1. **Confirmed** in Amazon press releases or news coverage
2. **Active** as of the snapshot date (excludes mothballed or unconfirmed announced sites)
3. **Continental US + Anchorage** (excludes international: BCN, CGN, LEJ, etc.)

## Known limitations

- Some smaller mini-stations may not be captured
- "Opened year" reflects best public information but Amazon does not always announce openings
- The line between "gateway" and "mini_station" is judgement-based, not officially defined
- This list will go stale; the most authoritative real-time source is the Chaddick Institute's annual Amazon Air Industry Report

## Citation recommendation for the final project report

> Amazon Air facility list compiled from Amazon press releases, FreightWaves coverage,
> and the Chaddick Institute for Metropolitan Development annual Amazon Air report,
> snapshot date 2026-05-12.
