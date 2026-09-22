# Hussaini Automations — Event Lead Form

A single static page (`index.html`) that collects event leads and sends
them to a Google Sheet via an Apps Script web app.

## Deploy on Vercel via GitHub

1. Create a new GitHub repo and push this folder's contents to it
   (or use GitHub's "upload files" web UI — drag `index.html` and
   `README.md` in, commit).
2. Go to vercel.com, click **New Project**, and import that GitHub repo.
3. Leave all settings as default (no build step needed — it's static
   HTML) and click **Deploy**.
4. Vercel gives you a live URL (e.g. `your-project.vercel.app`) —
   that's the link to share at the event.

## Before you deploy

- The Google Apps Script endpoint is already wired into `index.html`
  (the `ENDPOINT_URL` constant near the bottom of the file).
- Test locally first: open `index.html` directly in a browser, submit
  a test entry, and confirm a new row appears in your "Event Leads"
  Google Sheet.

## Updating later

If you ever need to change the form (add a field, tweak the endpoint,
etc.), edit `index.html` and push the change to GitHub — Vercel
redeploys automatically on every push.
