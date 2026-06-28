# Gap Analysis — rajathn8.github.io vs. the Rama playbook

Benchmark: `BUILD_SUMMARY.md` (the `engineer-rama-rao.github.io` build).
This file lists what that build has that **this** site does **not** yet have.
Audited: 2026-06-27.

---

## ✅ What we already have

- 4 pages: `index.html`, `about.html`, `resume.html`, `blog.html`
- Core SEO meta on home: description, keywords, author, canonical, OG, Twitter card
- 1 JSON-LD graph (Person + Organization + EducationalOrganization + Credential + PostalAddress)
- `robots.txt` (allows ~7 AI crawlers)
- `sitemap.xml` (4 page URLs)
- Google Search Console verification file (`google648f3bf0a48ad896.html`)
- `favicon.svg`
- Full résumé PDF (`assets/Rajath_Rao_Resume.pdf`)

---

## ❌ What we DON'T have / haven't done

### SEO & discoverability files
- [x] `llms.txt` — LLM-readable resume (ChatGPT/Perplexity/Claude read it) — done 2026-06-27
- [x] `humans.txt` — done 2026-06-27
- [x] `ai.txt` — explicit AI train/embed/cite allow — done 2026-06-27
- [x] `ads.txt` — "no ad relationships" professional signal — done 2026-06-27
- [x] `feed.xml` — RSS feed — done 2026-06-27
- [x] `.well-known/security.txt` — RFC 9116 — done 2026-06-27
- [x] Image sitemap — done 2026-06-27
- [x] Geographic SEO meta: `geo.region`, `ICBM`, `og:locale` — done 2026-06-27
- [n/a] Cache-busting `?v=` on CSS/JS — N/A, all CSS is inline, no external CSS/JS

### Structured data (we have 1 graph; playbook has 6 blocks)
- [x] `WebSite` schema — done 2026-06-28
- [x] `ProfilePage` schema — done 2026-06-28
- [x] `FAQPage` schema → rich snippets in Google — done 2026-06-28
- [x] `BreadcrumbList` schema — done 2026-06-28
- [ ] (Optional, if job-seeking) `JobPosting` self-as-candidate — needs your decision

### Search-engine registration
- [ ] Bing Webmaster verification (`BingSiteAuth.xml`) — needs your Bing login
- [x] IndexNow key file + URL submission (Bing/Yandex/Seznam) — done 2026-06-28 (HTTP 202)

### Crawler coverage
- [x] robots.txt expanded from ~7 to ~26 named search + AI agents — done 2026-06-27

### Performance / images
- [x] WebP — all 12 images converted (9.05MB → 5.54MB) — done 2026-06-27
- [x] Large hero images optimized + `<img>` tags swapped to WebP — done 2026-06-27
- [x] Stray root PNGs `theme.png` + `evereset_walk_1.png` deleted (~8.4MB) — done 2026-06-28
- [x] Branded 1200×630 OG image (`og-image.png`/`.webp`); og/twitter image swapped on home/resume/blog — done 2026-06-28

### Contact / conversion (lighter on this site by design, but available levers)
- [ ] vCard (`.vcf`) one-tap contact save
- [ ] QR code (PNG + SVG) for print/in-person
- [ ] 1-page CV variant
- [ ] Word `.docx` CV source published
- [ ] Business-card PDF
- [ ] Calendly booking link
- [ ] WhatsApp / SMS deep-link CTAs
- [ ] `tel:` phone CTA
- [ ] Contact / intake form

### Housekeeping
- [x] `README.md` live-site URL fixed — done 2026-06-28

---

## Suggested priority order (highest SEO ROI first, lowest effort)

1. `llms.txt`, `humans.txt`, `ai.txt`, `ads.txt`, `.well-known/security.txt` — pure text, minutes
2. Expand robots.txt AI crawler list
3. Add `WebSite` + `ProfilePage` + `FAQPage` + `BreadcrumbList` JSON-LD
4. Geo meta + image sitemap + `feed.xml`
5. Bing + IndexNow registration
6. WebP image optimization + delete stray root PNGs
7. Fix README URL
8. (Optional) contact/conversion levers — only if you want inbound contact
