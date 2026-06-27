# Progress Log — rajathn8.github.io

A running record of everything done on this site, newest first.
See `GAP_ANALYSIS.md` for the outstanding to-do list (benchmarked against `BUILD_SUMMARY.md`).

---

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
