# SignXOnline — Global Affiliate Site v2

**Live URL:** https://brightlane.github.io/signxonline/  
**Affiliate URL:** https://www.linkconnector.com/ta.php?lc=007949090955004532&atid=signx  
**Build script:** `build.py`

---

## Quick Start

```bash
git clone https://github.com/brightlane/signxonline.git
cd signxonline
python3 build.py
```

Requires Python 3.8+. No external dependencies.

---

## Deploy

Push `build.py` to `main`. Workflow builds and deploys automatically.

**Settings → Pages → Source → GitHub Actions**

---

## Project Structure

```
signxonline/
├── build.py
├── README.md
├── .github/
│   └── workflows/
│       └── deploy.yml
└── dist/                       ← generated on build, never edit manually
    ├── index.html
    ├── assets/style.css
    ├── sitemap.xml
    ├── robots.txt
    ├── llms.txt
    ├── .nojekyll
    ├── 404.html
    ├── {slug}/index.html
    └── {lang}/{slug}/index.html
```

---

## Build Stats

| Metric | Value |
|---|---|
| Total pages | 2,178 |
| Languages | 24 |
| Keyword slugs | 98 |
| Affiliate links per page | 61 |
| Features | 12 |
| Industries | 12 |
| Comparison table rows | 15 |
| Testimonials | 9 |
| FAQ entries | 10 |
| Dependencies | 0 |

---

## Languages (24)

🇬🇧 English · 🇪🇸 Español · 🇫🇷 Français · 🇩🇪 Deutsch · 🇧🇷 Português · 🇯🇵 日本語 · 🇰🇷 한국어 · 🇨🇳 中文 · 🇸🇦 العربية · 🇮🇹 Italiano · 🇷🇺 Русский · 🇳🇱 Nederlands · 🇵🇱 Polski · 🇹🇷 Türkçe · 🇮🇩 Indonesia · 🇸🇪 Svenska · 🇻🇳 Tiếng Việt · 🇮🇳 हिन्दी · 🇲🇾 Melayu · 🇺🇦 Українська · 🇷🇴 Română · 🇨🇿 Čeština

---

## v1 → v2 Upgrades

| | v1 | v2 |
|---|---|---|
| Pages | 1,785 | **2,178** |
| Languages | 22 | **24** (+Czech, +Romanian) |
| Slugs | 84 | **98** |
| Affiliate links/page | 54 | **61** |
| Comparison rows | 13 | **15** (with actual pricing) |
| Testimonials | 8 | **9** (longer, more specific) |
| Pricing tiers | 3 | **4** (added Lifetime plan) |
| Steps | 3 | **4** (added "Signed. Sealed. Stored.") |
| Stats band | Stats bar | **8-item stats band** |
| Social proof | Basic | **6 hero proof items with real numbers** |
| Pricing | Generic | **Actual verified prices: $59/yr, $145 lifetime** |
| Lifetime plan | Not featured | **Dedicated plan card with green highlight** |
| Hero gradient | Single | **Dual radial gradient with green accent** |
| Typography | Standard | **Gradient text on h1 em elements** |
| FAQ depth | Shallow | **10 deep answers including pricing comparison math** |
| llms.txt | 50 lines | **77 lines with pricing data for AI assistants** |
| Footer columns | 4 | **5** (added Pricing column) |
| Ann. bar | Top bar | **Lifetime plan announcement bar** |

---

## Page Sections

1. **Announcement bar** — Indigo bar promoting lifetime plan with direct CTA
2. **Nav** — Dark glass with 5 nav links + CTA button
3. **Hero** — Dual radial gradient, gradient h1, badge row, 6 social proof items
4. **Stats band** — 8 key stats ($59, $145, 50+ countries, $89 saved, 5 min, 30 days, 100%, ISO 27001)
5. **Features** — 12 glowing feature cards (all affiliate)
6. **Industries** — 12 green industry cards (all affiliate)
7. **How it works** — 4-step guide with detailed copy
8. **Why SignX** — 6 value prop cards (left border accent)
9. **Comparison table** — 15-row table vs DocuSign, Adobe Sign, HelloSign with actual prices
10. **Testimonials** — 9 long, specific, business-focused reviews
11. **Pricing** — Free / $59 Premium / **$145 Lifetime** / Enterprise (4 cards)
12. **FAQ** — 10 deep answers including pricing math and legal jurisdiction details
13. **Final CTA** — Gradient banner with pricing hint
14. **Footer** — 5-column with features, industries, comparisons, pricing, language switcher

---

## Customising `build.py`

| Section | What to change |
|---|---|
| `AFFILIATE_URL` | Your LinkConnector URL |
| `BASE_URL` | Change if moving to a custom domain |
| `LANGUAGES` | Add/edit languages and all per-language strings |
| `FEATURES` | Add/remove feature cards |
| `INDUSTRIES` | Add/remove industry cards |
| `COMPARE` | Edit comparison table rows |
| `STATS` | Edit the stats band |
| `TESTIMONIALS` | Edit customer reviews |
| `FAQS_EN` | Edit FAQ questions and answers |
| `PAGE_SLUGS` | Add/remove keyword target pages |
| `CSS` | Edit all styles, colours, effects |
| `build_page()` | Edit HTML structure |

After any change: `python3 build.py`

---

## Post-Deploy Checklist

- [ ] Repo Settings → Pages → Source → **GitHub Actions**
- [ ] Submit `sitemap.xml` to [Google Search Console](https://search.google.com/search-console)
- [ ] Submit `sitemap.xml` to [Bing Webmaster Tools](https://www.bing.com/webmasters)
- [ ] Add `/assets/og-image.png` (1200×630px)
- [ ] Add Google Analytics 4 tag inside `build_page()` `<head>`
- [ ] Verify tracking in your LinkConnector dashboard

---

## Affiliate Disclosure

Commissions earned via LinkConnector. All links use `rel="noopener sponsored"`. FTC-compliant disclosure on every page. SignX® is a trademark of Wondershare Technology Co., Ltd.
