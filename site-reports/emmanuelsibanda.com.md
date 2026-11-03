# Site report — emmanuelsibanda.com

**Scan run:** 2026-11-03 (UTC), fresh production fetch — `Cache-Control: no-cache`, `www.emmanuelsibanda.com`, plus headless browser render. Not Otto pool cache.

**Production URL checked:** https://www.emmanuelsibanda.com/

---

# Summary

Welcome to your trial for **emmanuelsibanda.com**. I re-ran the scan from scratch against what Vercel is serving on your main domain today (not cached Otto analytics — none are connected yet).

**Bottom line for ownership:** Production still shows your **generalist “business problems → working systems”** homepage, not the newer **hospitality & tourism automation** positioning. Google is starting to pick up hospitality language in some results, but the live HTML/JS bundle on `www` has not switched yet — so buyers and search engines can see different versions of you. The site also **failed Google PageSpeed (page hung)** in lab testing, and **`/sitemap.xml` returns your homepage HTML instead of a sitemap**, which hurts crawl clarity.

---

# Score

- **Overall Score:** `32` / 100 (`Poor`)
- **Website Health & Speed:** `52` / 100 (`1` page checked; `1` H1 present; `0` images missing alt on `/`; `0` missing meta descriptions in shell; PageSpeed lab **failed — page hung**; visible copy is thin ~`37` words after JS render)
- **Search & AI Visibility:** `12` / 100 (Weak match on Puerto Rico hospitality buyer searches; **no** durable `site:emmanuelsibanda.com` index in spot checks; AI-style “recommend consultants by name” queries surface **industrial** firms, not Emmanuel Sibanda)
- **Connected Sources:** None (GA4, GSC, Meta not connected)

---

# What's costing you customers

1. **Production vs. what you expect “live” — positioning split**
   - **What this means for you:** If you already shipped the hospitality landing page, it is **not** what every visitor gets at `https://www.emmanuelsibanda.com/` yet. Today’s production title is still *“From business problems to working systems”* and the rendered H1 is a long generalist product-engineer pitch — not *“Automation for Puerto Rico’s hotels, venues, and travel agencies.”*
   - **Evidence:** Fresh fetch `2026-11-03` — HTML shell + `main.11024589.js` (Vercel `last-modified` 2026-11-02). Some Google result snippets show hospitality copy ahead of the CDN bundle — that inconsistency confuses both buyers and rankings.

2. **Invisible or weak on high-intent Puerto Rico buyer searches**
   - **“hospitality automation puerto rico”** — top results are operators/software vendors (e.g. ForReal 360, Innat8, PMI-style property tech), not your domain.
   - **“tourism automation consultant in puerto rico”** — index signals vary; do not rely on a one-off snippet until production copy and Search Console confirm impressions.
   - **“ai automation services puerto rico”** — IslaIntel, Romero Automations, 787 Solutions, Pintado.AI, and similar own the page.

3. **Lab performance failure (PageSpeed / Lighthouse)**
   - **What this means for you:** Google’s lab could not finish loading the page (**PAGE_HUNG**). That matches what we saw in the browser (hard to reach “fully settled” load). Mobile GMs on weak hotel Wi‑Fi may bail before your offer renders.

4. **Broken sitemap + thin rendered homepage**
   - `/sitemap.xml` returns the SPA shell, not XML — crawlers get no URL list.
   - After JavaScript runs, the homepage exposes about **37 words** of indexable text — thin for competitive Puerto Rico automation keywords.

5. **Zero AI-assistant brand recall for hospitality automation**
   - Broad “best automation consultants in Puerto Rico” style queries recommend **industrial / manufacturing integrators** (JC Automation, Principia, CSE, etc.), not hospitality-focused consultants — your positioning is not yet established in public, structured copy at production.

---

# Fix plan

1. **Promote the hospitality build to production (or give Otto the preview URL)**
   - **Where:** Vercel production alias for `www.emmanuelsibanda.com`
   - **What Otto will change:** Confirm the deployment you see in the browser is the one wired to **production**, then re-scan. If it is still preview-only, say **Deploy** and we promote + verify.

2. **Align title, meta, H1, and body to Puerto Rico hospitality buyers**
   - **Where:** Homepage `/`
   - **What Otto will change:** One clear H1 (hospitality + Puerto Rico), supporting H2 sections (hotels, venues, travel agencies), meta title/description/OG tags that match — so Google, social previews, and humans see the same story.

3. **Fix `/sitemap.xml` and add crawl paths**
   - **Where:** Static/sitemap config on Vercel
   - **What Otto will change:** Valid XML sitemap listing `/` and any service sections; submit via Search Console once connected.

4. **Stabilize performance until PageSpeed completes**
   - **Where:** `/` bundle load chain
   - **What Otto will change:** Diagnose hang (long tasks, blocking JS, hero image), reduce main-thread work, retest until PSI returns a score instead of PAGE_HUNG.

5. **Connect GA4 + Search Console**
   - **What this means for you:** Weekly traffic, queries, and form clicks in your reports instead of guesswork.
   - **Blocker:** Reviewer connects integrations in Otto Settings — one ask when you are ready.

---

# Scan details (sources used)

| Check | Result |
|--------|--------|
| HTTPS production HTML | Title: *Emmanuel Sibanda \| From business problems to working systems* |
| Headless render (6s) | H1 present; 1 image with alt; ~37 words body text |
| PageSpeed Insights (mobile) | **Failed — PAGE_HUNG** |
| `/sitemap.xml` | Returns HTML shell (invalid) |
| Otto pool / analytics cache | Empty — not used for this report |
| Connected integrations | PSI platform key only |

*Prioritized next step:* Confirm whether the hospitality page is **preview-only** or **production** — reply with **Proceed** if you want Otto to align production to that version and re-run the scorecard after deploy.
