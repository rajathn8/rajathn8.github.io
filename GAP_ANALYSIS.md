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
- [ ] `llms.txt` — LLM-readable resume (ChatGPT/Perplexity/Claude read it)
- [ ] `humans.txt`
- [ ] `ai.txt` — explicit AI train/embed/cite allow
- [ ] `ads.txt` — "no ad relationships" professional signal
- [ ] `feed.xml` — RSS feed
- [ ] `.well-known/security.txt` — RFC 9116
- [ ] Image sitemap (none of our images are in `sitemap.xml`)
- [ ] Geographic SEO meta: `geo.region`, `ICBM`, `og:locale`
- [ ] Cache-busting `?v=` query strings on CSS/JS

### Structured data (we have 1 graph; playbook has 6 blocks)
- [ ] `WebSite` schema
- [ ] `ProfilePage` schema
- [ ] `FAQPage` schema → rich snippets in Google
- [ ] `BreadcrumbList` schema
- [ ] (Optional, if job-seeking) `JobPosting` self-as-candidate

### Search-engine registration
- [ ] Bing Webmaster verification (`BingSiteAuth.xml`)
- [ ] IndexNow key file + URL submission (Bing/Yandex/Seznam)

### Crawler coverage
- [ ] robots.txt only names 7 AI agents; playbook names ~20
      (missing OAI-SearchBot, Bytespider, Applebot-Extended, MistralAI-User,
      cohere-ai, Amazonbot, FacebookBot, LinkedInBot, PiplBot, archive.org_bot, etc.)

### Performance / images
- [ ] Zero WebP — all images are JPG/PNG
- [ ] Large unoptimized hero images: `everest-base-camp.jpg` 2.6MB, `hiking.jpg` 2.6MB, `lake-reflection.jpg` 0.9MB
- [ ] Two huge stray root PNGs likely unused: `theme.png` 4.6MB, `evereset_walk_1.png` 3.7MB (candidates to delete or move)
- [ ] No dedicated branded 1200×630 OG image (we reuse `profile-home.png`)

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
- [ ] `README.md` live-site URL is wrong (`/rajath_rao_resume_2026` — should be `https://rajathn8.github.io/`)

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
