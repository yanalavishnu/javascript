# hello-jsdelivr

A tiny script that logs `hi` to the console, served from GitHub through [jsDelivr](https://www.jsdelivr.com/).

## Publish

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/<user>/<repo>.git
git push -u origin main
git tag v1.0.0
git push origin v1.0.0
```

## Use

```html
<script src="https://cdn.jsdelivr.net/gh/<user>/<repo>@1.0.0/index.js"></script>
```

Other URL forms:

| URL | Serves |
| --- | --- |
| `https://cdn.jsdelivr.net/gh/<user>/<repo>@1.0.0/index.js` | Pinned to tag `v1.0.0` (recommended) |
| `https://cdn.jsdelivr.net/gh/<user>/<repo>@1.0.0/index.min.js` | Auto-minified by jsDelivr |
| `https://cdn.jsdelivr.net/gh/<user>/<repo>@main/index.js` | Latest on `main` (cached up to 12h) |
| `https://cdn.jsdelivr.net/gh/<user>/<repo>/index.js` | Latest tagged release |

To bust the cache for a branch URL, visit `https://purge.jsdelivr.net/gh/<user>/<repo>@main/index.js`.
