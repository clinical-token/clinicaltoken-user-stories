# Clinical Token Stories

Public clinic and clinician narratives at
[`stories.clinicaltoken.com`](https://stories.clinicaltoken.com).

Separate from:

- Company site — [`www.clinicaltoken.com`](https://www.clinicaltoken.com)
- Investor pitch deck — [`pitchdeck.clinicaltoken.com`](https://pitchdeck.clinicaltoken.com)
- Engineering lab — [`lab.clinicaltoken.com`](https://lab.clinicaltoken.com)

## Structure

| Path | Purpose |
| --- | --- |
| `/` | Stories hub |
| `/stories/<slug>/` | One user story writeup |

## Local

Open any HTML file in a browser, or:

```bash
npx serve .
```

## Deploy (Vercel)

1. Import `clinical-token/clinicaltoken-stories` in Vercel (same GitHub org as www / lab / pitchdeck).
2. Framework preset: **Other** (static).
3. Attach domain `stories.clinicaltoken.com` (DNS via Cloudflare → Vercel).
4. Production branch: `main`.

## Push (this Mac)

Remote uses SSH host alias `github-clinicaltoken`. Load the key once per shell:

```bash
eval "$(ssh-agent -s)" && ssh-add --apple-use-keychain ~/.ssh/id_rsa_github_joe_clinical_token
git checkout main
git push origin main
```
