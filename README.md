# Paul Ann Labs — Astro site

A Trimmie Holdings company. Sister to Paul Ann Media.

---

## Deploy (same pattern as the other two)

1. Create a new GitHub repo named `paulannlabs`
2. Create `.gitignore` in it first so the `main` branch exists
3. Go to `github.com/jclylcj/paulannlabs/upload/main`
4. Open this folder, go **inside** it, Ctrl+A, drag everything onto the page
5. Scroll down, click the green **Commit changes** button
6. Netlify: **Add new project → Import an existing project → GitHub → paulannlabs**
   - Set project name to `paulannlabs` so the URL isn't random
7. Click **Make public** after the first successful deploy
8. Domain management → Add a domain → `paulannlabs.com`
9. GoDaddy DNS for paulannlabs.com:
   - **A** record, name `@`, value `75.2.60.5`
   - **CNAME**, name `www`, value `paulannlabs.netlify.app`

---

## Structure

```
src/
├── layouts/Layout.astro       SEO meta + Organization schema
├── components/
│   ├── Header.astro
│   └── Footer.astro
└── pages/
    ├── index.astro            Positioning, five phases, Stems + Peppermint
    ├── methodology.astro      Strangler Fig in detail + FAQPage schema
    ├── peppermint.astro       Reskilling program, maturity curve + FAQPage schema
    └── about.astro            Origin, internal-owner principle, family

public/
├── robots.txt                 AI crawlers explicitly allowed
└── llms.txt                   Methodology, pricing, and positions for language models
```

---

## Palette

Fig green, distinguishing Labs from Paul Ann Media (teal) and HomeTimeJobs (gold)
while staying in the same navy-grounded family. Green ties to the Strangler Fig
metaphor rather than being arbitrary.

| Token | Hex | Use |
|---|---|---|
| navy | `#1A2F3D` | ground, headers, footers |
| fig | `#4A9D6E` | primary accent, CTAs |
| gold | `#D4883A` | reserved, sparing |
| cream | `#F5F0EB` | page background |
| slate | `#7C8A8A` | secondary text |

---

## Copy decisions worth knowing

**No Empire Express claims anywhere.** The provenance record establishes that the
specific agent systems built at Empire belong to Empire. The site therefore
references the methodology's origin as "doing the work" and "real operations"
without naming a client or claiming any deployed system as a Paul Ann Labs product.
Keep it that way until there's a written agreement saying otherwise.

**Pricing is published.** Phase One at $800–$2,000/mo and the audit at $5,000–$15,000
are stated openly on the methodology page and in llms.txt. This filters inquiries
before they reach a call. Remove it if you'd rather qualify manually.

**"Stopping early is fine" is deliberate.** It disarms the main objection to phased
consulting — that phase one is a wedge for an endless engagement.

---

## Still to do

1. **Logo and favicon** — text wordmark currently. Same treatment as the other two.
2. **Email** — `hello@paulannlabs.com` is referenced throughout and does not exist.
3. **PAL agent product** — referenced in planning but not on the site yet, since it
   doesn't exist. Add when it does.
4. **Case study** — the strongest proof is the Empire work, which is the most
   constrained to publish. The insulation-products engagement is the clean substitute.
