# Sa7hil Campaign — Public Website Starter

This ZIP contains a GitHub Pages-ready static website with:

- Sa7hil branding/logo
- Landing page
- Login demo
- Dashboard
- Campaign creation
- Unique public campaign links (`campaign.html?id=...`)
- Copy/share/preview
- Reports
- Wallet UI with UPI/IMPS request placeholders
- Profile
- Admin panel UI

## GitHub Pages

Upload the contents of this folder to the **root** of your repository.

GitHub:
`Settings → Pages → Deploy from a branch → main → /(root)`

The repository root must contain `index.html`.

## Important for a REAL public launch

The included site uses `localStorage` as a demo data layer. That means it is not a multi-user production backend.

For a real public service, connect:

- Firebase Authentication
- Firestore
- Firebase Storage (if needed)
- Firebase Security Rules
- Admin custom claims / server-side authorization
- A proper payment gateway for UPI/IMPS verification

Never credit wallet balances based only on browser JavaScript. Payment success must be verified server-side/webhook-side.

The `admin.html` included here is a UI starter, not a secure production admin system until authentication/authorization is implemented.
