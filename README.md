# Jace AI Solutions — consulting site

single-file static site (`index.html`) — no build step, no dependencies, deploy anywhere.

## the whatsapp number

set in the CONFIG block at the top of the `<script>` at the bottom of `index.html`:

```js
const WHATSAPP_NUMBER = "917973744625";
```

to change it (e.g. to a +1 virtual number later): international format, digits only —
country code + number, no `+`, no spaces, no dashes (e.g. Canada 604-555-1234 → `16045551234`).
note: the number never appears on the page — visitors only see it after they open the chat.

that single constant powers:
- every "Chat on WhatsApp" button (nav, hero, CTA band, contact, footer)
- the floating green bubble (bottom-right)
- the contact form — on submit it opens WhatsApp with the visitor's answers
  pre-filled as a message to you (no backend, nothing stored)

## deploy

it's one static file — Render static site (`staticPublishPath: .`), GitHub Pages,
or Vercel all work as-is. custom domain later via the host's dashboard.

## content sources

positioning, skills, and the Work section come from the resume site
(`Desktop/resume/index.html`) — First Hello, Glow, My Personal Teacher,
Simple Analysis, Morrigan, and the applied-ML case studies are all real
shipped projects; stats in the hero strip are real numbers. no invented
testimonials or client logos — add real ones as they come.
