# AfroLearn — Landing Page

Public landing page for AfroLearn, a Pan-African STEAM education framework and curriculum
in active development. Per project framing discipline, the site presents AfroLearn as a
framework + curriculum with a platform **in development** — not an operational platform.

## What this is

A single, self-contained `index.html` (inline CSS + JS, Google Fonts as the only external
dependency). No build step, no framework.

Sections: hero, how-it-works, pattern decoder (interactive), the gap, approach (Ubuntu /
Ma'at / Sankofa), who-it's-for, curriculum consulting, partners, contact form, footer.

## Run locally

Open `index.html` in a browser, or serve it:

```sh
npx serve .        # or: python3 -m http.server
```

The contact form detects `file://` and shows a success state without submitting.

## Deploy

Hosted on **Netlify** (static publish of `.`). The contact form uses **Netlify Forms**
(`data-netlify="true"` + honeypot) — submissions appear in the Netlify dashboard with no
backend. Deploy with:

```sh
npx netlify-cli deploy --prod --dir .
```

## Source

Adapted from a Claude-generated artifact; the Claude artifact preview harness (postMessage
bridge, screenshot script) and absolute artifact URLs were stripped for hosting.
