# Santa's Chimney Sweeps — the revamp

A hand-built overhaul of [santaschimneysweeps.co](https://www.santaschimneysweeps.co/),
made as a gift. Everything that made the original *the original* is still here —
it's just been re-set like a good piece of letterpress.

## What stayed (the soul)

- **The oxblood red.** The exact background color of the old site (`#460203`)
  is still the foundation. It was always the best design decision on the page.
- **The mascot.** The chimney-in-a-Santa-hat logo, now with the gray box removed
  so it sits cleanly on the red. (Its original filename, `logooooo.jpeg`, is
  memorialized in a comment at the top of `index.html`.)
- **Every word of the copy.** The mission statement, all three service
  descriptions, all three testimonials, both portfolio write-ups, the
  "Why choose us???" heading (all three question marks, non-negotiable),
  "Book with Santa", "Reserve A Date" — verbatim.
- **The real photos.** All ten photos of actual Louisiana chimneys, job sites,
  and soot piles, straight off the job. Captions like "SOOT 2" and
  "JOB SITE 3" kept as-is. The before/after pair keeps its filename honor as
  "Job No. 7". EXIF/GPS metadata has been stripped from all of them
  (they're photos of customers' homes).
- **The structure.** Same three pages: Home, Book Online, Portfolio.

## What changed

- **The AI stock images are gone** — the man sweeping a *lit* fireplace with a
  straw broom has been retired, along with the clip-art house-value graphic.
  Only real job photos remain.
- **Typography.** Playfair Display (same didone family as the old headings),
  Lora for body text, Oswald for the small trade-card labels. All self-hosted
  in `fonts/` — no external requests, loads fast.
- **Rhythm.** The wall-to-wall maroon now alternates: oxblood → cream paper →
  soot-black photo sections. Arch-topped photo frames echo a fireplace opening.
- **Small copy repairs only**: "creosoot" → "creosote", "maintenace" →
  "maintenance", "homes value" → "home's value", and the "4 years" vs
  "five years" disagreement settled at four (est. 2022).
- **The leftover Wix store** (template cashmere sweaters and table lamps) was
  not carried over. Booking buttons now use `tel:` and `mailto:` links.
- Basic SEO: real page titles, meta descriptions, and LocalBusiness
  structured data with the real phone/email.

## Notes for whoever deploys this

- It's plain HTML + one CSS file. No build step, no framework, no JavaScript.
  Open `index.html` in a browser and that's the site.
- Host it anywhere static files go: GitHub Pages, Netlify, Cloudflare Pages.
- **Social links:** the old site's social icons pointed at blank placeholder
  URLs (literally `facebook.com/`), so they were left out. Add real profile
  links in the footer when you have them.
- **Online booking:** the old Wix booking calendar can't come along to a static
  site. If real-time booking matters more than the phone, either link the
  "Book Online" buttons back to the Wix booking page, or drop in a
  Cal.com/Calendly embed.

```
index.html          Home
book-online.html    Services & booking
portfolio.html      Soot Piles / Job Sites
css/styles.css      All styling
fonts/              Self-hosted woff2 (Playfair Display, Lora, Oswald)
images/             Optimized photos + transparent logo
```
