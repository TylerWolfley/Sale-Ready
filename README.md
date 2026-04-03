# Sale Ready Austin Static Site

A lightweight static homepage for Sale Ready Austin, built with semantic HTML, modern CSS, and small vanilla JavaScript.

## Project structure

```text
/
  index.html
  README.md
  /assets
    /css
      styles.css
    /js
      main.js
    /images
      logo.png
      /gallery
        project-01-before.svg
        project-01-after.svg
        project-02-before.svg
        project-02-after.svg
        project-03-before.svg
        project-03-after.svg
        project-04-before.svg
        project-04-after.svg
        project-05-before.svg
        project-05-after.svg
        project-06-before.svg
        project-06-after.svg
```

## Where to swap the logo

- Replace `/assets/images/logo.png` with the final logo file.
- The same file is used in the header, hero panel, and footer.
- If the final filename changes, update the `img` references in `/index.html` and the JSON-LD logo URL in the `<head>`.

## Where to update phone, email, and service area

Edit `/index.html` in these spots:

- hero and final CTA buttons (`sms:` and `mailto:` links)
- contact block in the final CTA section
- footer contact links
- SEO structured data in the JSON-LD block inside `<head>`

Current placeholders:

- Phone: `(512) 555-0189`
- Email: `hello@salereadyaustin.com`
- Service area: `Austin, TX and surrounding areas`

## Where to replace gallery placeholders

- Swap the files in `/assets/images/gallery/` with real before-and-after images.
- Keep the same filenames if you want the existing markup to keep working.
- Each project card in `/index.html` already points to the matching before/after file pair.

## Where to edit hero copy and service cards

- Hero copy lives near the top of `/index.html` inside the `.hero` section.
- The quick value strip is directly below the hero.
- Service cards live in the `#services` section.
- Audience, gallery captions, process steps, scope lists, and final CTA copy are all editable in `/index.html`.

## JavaScript behavior

`/assets/js/main.js` handles:

- mobile menu toggle and close behavior
- sticky header state on scroll
- current year in the footer
- light reveal-on-scroll behavior

## Static deployment

This project does not require a build step.

Deploy options:

1. Upload the repository contents to any static host.
2. Point the host to serve `index.html` from the site root.
3. Update the canonical URL, Open Graph URL, Open Graph image, favicon files, and JSON-LD placeholders in `/index.html` before production launch.

Good fits include GitHub Pages, Netlify, Vercel static hosting, Cloudflare Pages, or any standard web server.
