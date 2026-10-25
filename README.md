# Million Crowns Music

Website for Million Crowns Music, the label of the future.

- `index.html` is the homepage.
- `founders.html` is the Founders page.
- `assets/` holds the logo files.

The site is static HTML with no build step. Netlify publishes this repository as is, so any change pushed to `main` goes live automatically.

Social icons in `assets/icons/` are from Simple Icons (simpleicons.org), released under CC0.

## Chat assistant

The "Ask Million Crowns" chat calls `netlify/functions/chat.mjs` at `/api/chat`, which sends questions to Claude. It needs an `ANTHROPIC_API_KEY` environment variable in Netlify. The assistant's knowledge of the label (roster, releases, services, contacts) lives in the `KNOWLEDGE` text in that file, so update it whenever the site changes.
