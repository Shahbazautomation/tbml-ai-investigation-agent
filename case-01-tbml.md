# Case Study 01 — Trade-Based Money Laundering (TBML)

> **Synthetic case — for portfolio demonstration only. All names, companies, and figures are fictional.**

## Case Reference
`CS-TBML-01` (synthetic)

## Typology
Trade-Based Money Laundering via **over-invoicing** and a **shell counterparty**.

## Background / Trigger

A commercial bank's Transaction Monitoring Unit flagged a Letter of Credit (LC) transaction for review after an automated alert on unusually high per-unit pricing relative to market benchmarks. The importer, **Zenith Textile Traders (Pvt) Ltd.** (fictional entity), submitted trade documents for a shipment of "premium finished fabric" from a supplier in a high-risk jurisdiction, **Alpha Fabrics FZE** (fictional entity).

## Investigative Methodology

1. **Document review** — LC, commercial invoice, bill of lading, packing list, and customs goods declaration (GD) compared line-by-line for consistency.
2. **Price benchmarking** — declared unit price (~USD 42/kg) compared against published trade data and comparable HS-code shipments (market range USD 9–14/kg).
3. **Beneficial ownership tracing** — corporate registry and UBO declarations pulled for both the importer and the supplying entity to identify common control.
4. **Bank record analysis** — importer's account history reviewed for the source of the LC margin funds and post-clearance fund flows.
5. **Cross-reference with FMU/SBP guidance** on TBML red flags and prior STR filings involving the same counterparty network.

## Red Flags Identified

- Declared unit price **3–4x above market benchmark** for the stated goods category.
- Supplier entity registered **18 months prior**, no prior trade history, registered address shared with two unrelated trading companies (shell indicator).
- Importer's LC margin funded by a same-day inbound transfer from a **third-party individual account** with no documented commercial relationship to the importer.
- Shipping route showed a **transshipment stop** in a jurisdiction inconsistent with the stated manufacturing origin.
- Post-clearance, ~60% of the imported "fabric" lot was **re-exported within 30 days** to a third country at a price close to the original inflated value — inconsistent with normal retail/wholesale margins.

## Analysis — Evidence Trail (synthetic figures)

| Date | Transaction | Amount (USD) | Notes |
|------|-------------|--------------:|-------|
| 2026-01-04 | Inbound transfer to importer (LC margin funding) | 85,000 | From unrelated third-party individual account |
| 2026-01-06 | LC issued — Zenith Textile Traders → Alpha Fabrics FZE | 340,000 | Declared 8,000 kg @ USD 42.5/kg |
| 2026-01-22 | Goods cleared through customs | — | GD value flagged by risk-engine for over-valuation |
| 2026-02-14 | Re-export of ~4,800 kg to third-country buyer | 205,000 | Sold at near-original inflated unit price |

**Assessed outflow inconsistent with legitimate trade margin:** the pricing and rapid re-export pattern are consistent with using the trade transaction to move value across borders while generating an ostensibly legitimate paper trail, rather than genuine commercial trade.

## Outcome / Recommendation

- Case escalated for **STR filing** with the Financial Monitoring Unit (FMU) citing TBML red flags under FATF Trade-Based Money Laundering guidance.
- Recommended **enhanced due diligence (EDD)** on both counterparties and a review of all prior LC transactions involving Alpha Fabrics FZE across the bank's client base.
- Recommended freezing further LC issuance to the counterparty pending FMU response.

## Skills Demonstrated

Trade document analysis · TBML red-flag detection · Beneficial ownership tracing · Bank record/fund-flow analysis · STR drafting · FATF/AML Act 2010 regulatory application

## Related automation

The pricing-anomaly and shell-counterparty logic in this case is the same red-flag set implemented in my live [TBML AI Investigation Agent](https://github.com/Shahbazautomation/tbml-ai-investigation-agent), which automates first-pass screening of trade transactions against these indicators.
