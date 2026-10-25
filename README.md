# FORTY FIVE MVP — prototype

## Included
- Responsive storefront with two sample products
- Custom T-shirt preview: text, shirt colour, size and preview price
- Cart and demo checkout form
- Owner dashboard (demo code: `4545`)
- Product price editing, order status updates, CSV export
- PWA manifest and service worker for installable-web-app testing

## Important limitations
This is a **front-end prototype**, not a production store.
- Products, cart and orders are saved in the current browser's `localStorage`.
- Orders will NOT sync between customer and owner devices.
- The owner code is a demo gate only; it is not secure authentication.
- No real payment gateway, email/SMS, cloud database, supplier integration, live shipping, returns workflow or tax calculation is connected.
- Do not collect real customer personal data with this prototype.
- Prices are demo values, not confirmed offers.

## Test locally
Open `index.html` in a modern browser. Some PWA features require HTTPS or localhost.

## Free web hosting route
1. Create a GitHub account and a new public repository.
2. Upload `index.html`, `manifest.webmanifest`, and `service-worker.js` to the repository root.
3. In repository Settings → Pages, publish from the main branch/root.
4. Open the HTTPS Pages URL on Android Chrome. Use browser menu → Install app / Add to Home screen.
5. Test the app on a second device. Remember: localStorage does not sync orders.

## Android APK route
A PWA is not automatically an APK. Once the HTTPS site is deployed and meets the packaging tool's current requirements, evaluate PWABuilder (https://www.pwabuilder.com/) or Bubblewrap/TWA. Follow its current build/signing instructions and test the APK on your own phone. Play Store publishing requires a Google Play developer account and fee; that is outside the ₹500 MVP budget.

## Recommended production next phase
Add a hosted database and real owner authentication before accepting orders. Firebase/Supabase free tiers may be options, subject to current limits and configuration. Then add customer order tracking, privacy notice, payment and shipping workflows.
