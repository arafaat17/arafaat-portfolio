# Arafaat Shaikh — portfolio

A responsive, buildless portfolio for systems engineering, applied AI, and automation.

## Preview

Run `python3 -m http.server 8000` and open `http://localhost:8000`.

## Content and interactions

- `index.html` contains the page, responsive styles, and browser-local interactions.
- The pipeline explorer embeds the original live NodeFlow Cloud Run sandbox, with a full-screen link. Inputs are sent to that service.
- The portfolio guide calls the existing `/api/chat` Gemini endpoint. Suggested questions use the same live path. Failed requests, invalid responses, and requests exceeding 20 seconds show an explicitly labelled curated answer.
- The existing Gemini backend and model configuration are unchanged. Vercel must retain its `GEMINI_API_KEY` environment variable. A static local server cannot execute `/api/chat`, so local previews show the fallback.
- Public projects link to source. Internal work is anonymised; no unverified performance metrics or testimonials are included.
- LinkedIn links appear in navigation, the introduction, and the contact section.

## Publish

This repository is connected to Vercel. Merging into `main` should trigger a production deployment. The canonical portfolio URL is https://arafaatshaikh.mywire.org/.

The previous `styles.css` is retained for reference; the new template uses inline styles.
