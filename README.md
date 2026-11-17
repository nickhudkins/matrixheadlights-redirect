# matrixheadlights.store

The ACM Technik "Matrix Headlights" explainer page, deployed on Vercel. No build step.

- `how-it-works.html`: the page, served at `/how-it-works` (`cleanUrls`)
- `/` redirects there temporarily (`vercel.json`), so the bare domain still works
- `og.png`: the 1200×630 link-preview image used by the Open Graph and Twitter tags

The **Buy Now** buttons link to the ACM Technik feature builders:
- Volkswagen: https://acmtechnik.com/products/vw-feature-activation-suite
- Audi: https://acmtechnik.com/products/audi-feature-activation-suite

Earlier this repo only redirected the domain to acmtechnik.com. To go back to that, restore the `redirects` block in `vercel.json` from the first commit.
