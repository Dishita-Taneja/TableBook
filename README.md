# TableBook 

A frontend-only restaurant **table booking system**. Manage tables, bookings, customers,
availability, a monthly booking calendar and reports — no backend, no build step.
All data is stored in your browser's `localStorage`.

## Features

- **Auth gate** — register / login (stored locally, roles: Admin, Manager, Staff)
- **Dashboard** — today's reservations, occupancy %, total customers, estimated revenue
- **Table Management** — full CRUD with capacity, floor, location and status badges
- **Bookings** — create, confirm, seat, cancel and no-show; status colour-coded
- **Table Layout** — live floor plan, colour-coded tiles with status glyphs
- **Customers** — directory with visit history
- **Availability** — find free tables for a party size / time slot
- **Calendar** — month view of bookings by day
- **Reports** — totals, cancellations, active covers, revenue + charts
- **Dark / light theme** — toggle in the top bar (persisted)
- **Motion** — micro-interactions and a one-time load stagger; all ≤ 400ms and
  fully disabled when `prefers-reduced-motion` is set

## Project structure

```
TableBook/
├── index.html
├── favicon.svg
├── README.md
├── .gitignore
├── css/
└── js/
    ├── app.js
    ├── data.js
    ├── ui.js
    └── pages/
        ├── availability.js
        ├── bookings.js
        ├── calendar.js
        ├── customers.js
        ├── dashboard.js
        ├── layout.js
        ├── reports.js
        └── tables.js
```
## Run locally

No build. Just open the file:

```bash
open index.html
```

or serve the folder with any static server:

```bash
npx serve .
```
