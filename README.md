# Dub Automotive CRM — clickable demo (Azmin Digital)

Static website, no server code. Upload the whole folder as-is.

Pages: `index.html` (dashboard), `leads.html`, `lead.html`, `studio.html`, `mobile.html`.
Pages carry `noindex`, so search engines won't list the demo.

Target address: **https://dub.azmindigital.com** (change the `CNAME` file if you pick another subdomain).

## Option A — Netlify (easiest, free, HTTPS automatic)
1. Go to https://app.netlify.com/drop and drag this folder onto the page.
2. Site configuration → Domain management → Add a domain → `dub.azmindigital.com`.
3. At your domain's DNS provider, add a record:
   - Type `CNAME`, Name `dub`, Value `<your-site-name>.netlify.app`
4. Wait for DNS (usually minutes) — Netlify issues the SSL certificate itself.

## Option B — GitHub Pages
1. Create a repository (e.g. `dub-crm-demo`) and upload all files in this folder, including `CNAME`.
2. Settings → Pages → Source: "Deploy from a branch" → `main` / root → Save.
3. DNS: `CNAME`, Name `dub`, Value `<your-github-username>.github.io`
4. Back in Settings → Pages, tick "Enforce HTTPS" once the certificate is ready.

## Option C — your existing web hosting (cPanel)
1. cPanel → Domains → create subdomain `dub.azmindigital.com`.
2. File Manager → open the subdomain's folder → upload all files.
