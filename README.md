# vsa-iti-l2

Static Level 2 test page for Vaish Industries ITI hiring. Camera + mic recording needs an
origin we control (Apps Script's iframe blocks `getUserMedia`), so this page is served from
GitHub Pages and talks to the Apps Script backend (`iti-hiring-tests`) over `fetch`.

- `index.html?k=<one-time token>` — issued by the backend's `admin=l2invite`.
- No secrets here: the backend validates the token, slot window and stores everything.
