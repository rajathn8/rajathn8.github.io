# Progress Log — rajathn8.github.io

A running record of everything done on this site, newest first.
See `GAP_ANALYSIS.md` for the outstanding to-do list (benchmarked against `BUILD_SUMMARY.md`).

---

## 2026-06-28

### Structured data + OG image + IndexNow + cleanup (autonomous batch)
- **JSON-LD:** added `WebSite`, `ProfilePage`, `BreadcrumbList`, and `FAQPage` (5 recruiter Q&As → eligible for rich snippets) to `index.html`.
- **Branded OG image:** generated `assets/images/og-image.png` + `.webp` (1200×630, navy + orange) and pointed `og:image`/`twitter:image` on home/resume/blog to it. Person JSON-LD `image` left as the real photo.
- **IndexNow:** created key file `280477f6f4b541e6b002ae0a575cc1b3.txt` and submitted all 4 URLs to the IndexNow API (Bing/Yandex/Seznam). No account required.
- **Cleanup:** deleted unreferenced stray root PNGs `theme.png` (4.6MB) + `evereset_walk_1.png` (3.7MB) — ~8.4MB.
- **README:** fixed wrong live-site URL (`/rajath_rao_resume_2026` → `https://rajathn8.github.io/`).
- **Note:** cache-busting `?v=` is N/A — all CSS is inline, no external CSS/JS links. `css/style.css` is orphaned/unreferenced (left in place).

## 2026-06-27

### Performance + SEO files + crawlers (batch)
- **SEO files added:** `llms.txt`, `humans.txt`, `ai.txt`, `ads.txt`, `feed.xml`, `.well-known/security.txt`.
- **Geo SEO:** added `geo.region`, `geo.placename`, `ICBM`, `og:locale=en_GB`, and RSS `<link rel="alternate">` to home.
- **Crawlers:** expanded `robots.txt` from ~7 to ~26 named agents (search + AI/LLM bots).
- **Image sitemap:** `sitemap.xml` now lists images + uses `image:` namespace; dates bumped to 2026-06-27.
- **Performance (WebP):** converted all 12 `assets/images` files to WebP (9.05MB → 5.54MB, saved 3.5MB). Swapped the 5 referenced `<img>` tags (hiking, lake-reflection, everest-base-camp, IMG_0143, himalaya-trek) to `.webp`; kept `profile-home.png` as PNG for social cards.

### Setup
- Studied `BUILD_SUMMARY.md` (the `engineer-rama-rao.github.io` playbook) as the gold standard.
- Audited this repo against it and wrote `GAP_ANALYSIS.md` listing everything not yet done.
- Created this progress log to track all future work.
