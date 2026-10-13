# Kinetic Twin: conversational 3D digital twin WMS

**Live demo:** https://1brytn.github.io/kinetic-twin/

A concept prototype for a next-generation Warehouse Management System. Instead of static dashboards, warehouse operations run as a live 3D digital twin, with an embedded ops copilot you can ask in plain language ("Why is shipment #78466 delayed?"). The copilot traces the causal chain, lights up the trucks, doors, aisles and forklifts involved, and proposes fixes you can approve.

## What it shows

- **Live 3D twin.** Trucks arrive by road, wait in the yard, back in to dock doors D1 to D8 and pull out. Forklifts run putaway and picking, rack stock and staging pallets update as they work.
- **Root-cause reasoning.** Doors stall when inbound staging fills; staging fills when putaway capacity drops; the copilot walks that chain back to the real cause.
- **Disruption injection.** Late trucks plus an e-commerce surge, a spill in the fast-mover aisle, or a forklift battery fault.
- **Approve-to-act.** Recommended actions (cross-dock, reroute an aisle, reassign a forklift, battery swap) change the running simulation.
- **Blueprint tab.** White paper covering the paradigm shift, six-layer system architecture, agentic AI logic and use cases.

## Notes

- All data is synthetic. Time and impact figures in the blueprint are illustrative design targets, not measured results.
- In this public demo the copilot runs on a built-in rules engine over the live simulation state (no API key needed).
- Built as a single HTML file with three.js (r128) for 3D and Mermaid for the architecture diagram.

## Run locally

Open `index.html` in a browser, or serve the folder: `python -m http.server`.

## Author

Krisna Hayu Dirgantara, Industrial Engineering (UMM).
[LinkedIn](https://linkedin.com/in/KrisnaHayuDirgantara) · [Portfolio](https://1brytn.github.io/Portfolio)
