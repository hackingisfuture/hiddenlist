# poctabaahimohsin

Static host for proof-of-concept pages used in **authorised** security testing.

Published at: `https://hackingisfuture.github.io/poctabaahimohsin/`

## Layout

| path | purpose |
|---|---|
| `poc/` | your PoC pages — publish at `/poc/<name>.html` |
| `templates/` | starting points (CSRF, postMessage, CORS) |
| `.nojekyll` | tells Pages to serve raw HTML without Jekyll processing |

## Adding a PoC

```bash
cp templates/csrf.html poc/target-csrf.html
# edit it, then
git add poc/ && git commit -m "add poc" && git push
```

Live within ~60s at `/poc/target-csrf.html`.

## Note

This repo is **public** — GitHub Pages requires it on the free plan. Do not commit
session cookies, tokens, or customer data. Reference targets by hostname only.
