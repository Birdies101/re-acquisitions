# Conventions

## File naming

Use `YYYY-MM_Market_AssetType_Strategy_Description_vN.ext` so files sort by date and the latest version is obvious.

Examples:

- `2026-11_Orlando_MF_ValueAdd_Model_v2.xlsx`
- `2026-12_Atlanta_Industrial_CorePlus_Memo_v1.md`
- `2027-01_Sunbelt_BridgeLoans_CaseStudy_v1.md`

Use underscores between parts, no spaces, and bump the version number instead of overwriting a file you have shared.

## Excel standards

- Color code: blue font for inputs, black for formulas, green for links to other sheets.
- One assumptions sheet. No hard-coded numbers inside formulas.
- Build checks: sources equal uses, debt balance at maturity, waterfall distributes 100% of cash.
- Never paste values over formulas.
- Add a notes sheet listing data sources and open questions.

## Writing standards

- Lead with the conclusion, then the numbers, then the risks.
- Cite every data source with a link and date.
- State assumptions explicitly and show a downside case.

## Data rules

- Public or synthetic data only. Never commit data from an employer, a paid provider, or a private deal.
- Large raw downloads stay out of git (`data/raw/` is ignored). Document where to get them in `data/raw/README.md`.

## Commits

- Commit small and often with clear messages, for example `Add exit cap sensitivity to MF template`.
- A visible history of steady improvement is part of the portfolio.
