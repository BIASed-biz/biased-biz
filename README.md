# biased.biz — Static Site (Vercel)

Concept: BI³AS³ed is a *model* for how a healthy business works (5 pillars).
Home = "university" (teaching, no hard sell). Landing pages carry the CTA.

## Deploy
1. Push to GitHub → import in Vercel (framework: Other, no build step)
2. Domain: www.biased.biz
3. Contact: hello@biased.biz · +49 156 79433747 (mail + phone only, no forms)

## Structure
- `/` EN homepage (main) · `/de/` · `/ru/`
- 5 hubs per language: strategy/operations/analytics/sales-service/executive (+ 5-pillars)
- LPs under each hub. EN + DE complete (~43 each). RU selective (7 LPs).
- `/assets/style.css` design system · `/favicon.svg` · `/vercel.json` redirects+cleanUrls

## SEO / GEO
- Every page: title, meta description, favicon
- Homepages: hreflang (en/de/ru/x-default)
- LPs: university-tone sections + GEO-optimized FAQ + CTA + hub back-link
- 46× 301 redirects from old IONOS URLs → new (German LPs → /de/, Russian → /ru/)
- Home (/) stays EN; old German homepage had no separate path

## Status
✅ EN + DE LPs complete · ✅ RU 7 LPs + 6 hubs · ✅ redirects · ✅ favicon
⬜ IONOS forwarding — NOT yet activated (final step, when everything is confirmed)
⬜ Optional: expand RU coverage further

## Redirect note
Old IONOS URL tree is mapped 1:1 in vercel.json. Home / needs no redirect (it IS the new EN home).
If the old German homepage lived at a distinct path, add one redirect → /de/.
