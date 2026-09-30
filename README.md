# Proposal Generator

Generates commercial proposals from RO system technical design PDFs.

## How it will work

1. **Extract**: read the design PDF: customer, project, and per-train equipment
   (pressure exchanger / turbocharger, booster pump, interstage booster pump,
   high-pressure feed pump) with model numbers and quantities.
2. **Classify**: determine the system configuration:
   - PX + booster pump
   - PX + interstage booster pump
   - Turbocharger
3. **Price**: look up list prices and apply discount rules.
4. **Render**: fill the proposal template and export Word/PDF.

## Layout

```
proposal_generator/   source code
templates/            proposal template(s): layout only, no pricing
tests/                tests (using anonymized sample data only)
data/                 CONFIDENTIAL: PDFs, price list, outputs (git-ignored)
```

## Confidentiality

Customer documents, price lists, discount rules and generated proposals belong
in `data/`, which git ignores. Keep this repository **private**.
