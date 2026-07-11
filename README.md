# biased.biz — Static Site (Vercel)

## Deploy
1. Push this repo to GitHub
2. Import in Vercel → framework: "Other" → no build step
3. Domain: www.biased.biz

## Structure
```
/index.html          EN homepage (main)
/de/index.html       DE homepage
/ru/index.html       RU homepage
/assets/style.css    Design system (extracted from IONOS modules)
/vercel.json         Clean URLs config
```

## TODO before launch
- [ ] Replace PHONE placeholder (+49 156 79433747) in all index.html
- [ ] Add favicon
- [ ] Migrate LPs (see map below)

## LP Migration Map (recycle IONOS modules → static pages)
Old IONOS modules use inline styles — they can be pasted 1:1 into new pages,
or refactored to use assets/style.css classes.

| Old (IONOS) | New EN | New DE | New RU |
|---|---|---|---|
| /die-5-saeulen.../ | /5-pillars/ | /de/5-saeulen/ | /ru/5-opor/ |
| /start-up-und-strategie-beratung/ | /strategy/ | /de/strategie/ | /ru/strategiya/ |
| /prozessoptimierung.../ | /operations/ | /de/prozesse/ | /ru/protsessy/ |
| /business-intelligence-und-analytik/ | /analytics/ | /de/analytics/ | /ru/analitika/ |
| /de-vertrieb-und-service/ | /sales-service/ | /de/vertrieb-service/ | /ru/prodazhi/ |
| /de-executive-development/ | /executive/ | /de/executive/ | /ru/razvitie/ |
| LPs (40+) | subpages under each pillar | dito | selektiv (nicht alle) |

Priority: DE has all content (recycle 1:1). EN: translate pillar pages + top-10 LPs.
RU: recycle entry-ru modules + translate top-5 LPs.

## SEO
- hreflang tags on every page (en/de/ru/x-default) — already in homepages
- Each new page needs: title, meta description, canonical
- 301 redirects from old IONOS URLs → add to vercel.json "redirects" once mapping is final
