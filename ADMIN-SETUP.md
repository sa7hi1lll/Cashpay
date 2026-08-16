# Sa7hil Admin Setup

The admin page checks the Firebase Authentication ID token for the custom claim:

`admin: true`

## Important
Do NOT set this claim from browser JavaScript.

Set it from a trusted backend using the Firebase Admin SDK, for example:

`setCustomUserClaims(uid, { admin: true })`

Then sign out/in (or refresh the ID token) and open `admin.html`.

Also publish Firestore Security Rules that require `request.auth.token.admin == true` for admin-only updates.

The included admin page is therefore an admin UI; the custom claim + Security Rules provide the authorization boundary.
