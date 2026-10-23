# matrixheadlights.store → acmtechnik.com

A tiny Vercel project that permanently (301/308) redirects every URL on its domain to https://acmtechnik.com/.
`vercel.json` does the redirect; `index.html` is only a fallback.

## Deploy (pick one)

**From a terminal (fastest):**
```
cd matrixheadlights-redirect
npx vercel --prod
```
Log in when asked, accept the defaults. No build step or framework needed.

**From GitHub:** push this folder to a new repo, then on vercel.com click **Add New → Project**, import the repo, and click **Deploy** (Framework preset: Other).

## Point matrixheadlights.store at it

1. In the Vercel project, open **Settings → Domains**, add `matrixheadlights.store` and `www.matrixheadlights.store`.
2. Vercel shows the DNS records to create. Usually:
   - `A` record, host `@`, value `76.76.21.21`
   - `CNAME` record, host `www`, value `cname.vercel-dns.com`
   Always use the exact values Vercel shows for your project.
3. In **Hover → matrixheadlights.store → DNS**, delete any existing `@`, `*` and `www` records (including Hover's forwarding A records to 216.40.34.41) and remove any Hover forward you set up, then add the records from step 2.
4. Wait for Vercel to show the domains as valid (minutes to a few hours). Vercel issues the HTTPS certificate automatically, so both http:// and https:// redirect cleanly.
