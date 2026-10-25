# www.altitude.yoga → studio.altitude.yoga

This GitHub Pages site exists only to answer for **www.altitude.yoga** (and **altitude.yoga**,
when its A records point at GitHub) and send visitors to the Altitude Yoga website at
**studio.altitude.yoga**, which is published from
[as200219/altitude-yoga-website](https://github.com/as200219/altitude-yoga-website).

- `index.html` forwards straight away (script, with a refresh tag as a fallback). Old Wix
  addresses map to the new pages (`/team-1` → `teachers.html`); anything else goes to the home
  page, keeping any `*.html` page name as is.
- `404.html` is the same page, so every address on www forwards, not just the home page.
- `CNAME` holds the domain this site answers for.

DNS (Wix → Domains → altitude.yoga): `www` is a CNAME to `as200219.github.io`.

The forwarding target is `http://studio.altitude.yoga` so it works before the studio site's
HTTPS certificate is issued; once HTTPS is enforced there, GitHub upgrades it automatically.
