# Automatic Ticket Assignment – ServiceNow Project

A ServiceNow Flow Designer project that routes newly created Incident records to assignment groups based on the incident Category.

## Project implementation

- **Platform:** ServiceNow Personal Developer Instance (PDI)
- **Flow:** Automatic Ticket Assignment
- **Trigger:** Incident Created
- **Flow logic:** Category conditions followed by Update Incident Record actions

## Assignment mapping documented in the project

| Incident category | Assignment group |
|---|---|
| Hardware | Hardware Support |
| Network | Network Support |
| Software | software support |
| Database | security support |

**Accuracy note:** The supplied ServiceNow evidence shows `Database` as the fourth category mapped to `security support`. It does not show a separate `Security` category.

## Repository contents

- `Automatic_Ticket_Assignment_Project_Report.pdf` – PDF project report
- `Automatic_Ticket_Assignment_Project_Report.docx` – editable Word report
- `evidence_screenshots/` – screenshots captured during the ServiceNow project build and testing

## Testing evidence

The evidence includes the Flow execution details and incident records. The Hardware debug execution shows the Hardware condition evaluating to True and its Update Record action completing; the other category conditions are False for that Hardware test record. Separate incident records show the other category-to-group assignments.

## Important scope note

This repository contains project documentation and screenshots. It does not contain a ServiceNow application export or update set.
