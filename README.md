# Sa7hil Campaign — Firebase ZIP

Firebase project configured: `cashpay-61b07`.

## Setup
1. Firebase Console → Authentication → enable Email/Password.
2. Firebase Console → Firestore Database → create database.
3. Review `firebase.rules.txt` and publish proper Security Rules.
4. Upload all files to GitHub repository root.
5. GitHub Pages → Deploy from `main` / root.
6. `index.html` must remain in repository root.

## Important
The Firebase web config is intended for web apps and is not a server password. Security must come from Firebase Auth and Firestore Rules.

UPI/IMPS wallet crediting is NOT implemented as a fake client-side success flow. Real payments require a payment gateway and server/webhook verification.
