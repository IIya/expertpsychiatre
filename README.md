# expertpsychiatre.be

Site vitrine du Dr Monique Debauche — expertise psychiatrique médico-légale, Bruxelles.

Static single-page site. No build step, no dependencies, no JavaScript.

## Files

| Path | Purpose |
|---|---|
| `index.html` | The whole site — markup and CSS in one file |
| `fonts/` | Self-hosted Lora (variable, latin + latin-ext) |
| `favicon.svg` | Tab icon |
| `CNAME` | Tells GitHub Pages the custom domain. **Do not delete.** |

## Editing

Open `index.html`, change the text, save. Everything is in that one file.

Preview locally:

```
python3 -m http.server 8765 --directory .
```

Then open http://localhost:8765

## Publishing

```
git add -A && git commit -m "Update text" && git push
```

GitHub Pages rebuilds automatically, live in ~30 seconds.

## Notes

- Fonts are self-hosted deliberately — no request ever goes to Google, which keeps
  the site clean under GDPR. If you add a font, download it into `fonts/` rather
  than linking to a CDN.
- The layout switches from two columns to one below 900px wide.
