# Jace AI Solutions — custom browser automation site

single-file static site (`index.html`) — no build step, no dependencies.
live: https://jace-ai-solutions.onrender.com (Render static site, auto-deploys on push to main).

the site is the browser-automation product pitch ("the internet was made for humans, not
scripts"), styled like Claude web: warm cream, terracotta accent, serif headings, dark
terminal blocks. the earlier general consulting site lives in git history (last version at
commit `eaf6e4b`) if it's ever wanted back.

## the whatsapp number

set in the CONFIG block at the top of the `<script>` at the bottom of `index.html`:

```js
const WHATSAPP_NUMBER = "917973744625";
```

to change it: international format, digits only — country code + number, no `+`, no spaces,
no dashes. the number never appears on the page — visitors only see it after they open the
chat. it powers every green button, the floating bubble, and the contact form (which opens
WhatsApp with the visitor's answers pre-filled — no backend, nothing stored).

## content honesty notes

- the "3 real end-to-end submissions" proof (SuccessFactors / Greenhouse / Workday) is from
  the verified runs in `Desktop/test_e2b/design/project.md`.
- the hotel-receptionist section is labeled **illustrative** — it is an offer example, not a
  deployed system.
- the hero "spots open" counter is seeded from the UTC date (1–5, same for all visitors on a
  given day).
