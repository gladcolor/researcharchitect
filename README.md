# Research Architect

Landing page for [researcharchitect.ai](https://researcharchitect.ai) — AI systems that design research, not just execute it.

## Hosting

- **GitHub Pages** serves the static site from the `master` branch
- **Cloudflare** manages DNS for `researcharchitect.ai`

## Setup

### Cloudflare DNS Records

Add these DNS records in Cloudflare dashboard for `researcharchitect.ai`:

| Type  | Name | Content                      | Proxy |
|-------|------|------------------------------|-------|
| CNAME | @    | `<github-username>.github.io` | DNS only (gray cloud) |
| CNAME | www  | `<github-username>.github.io` | DNS only (gray cloud) |

> Replace `<github-username>` with your GitHub username or organization name.

### GitHub Pages

1. Go to repo **Settings → Pages**
2. Set Source to **Deploy from a branch**, branch: `master`, folder: `/ (root)`
3. Custom domain: `researcharchitect.ai`
4. Check **Enforce HTTPS** (after DNS propagates)
