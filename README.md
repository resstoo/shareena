# شارعنا يستاهل — Campaign Studio

Private, buildless planning workspace for an Egyptian anti-littering campaign.

## Run
No build or package installation is needed. With Python 3 installed, run from the repository root:

```bash
python -m http.server 8000 --directory dist
```

Open http://localhost:8000. Stop the server with Ctrl+C. You can also serve `dist/` with any static web server.

### تشغيل محلي
شغّل الأمر السابق من مجلد المشروع، وافتح الرابط المحلي. الموقع يدعم العربي والإنجليزي، والاختيارات محفوظة في نفس المتصفح.

### Files
- `dist/index.html`: page structure.
- `dist/style.css`: responsive styling and RTL layout.
- `dist/data.js`: campaign content and planning data.
- `dist/i18n.js`: Arabic translation catalog and formatting.
- `dist/app.js`: interactions, budgeting and saved planning state.
- `dist/exports.js`: English copied-plan and creator-brief text.
- `docs/`: verified Arabic and English screenshots.

The existing hosted site uses access controls supplied by its hosting platform. This portable frontend does not implement authentication itself. Publishing this source repository does not enable a public website.

## Languages
Arabic is the default, with a persistent Arabic/English switch in the top bar. Arabic uses right-to-left navigation, Noto Sans Arabic typography, localized numbers and EGP amounts, translated accessible names, and localized plan/creator-brief exports. Language switching shares the same existing planning state and localStorage key.

## Experience
- Compare smart provocation, street pride, and a combined approach.
- Compare an independent organization with a hosted-pilot bridge.
- Explore 30 Egyptian Arabic message variants across five audiences and three tones; save a shortlist.
- Work through a 12-item, three-phase 90-day roadmap.
- Adjust budget assumptions and four normalized priorities; inspect whole-bin affordability and operational trade-offs.
- Track placement readiness; explore partners, celebrity creative roles, and seven risks.
- Copy a current working-plan summary.

Preferences are saved to localStorage in the current browser. There is no backend, payment collection, external outreach, analytics, or cloud synchronization of planning state. Fonts use Google Fonts with local system fallbacks.

## Assumptions
The campaign is a concept, not an established registered organization. Costs and targets are illustrative planning values. Operating capacity, permissions, fundraising route, and quotes must be confirmed. Partner organizations are prospective learning contacts, and celebrity roles are casting ideas with no commitments.

Official reference pages reviewed 26 October 2026:
- https://green-ish.org/en/about-us/
- https://verynile.org/

## Validation
Desktop browser checks covered approach/model changes, audience/tone/variant changes, shortlisting, copying, keyboard tabs, budget changes/invalid inputs/zero budget, readiness checks, roadmap persistence, risk filtering, and disclosures. Phone (390px frame) and tablet (768px frame) layouts were reviewed; phone overview, messaging, and funding had no horizontal page overflow. Mobile drawer hides background controls and restores section access. Calculator invariants passed 140 budget/weight/cost scenarios. HTML IDs, local assets, fragment targets, and JS syntax were checked. Validation-only checklist selections and message shortlist entries were removed.

`docs/preview.jpg` records the validated overview. Hosting remains owner-private unless the owner explicitly approves a future audience change.

## Arabic localization validation (26 October 2026)
All 459 initial catalog entries plus numeric labels cover static copy and all audience, roadmap, readiness, and risk data. JS syntax passed. Browser QA verified language and direction switching, preserved audience/tone/shortlist, approach/model, budget, readiness and roadmap selections across reload, localized errors, and copying plans and creative briefs in both languages. Risk filters and open details survive locale changes. Arrow-key tab movement follows LTR/RTL direction. Responsive frames at 390px and 768px were visually reviewed; Arabic overview, funding and messages had no horizontal page overflow. The mobile drawer opens on the right for Arabic and left for English. No audience or access changes were requested or made.

## Source snapshot
Exported from the validated Arabic/English site source commit `7f3ebe33ffd30edfaa7b41f6ae1e3478a4e6c4e1`. Hosting credentials, platform project configuration and browser planning data are excluded from this portable source snapshot.
