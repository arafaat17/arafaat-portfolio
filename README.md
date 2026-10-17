# Arafaat Shaikh — portfolio

A responsive, buildless portfolio for systems engineering, applied AI, and automation.

## Preview

Run `python3 -m http.server 8000` and open `http://localhost:8000`.

## Content and interactions

- `index.html` contains the page, responsive styles, and browser-local interactions.
- The pipeline explorer is explicitly labelled as a simulation. It does not call a model or measure backend performance; the original live NodeFlow sandbox is linked separately.
- The portfolio guide uses curated answers and sends no chat data. The existing `api/chat.js` endpoint is retained but is not called by this template.
- Public projects link to source. Internal work is anonymised; no unverified performance metrics or testimonials are included.
- LinkedIn links appear in navigation, the introduction, and the contact section.

## Publish

This repository is connected to Vercel. Merging into `main` should trigger a production deployment. The canonical portfolio URL is https://arafaatshaikh.mywire.org/.

The previous `styles.css` is retained for reference; the new template uses inline styles.
