# LECIFY – statische Landingpage

Live unter https://lecify.mattea.pro (via GitHub Pages).

Diese Repo enthält **ausschließlich die öffentliche Marketing-Landingpage**. Die eigentliche
SaaS-App (Multi-Tenant-Zeiterfassung, Auth, Datenbank, Server-Actions) lebt in einem anderen
Repo und wird separat deployed.

## Dateien im Root

| Datei | Zweck |
|---|---|
| `index.html` | Startseite |
| `impressum.html` | Impressum (Platzhalter) |
| `datenschutz.html` | Datenschutzerklärung (Platzhalter) |
| `agb.html` | AGB (Platzhalter) |
| `404.html` | Fehlerseite |
| `CNAME` | **nicht löschen** — enthält `lecify.mattea.pro`, damit die Custom Domain funktioniert |

## Technik

- Statisches HTML + Tailwind via Play-CDN. Kein Build-Schritt, kein `node_modules`.
- Dark/Light-Mode: Theme-Toggle oben rechts, Präferenz wird in `localStorage` gespeichert
  (fällt sonst zurück auf `prefers-color-scheme`).

## Links zur App

Die „Konto erstellen" / „Anmelden"-Buttons zeigen aktuell auf `https://lecify.vercel.app` als
Platzhalter. Beim Beta-Launch wird die echte App-URL per Suchen/Ersetzen eingetragen.

## So lädst du eine neue Version hoch (manuell, via GitHub-Web-UI)

1. Oben auf **Add file → Upload files** tippen.
2. Deine Website-Dateien hineinziehen. Die Startseite muss **index.html** heißen.
3. Unten auf **Commit changes** tippen.
4. Nach 1–2 Minuten ist die neue Version unter https://lecify.mattea.pro zu sehen.

**Wichtig:** `CNAME` nicht löschen — sonst geht die Custom Domain verloren.
