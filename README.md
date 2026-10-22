# Aura Box · Coming soon

Eén bestand: `index.html` (HTML, CSS, JS en logo inline). Lettertypes via Google Fonts.

## Instellen
Bovenaan het script in `index.html` staat `CONFIG`:
- `launchDate`: bijv. `"2026-12-01"` voor een aftelling. `null` = "Ouverture bientôt".
- `endpoint`: URL die e-mails ontvangt via POST (JSON `{email, lang}`), bijv. Formspree. Leeg = alleen demo (opslag in de browser van de bezoeker).

## Online zetten op Cloudflare Pages
1. Zet deze map in een GitHub-repository (bijv. `aura-coming-soon`).
2. Cloudflare dashboard > Workers & Pages > Create > Pages > Connect to Git.
3. Kies de repository. Framework preset: None. Build command: leeg. Output directory: `/` (root).
4. Deploy. Daarna eventueel eigen domein onder Custom domains.

Elke push naar `main` zet de pagina automatisch opnieuw online.
