 # LoopLoyal — Digital Loyalty Card System

A mobile-first concept for digital loyalty cards for barbershops, beauty salons, cafés and other local businesses.

## Current prototype

- Responsive landing page
- Interactive sample loyalty card
- Sample stamp circles and reward progress
- Business-focused explanation of shop QR codes, staff-authorised stamps, shop profiles and reviews

## Important limitations

This is a front-end demonstration, not a live loyalty service yet. The sample stamp button only changes the preview in the current browser. It does not create accounts, generate shop-specific QR codes, store real customer cards, verify visits, enforce a server-side 24-hour restriction, or publish customer reviews.

Do not use this demo to issue real rewards or collect customer personal information.

## Next development stages

1. Choose a backend and authentication provider.
2. Create database tables for businesses, staff, customers, loyalty cards, stamp events, rewards and reviews.
3. Generate a unique QR URL for every business.
4. Add owner/staff authentication and server-side stamp authorisation.
5. Enforce the 24-hour rule on the server per customer and shop.
6. Add reward redemption history and verified-visit reviews.
7. Add location search, business profiles and deployment configuration.

## Run locally

Open index.html in a browser, or serve this folder using a local development server.

## GitHub Pages

In the repository, open Settings, then Pages. Select Deploy from a branch, choose main and the root folder, then save. GitHub Pages may take a few minutes to publish.

## Security design note

A static QR code alone is not proof that a customer has visited a shop. In production, a stamp must be authorised by an authenticated shop owner or staff account, or another short-lived server-verified mechanism. The 24-hour restriction must be enforced on the server, not in browser JavaScript.
