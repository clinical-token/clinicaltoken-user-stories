# Clinical Token User Stories

Public clinic and clinician narratives at
[`userstories.clinicaltoken.com`](https://userstories.clinicaltoken.com).

Separate from:

- Company site — [`www.clinicaltoken.com`](https://www.clinicaltoken.com)
- Investor pitch deck — [`pitchdeck.clinicaltoken.com`](https://pitchdeck.clinicaltoken.com)
- Engineering lab — [`lab.clinicaltoken.com`](https://lab.clinicaltoken.com)

## Structure

| Path | Purpose |
| --- | --- |
| `/` | User stories hub |
| `/user-stories/<slug>/` | One user story writeup |

## Writing guidelines

- **Keep every user story under 5 minutes of reading time.** Aim for roughly 1,000 words or less (about 200–250 words per minute). Show an explicit `N min read` line near the top of the article.
- Prefer one clear clinical workflow, one finding, and one call to action. Cut secondary tangents so busy clinicians can finish the story in a single sitting.
- Use Clinical Token AI agents (not bare “agents”) when referring to software, so readers do not confuse them with human staff.

## Local

Open any HTML file in a browser, or:

```bash
npx serve .
```

## Deploy (Vercel)

1. Import `clinical-token/clinicaltoken-user-stories` in Vercel (same GitHub org as www / lab / pitchdeck).
2. Framework preset: **Other** (static).
3. Attach domain `userstories.clinicaltoken.com` (DNS via Cloudflare → Vercel).
4. Production branch: `main`.

## Push (this Mac)

Remote uses SSH host alias `github-clinicaltoken`. Load the key once per shell:

```bash
eval "$(ssh-agent -s)" && ssh-add --apple-use-keychain ~/.ssh/id_rsa_github_joe_clinical_token
git checkout main
git push origin main
```
