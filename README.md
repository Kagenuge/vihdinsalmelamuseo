# vihdinsalmelamuseo.fi

Website of Salmelan Rustholli, a home museum in Oravala, Vihti. Plain HTML + CSS, hosted on GitHub Pages.

## Edit

Edit `index.html` / `style.css`, preview locally, and push to `main`. Pages deploys automatically.

```sh
python3 -m http.server 8000   # http://localhost:8000
```

## Notes

- Fonts are self-hosted (Libre Caslon Display and Text, Bodoni Moda italic for the hero subtitle, Albert Sans for small labels; latin subset), so there are no third-party requests and no cookie banner is needed.
- Custom domain: add a `CNAME` file containing `www.vihdinsalmelamuseo.fi` only at DNS cutover. Before that it would redirect the github.io preview to a domain that doesn't point here yet.
- Images: each photo comes in a few widths (`img/<name>-<width>.webp`) for `srcset`. To add more, resize the original to WebP at quality ~72, e.g. with `sharp`.
