# Farm Fresh Box

Weekly grocery pre-order app: customers order by the weekly cut-off, and the order is delivered to their society.
The whole app is one file, `index.html` (React loaded from a CDN), so there is nothing to build.

## Deploy on Render (Static Site)
1. In Render choose **New > Blueprint** (or **New > Static Site**) and connect this repo.
2. For a Static Site set **Build command** to empty and **Publish directory** to `.`
3. `CFG.pageUrl` in `index.html` is already set to https://farm-fresh-box.onrender.com. Change it if the address changes.
   (society invite links are built from it), then commit and push.
4. Set `CFG.wa` to the real WhatsApp number (country code first, no plus sign). Orders are sent to it.

## Admin
Open the site with `#admin` at the end of the address. The test admin number is in `ADMIN_MOBILES`.

## Known limits (no backend yet)
Orders, employees, delivery codes, settings and insights are saved in each person's own browser,
and the login OTP is a demo shown on screen. Real OTP and shared data need a backend.
