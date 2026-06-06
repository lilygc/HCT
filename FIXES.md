# HCT – Future Fixes & Minor Improvements

Items to apply in a future session. Mark `[done]` when complete rather than deleting.

---

## Visual / UI
- [ ] Confirm reserved color #7C9080 (muted sage-green) is used or earmarked somewhere in the palette
- [ ] Review mobile layout of category tiles on small screens (iPhone SE)
- [ ] Back-to-top button: verify it doesn't overlap nav on narrow viewports

## Content / Data
- [ ] Populate empty categories: Civil War, Gulf War, Korean War, WWI, WWII, Iraq/Afghanistan, MST, Documentaries & Films, Highly Rated, Women Veterans
- [ ] Verify "1st Person Narratives – Iraq and Afghanistan" tag matches spreadsheet exactly

## Functionality
- [ ] AI recommendation search bar requires Anthropic API key + backend relay (Netlify Function) — not yet wired up
- [ ] Consider migrating from GitHub Pages to Netlify to enable backend features (AI search, analytics)
- [ ] Add Google Analytics
- [ ] Create favicon from the water lily / purple heart emblem

## Domain Setup
Primary domain: **HealingCombatTrauma.com** (GoDaddy) — canonical destination for all traffic.
All others redirect to .com.

### HealingCombatTrauma.com → GitHub Pages (GoDaddy)
- [ ] In GoDaddy DNS, add CNAME record: name `www`, value `lilygc.github.io`
- [ ] In GoDaddy DNS, add four A records (root domain) pointing to GitHub's IPs:
  - `185.199.108.153`
  - `185.199.109.153`
  - `185.199.110.153`
  - `185.199.111.153`
- [ ] In GitHub repo: Settings → Pages → Custom domain → enter `healingcombattrauma.com`
- [ ] Confirm HTTPS certificate auto-provisions (may take a few minutes)

### HealingCombatTrauma.org → redirect to .com (Hover)
- [ ] In Hover dashboard, use Domain Forwarding to redirect to `https://healingcombattrauma.com`

### PTSD domains (e.g. HealingPTSD.com / .org)
- [ ] Redirect all to `https://healingcombattrauma.com` for now
- [ ] Revisit once site is live — could eventually point to the PTSD Resources category page (good for SEO)

### WordPress
- [ ] Delete/cancel WordPress site — no longer needed
- [ ] If on WordPress.com, let plan lapse or delete under account settings

## Known Bugs
- [ ] (Add items here as you notice them)

---

*To apply fixes: paste relevant items into a new Claude session along with the current index.html.*
