# Fire Alarm & Building Operations Analytics

**Starky Paulino | Excel · Power Query · Power BI · DAX**

## Project overview

Built a four-page Power BI report to explore recorded building-system impairments, floor activity, recurring trouble and supervisory observations, report coverage, and documented durations.

The project combines fire-life-safety domain knowledge with data preparation, modeling, visualization, and careful treatment of incomplete operational records.

**Status:** Internal report built and refresh tested. Source validation remains provisional. A public demonstration using synthetic data is in preparation.

## Business questions

- How does recorded impairment activity vary by month?
- Which floors and reasons appear most often in floor-disablement records?
- Which devices have recurring trouble observations?
- How complete is the reporting coverage?
- What do eligible records show about documented durations?

## Preparation and modeling

- Preserved source records and assigned fixed record identifiers.
- Kept original labels alongside standardized categories.
- Flagged missing times, uncertain dates, possible repeats, and unresolved mappings.
- Separated directly observed FACP conditions from context and assumed-live entries.
- Classified durations as eligible, requiring review, or excluded.
- Connected four preparation tables to a shared date table using one-to-many relationships.
- Created DAX measures for record counts, observations, coverage, and eligible average and median durations.

## Report pages

| Page | Purpose |
|---|---|
| Data Quality & Coverage | Reporting coverage and duration eligibility |
| Operations Overview | Monthly activity, categories, floors, and reasons |
| Trouble & Supervisory | Recorded observations by month, device, and status |
| Documented Durations | Eligible record counts and average versus median durations |

## Interpretation and limitations

- Recorded observations can describe the same condition across multiple shifts; they are not unique incident counts.
- Reporting practices changed in August 2026, limiting comparisons across that change.
- A day without a report is not evidence of an event-free day.
- Duration analysis includes eligible records only.
- Durations may overlap and do not measure total building downtime or overall mean time to repair.
- Source-review questions remain open, and results may change as they are resolved.

## Validation

- Checked record totals and duration classifications.
- Tested date filtering and chart interactions.
- Resolved Power Query conversion errors while preserving source text.
- Refreshed the data and schema without reported errors.
- Saved a separate reviewed Power BI backup.

These checks confirm report behavior and internal consistency; they do not establish that every source record is accurate.

## Public demonstration

The operational workbook, source records, and internal Power BI file are not included in this repository.

A synthetic demonstration and report screenshots will be added separately and clearly labeled as demonstration data.

## Skills demonstrated

Excel data preparation, Power Query transformations, dimensional modeling, DAX, interactive Power BI reporting, data-quality assessment, and analytical communication.

## Author

Starky Paulino  
Data Analyst / BI Analyst
