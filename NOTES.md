# Copilot-Assisted DAX Development Notes

## Measure 1: Total Sales

Copilot Suggestion:
SUM(Fact_Sales[sales_amount])

Correction:
No correction was required.

## Measure 2: Running Total

Copilot Suggestion:
Use CALCULATE and FILTER functions to calculate cumulative sales.

Correction:
The date reference was verified and adjusted to match the Dim_Date table.

## Measure 3: Month-over-Month Growth %

Copilot Suggestion:
Use DATEADD to retrieve previous month sales.

Correction:
The formula was tested and validated using the dashboard visuals.

## Measure 4: City Rank

Copilot Suggestion:
Use RANKX to rank cities based on total sales.

Correction:
Ranking order was set to DESC to display highest sales first.

## Learning Outcome

GitHub Copilot helped generate DAX formulas quickly and reduced development time. However, formulas still required testing and validation before use.