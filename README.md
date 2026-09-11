# Herd Co. website

Static company website for Herd Co., Inc. (Bartlett, Nebraska). Built for GitHub Pages and used as the
employer website on Handshake.

## Files

| File | What it is |
| --- | --- |
| `index.html` | Home page: who we are, how the yard works, values, careers teaser, contact |
| `careers.html` | Job listings and how to apply. This is the page to link from Handshake. |
| `style.css` | All styling, light and dark theme |
| `favicon.svg` | Browser tab icon |

## Logo and colors

`logo.png` / `logo-dark.png` are cleaned-up versions of the original Herd Co logo scan (flat colors, transparent
background). The `-800` files are smaller copies used in the page header. The site palette in `style.css` comes
from the logo: near-black brown `#221E19`, tan `#B29E88`, warm grey `#C0B5A5`, white.

## Apply buttons

The Apply buttons on the careers page link to Handshake. Replace `https://joinhandshake.com` in `careers.html`
with the actual Handshake posting URL. Keep Handshake mentions light on the page; the site does not claim it is
the only way to apply.

## Editing job listings

Open `careers.html` and find the `<div class="jobs">` block. Each `<article class="job">` is one posting.
Copy a block to add a job, delete a block to remove one, and update the `data-updated` date. The current
listing is the Accountant / Controller position from "Herd Co Controller Position Job Posting.pdf".

## Publishing on GitHub Pages

The site lives in the `herd-co/herd-co.github.io` repository, which GitHub publishes automatically at:

- Home: https://herd-co.github.io/
- Careers (link this from Handshake): https://herd-co.github.io/careers.html

Every `git push` to `main` republishes the site within a minute or two. To push a change from this folder:

```bash
git add -A
git commit -m "Update job listings"
git push
```

## Using a custom domain (optional)

If you buy a domain such as `herdcocattle.com`, add it under **Settings > Pages > Custom domain** and point
the domain's DNS at GitHub Pages per their instructions. Handshake accepts either the github.io URL or a
custom domain as the company website.
