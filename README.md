# Alura Research Desk

A mobile-friendly research dashboard for daily Basic-plan limits, research links, keyword and competitor findings, session notes, and recorded activity history.

## Privacy

The site is reachable on GitHub Pages. Research content is encrypted in `data.js` using AES-GCM with a password-derived key. This is a light privacy lock, not an account or access-control service. No passwords, personal income, client names or account credentials belong in dashboard content. Plaintext data must never be committed. Search engines are asked not to index the site.

## Updating

1. Prepare the sanitized source JSON outside the repository history.
2. Preserve unknown quota values as unknown. Logged activity counts are not confirmed quota debits.
3. Encrypt with `node scripts/encrypt.mjs <source.json> <password-file> data.js`.
4. Test the page, filters, date history, wrong-password state, unlock and lock. Inspect phone and desktop layouts.
5. Commit only application assets and encrypted `data.js`. Publish from `main`, root directory.
6. Check the deployed site and record the research checkpoint time. No live Alura polling runs in this site.

Daily research session: 22:00 Asia/Kolkata. That is the research session time, not a claim about Alura's reset timezone. Monthly AI credits, API credits and daily research quotas are separate.
