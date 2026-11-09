# The BarberShop Blenheim, website (DNA-X side project)

Static one-page site for The BarberShop, 25 Grove Road, Mayfield, Blenheim. Plain HTML, no build step, hosts on GitHub Pages.

## Files
- `index.html`: the whole site (styles and script inline)
- `img/logo-white.png`: logo cut out of the sign photo, white on transparent (use on blue/dark)
- `img/logo-badge-clean.png`: rebuilt blue badge, clean edges (social / Google profile)
- `img/favicon.png`: tab icon
- `img/shop-*.jpg`, `img/team.jpg`: shop and team photos
- `_source/`: raw photo crop of the sign (not used by the site)

## Before go-live
1. Real prices: replace every `From $XX` in the Services section.
2. Remove `<meta name="robots" content="noindex, nofollow">` so Google can index it.
3. Booking form: set `FORM_ENDPOINT` at the top of the script (Formspree or a Make webhook that emails/SMSes the shop). Left blank, the form runs in demo mode and sends nothing.
4. Confirm crew names and roles are current.
5. Custom domain (optional): add a `CNAME` file and point DNS at GitHub Pages.

## The two offers
- **Website, $100**: this site live, their domain, form wired to email.
- **Booking system, $1,000 (separate project)**: real availability per barber, confirmations and reminder texts, cancel/reschedule links, a simple day-sheet for the shop. The demo form shows the customer side of it.
