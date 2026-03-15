# Pizzon Admin Panel

Full admin panel to **control the entire website**: orders, dispatch, riders, menu, content, settings, coupons, and users. **Not linked from the customer website** — no nav button or link to this panel; only staff with the URL can access it.

## Run locally

From repo root:

```bash
pnpm run start:admin
# or
pnpm run dev:admin
```

Opens at **http://localhost:5174**

## Login

- Any username (and any password) signs you in for demo.
- Replace with real auth (e.g. backend `/api/auth/login`) when integrating.

## Sidebar & routes (after login)

- **Dashboard** (`/`) — Overview, stats, recent orders
- **Orders** (`/orders`) — Orders list, assign rider, view, invoice, track
- **Order detail** (`/orders/:id`) — Status, customer, items, assign rider, invoice
- **Track** (`/track`) — Live rider map
- **Riders** (`/riders`) — Riders list, add/edit
- **Menu & Products** (`/menu`) — Categories and items (controls website menu)
- **Content** — About, Blog, Team, Specials, Gallery, Testimonials, Contact, Reservation (controls each section on the website)
- **Coupons** (`/coupons`) — Discount codes for checkout
- **Settings** (`/settings`) — Store info, hours, tax, delivery
- **Users** (`/users`) — Panel users (admin/staff)

No animations. Backend integration can replace mock data and wire save actions later.

## Deploy

Deploy this app separately (e.g. `admin.pizzon.com`). Do not link to it from the public site.
