# Synthetic Control Analysis — Owens Valley Water Transfer and LA Economic Growth

A sample of my applied econometrics code in R. It estimates the long-run
regional effect of the early-20th-century Owens Valley water transfer on
economic growth in Los Angeles County, using the **synthetic control method**
(Abadie, Diamond, and Hainmueller).

Los Angeles County is the treated unit; a weighted combination of untreated
California counties forms the "synthetic Los Angeles" counterfactual. The
outcome is GDP per capita and the treatment year is 1920, estimated on a
historical county-level panel (1860–1950).

## What the code does

1. Loads and prepares the historical census panel of per-capita economic
   variables (GDP, manufacturing, agriculture, capital investment, employment,
   wages).
2. Constructs the synthetic control and estimates the treatment gap.
3. Runs a placebo (falsification) test that reassigns treatment to each control
   county and computes permutation-based p-values (Cavallo et al., 2013).
4. Visualizes the path plot and the placebo gap distribution.

## Files

- `Code_Sample_Arpita_Nehra_PDF.html` — the rendered report (code, output,
  tables, and figures). **Download it and open in any web browser to view.**

## Tools

Written in **R** / R Markdown. Key packages: `Synth`, `readxl`, `ggplot2`,
`stargazer`, `xtable`.

## Author

Arpita Nehra
