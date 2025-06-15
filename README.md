## ERPNext ETA

Integration for Egyptian Tax Authority

### Multi-company

ETA operations only run for companies where the **Country** field is set to
"Egypt". Scheduler tasks and API endpoints skip other companies automatically.
Custom fields such as *ETA Default Activity Code* use dynamic requirements based
on Frappe `depends_on` expressions like `eval:doc.country == 'Egypt'` so
non‑Egyptian companies are not forced to fill them.

#### License

GPLv3
