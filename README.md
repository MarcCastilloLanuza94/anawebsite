# anabujosa.com

Ana Bujosa's product portfolio: one static page listing every live product with links and highlight stats.

## Structure

- `index.html` — the whole site. No build step, no dependencies. Styles are inline; fonts load from Google Fonts.

## Preview locally

Open `index.html` in a browser, or serve the folder:

```bash
npx --yes serve .
```

## Deploy

The repo is a plain static site, so any host works. On Vercel:

```bash
npx vercel --prod
```

Then add `anabujosa.com` as a domain in the Vercel project and point the DNS at Vercel.

## Updating stats

All numbers live in `index.html` inside each `<article class="card">`. Each stat is a `.stat` tile with a number (`.n`) and a label (`.l`). Dated stats say so in the label, so update the date when you refresh the number.
