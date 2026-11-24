# RevzzKey

## Deployment
1. Install Node.js 18+.
2. Set environment variables on your hosting provider:
   - `DRIP_API_KEY`: rotated, new API key (do not use the key previously pasted into chat)
   - `ADMIN_PASSWORD`: long, unique admin password
   - `QRIS_IMAGE_URL`: optional; defaults to `/qris.jpeg`
3. Run `npm install` then `npm start`.
4. Host on a server that supports Node.js (Render, Railway, VPS etc.) and persistent storage. `data.json` is created on first use.

This is a starter implementation. Payment is manual verification by admin; do not rely on customer payment notes as proof. Admin password/token handling is rudimentary and should be strengthened before a public launch. Use HTTPS and persistent disk/database. Supplier order fulfillment occurs only after admin marks payment confirmed. The public catalog endpoint is read-only. Prices are in USD from supplier; configure customer-facing currency, markup and payment flow before launch.
