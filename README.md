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

## Before you publish: fill in the brackets

Search both HTML files for `[` and replace every bracketed placeholder:

- Street address, phone, and careers email (footer of both pages, and the "How to apply" section)
- Head capacity, year established, and employee count (the facts strip on the home page)
- Pay ranges on each job listing
- Hiring manager name in "Stop by"
- Replace `https://joinhandshake.com` with your actual Handshake employer profile URL once you have it

## Editing job listings

Open `careers.html` and find the `<div class="jobs">` block. Each `<article class="job">` is one posting.
Copy a block to add a job, delete a block to remove one, and update the `data-updated` date.

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
