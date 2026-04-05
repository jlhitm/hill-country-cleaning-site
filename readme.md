# Hill Country Cleaning Co. — Website

Static HTML site for hillcountrycleaning.co. Hosted on Netlify.

## Structure

- `index.html` — homepage
- `*-house-cleaning.html` — city-specific service area pages
- `q/` — quote calculator tool
- `llms.txt` — LLM crawler hints
- `privacy-policy.html` — legal
- `DEPLOY-NOTES.md` — original deployment guide

## Current Pages

- `/` — homepage
- `/buda-house-cleaning`
- `/kyle-house-cleaning`
- `/south-austin-house-cleaning`
- `/dripping-springs-house-cleaning`
- `/san-marcos-house-cleaning`
- `/cedar-park-house-cleaning`
- `/privacy-policy`
- `/q/` — quote calculator

## Deployment

Deploys via Netlify from this GitHub repo (main branch). Pushes to `main` trigger production builds.

## SEO / AEO

Each location page includes:
- LocalBusiness schema
- FAQ schema
- Location-specific meta description + canonical URL
- Keyword-optimized H1/H2
- GBP map link

Business Profile state tracked in `~/Documents/EmpireBrain/.scripts/gbp-review-state.json`.

## Related Brain Files

- `playbooks/seo-hcc-playbook.md` — SEO strategy and roadmap
- `playbooks/gbp-optimization.md` — Google Business Profile config + updates
- `systems/venture-state.md` — current state snapshot
- `projects/active/hill-country-cleaning.md` — business-level context

## Stack

- Custom HTML/CSS (no framework)
- Netlify hosting
- Originally built by Claude Code
