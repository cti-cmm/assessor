# v1.0 - 17 April 2025

## New Features

### Major

- Added several fields within each Domain to begin prioritizing practices for growth. These includes the fields Target Score, Est. Impact, Est. LoE, Priority, and Target Date.
- Assigned licensing for the CTI-CMM assessment to Apache License 2.0.
- Added two new sheets to the spreadsheet called "Priorities Summary" and "Planning Sheet". 
  - Priorities Summary captures all practices, and based on a user-defined priority is filtered to only the priority practices. 
  - The user then copies the resulting practices to the "Planning Sheet" for filtering and re-ordering.

### Minor

- Migrated from Google Sheets to Microsoft Excel for the maintanence of the assessment.
- Fixed the speed guage chart and migrated it from Google Sheets to Microsoft Excel formatting.

## Improvements

- Added Freeze panes for each Domain at column g, row 5 for ease of use with new wider columns from planning sheet prep.
- Uniformly spaced the columns across domains and ensured row spacing was appropriate.

## Fixes

- Multiple Domains on the Dashboard sheet were incorrectly linking to different cells on the source domain sheet, leading to inaccurate Score and Max values.
- All domain sheets - The Status field in each Domains wasn't applying the N/A change into it's value, which meant N/A was leaving the Status cell value at `Not Implemented`
- Max Score calculation was subtracting 6 instead of 3 for one row of N/A - this casued the section subtotal to be off by 3 per N/A leading to some wonky math.
- When Domain in Use was set to No, this wasn't deducting the max score from the Dashboard page. This meant the Total Score was not adjusting and thus was creating issues with factoring enterprise maturity.
