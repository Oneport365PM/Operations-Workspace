# OnePort 365 · Freight Operations Workspace (prototype)

A static HTML prototype with two views on the same shipment data:

- **Operations → Shipments**: what the Ops team uses. Each shipment's Progress tab lists the Booking and Post-Booking tasks for its service combination, from the OnePort 365 Service Workbook.
- **Leadership → SLA Milestones**: what leadership sees. Every active shipment across four stages (Prospect, Pre-Booking, Booking, Post Booking). Opening a shipment shows the leadership progress indicators under each stage, which complete from Ops activity in the Progress tab or from system events.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app: Shipments, Progress tab, Leadership view |
| `data/service-milestones.js` | The Service Workbook export: 27 service combinations and their tasks |

## Running it

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8080
```

Then go to `http://localhost:8080/`. Add `#leadership` to the URL to open on the Leadership view.

All data is sample data held in memory; reloading the page resets it.
