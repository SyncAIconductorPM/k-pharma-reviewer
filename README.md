# K-PharmaReviewer AI

Static cockpit for MFDS-style drug review.
Target custom domain: `https://pharma.weagentic.ai`

## Cloudflare Pages (free)

1. [dash.cloudflare.com](https://dash.cloudflare.com) → Workers & Pages → Create → Pages → Connect to Git.
2. Repository: `SyncAIconductorPM/k-pharma-reviewer`
3. Build: no command. Output directory: `/`
4. After first deploy you get `https://k-pharma-reviewer.pages.dev`
5. Custom domain: Pages → Custom domains → `pharma.weagentic.ai`

`weagentic.ai` is not registered yet. Buy or transfer the apex to Cloudflare, then add a CNAME:

```
pharma  CNAME  k-pharma-reviewer.pages.dev
```

Or Pages custom domain wizard will create the record if the zone is on Cloudflare.
