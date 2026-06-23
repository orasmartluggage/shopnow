# ORA Signature — Website

A single-page marketing site for the ORA Signature smart luggage. Built as one
self-contained `index.html` file plus an `assets/` folder of images. No build
step, no dependencies — just static files you can host anywhere.

---

## What's in here

```
index.html        ← the entire website (HTML + CSS + JS in one file)
assets/           ← logos and product photos
README.md         ← this file
.gitignore
```

---

## Put it online (GitHub Pages — free)

1. Create a new repository on GitHub (e.g. `ora-website`).
2. Upload **everything in this folder** to the root of the repo —
   `index.html`, the `assets/` folder, and this README. (You can drag the files
   straight into GitHub's web uploader.)
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment**, set **Source = Deploy from a branch**,
   **Branch = main**, folder = **/ (root)**, then **Save**.
5. Wait ~1 minute. Your site will be live at
   `https://<your-username>.github.io/<repo-name>/`.

**Custom domain (optional):** in Settings → Pages → Custom domain, add your
domain and follow the DNS steps GitHub shows you.

### Even faster: Netlify
Go to [app.netlify.com/drop](https://app.netlify.com/drop) and drag this whole
folder onto the page. It's live in seconds with a free URL you can rename.

---

## How to edit the common things

Open `index.html` in any text editor and use Find (Ctrl/Cmd-F).

| To change… | Find this | Notes |
|---|---|---|
| **Cabin price** | `₱4,499` | Appears in the hero, the lineup card, and the order section. Update all three. |
| **Order buttons** | `m.me/orasmartluggage` | Currently opens Messenger. Replace with your Shopee / Lazada / Shopify / checkout link if you have one. |
| **Pre-order prices** | `size__price--muted` | The 22″/24″/26″ cards say "Pre-order". Swap in real prices when ready. |
| **Reviews** | `REVIEWS` | Replace the three sample quotes with real ones, then delete each `<span class="rev-sample">Sample</span>` tag. |
| **Social links** | `orasmartluggage` | Instagram and Facebook are already wired up. |

> **Heads-up on the email signup:** the "Notify me" form looks and feels real but
> only shows a thank-you message — it does **not** store emails yet. To actually
> collect addresses, point it at a free form service like
> [Formspree](https://formspree.io) or your Mailchimp/Klaviyo signup form.

---

## Swapping photos

Replace any file in `assets/` with your own, **keeping the same filename**, and
the site updates automatically. What each file is:

| File | Where it shows |
|---|---|
| `logo-white.png` / `logo-black.png` | Logo (white on dark sections, black on light) |
| `hero.jpg` | Full-screen hero background (black case at the airport) |
| `band-family.jpg` | Full-width B&W range band (after "Why ORA") |
| `inuse-laptop.jpg` | "In use" — laptop + charging |
| `inuse-interior.jpg` | "In use" — layered lining |
| `colorways.jpg` | The three-colour airport lineup (Colors section) |
| `product-gunmetal.jpg` | "Closer look" detail / quote section |
| `band-airport.jpg` | Full-width "Built to board" lifestyle band |
| `brand-dark.jpg` | "The name" story section |
| `gal-wheels.jpg` | Gallery banner — wheels |
| `gal-usb.jpg` | Gallery — USB port + TSA lock |
| `gal-shell.jpg` | Gallery — three-layer shell |
| `gal-pulls.jpg` | Gallery — locking zip pulls |
| `gal-latch.jpg` | Gallery — reinforced latch |
| `ig1.jpg` … `ig6.jpg` | Instagram strip tiles (square) |

For new lifestyle or feature-in-action shots, the easiest path is to swap one of
these files (keep the same filename). Use ~1000–1900px wide JPGs for the big
images and ~640px squares for the `ig#.jpg` tiles to keep the page fast.

---

## Notes

- Works on phones, tablets and desktop; respects reduced-motion settings.
- All styling and scripts are inline in `index.html` — there are no external
  files to load except Google Fonts.
- Currency, specs and sizes reflect the ORA Signature spec sheet. Double-check
  the warranty / shipping wording before publishing — those are intentionally
  left generic.
