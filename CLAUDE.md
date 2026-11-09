# i.thie softworks – Label-Homepage

Statische Homepage des Labels „i.thie softworks“ (Michael Draws-Beer). Zweck vor allem: zentrales **Impressum + Datenschutz**, auf das YouTube (`@MichaelDraws-k6n`) und das geplante Instagram-Konto verlinken; dazu Übersicht der Spiele und Kanäle.

## Regeln des Nutzers

- **Nie selbst committen oder pushen** – auch nicht lokal. Der Nutzer committet selbst.
- **READMEs knapp**, keine TODO-Listen. Offene Punkte nur im Chat nennen.
- **Alles inline im HTML** (CSS, JS, Schrift als base64). Separate Dateien nur für Bilder.
- Erst fragen, bevor Dinge außerhalb des Auftrags angefasst werden.

## Aufbau

- `index.html` – Startseite (englisch): Logo, Spiele, Kanäle, Footer-Link „Impressum · Datenschutz“.
- `impressum.html` – deutsch: Impressum (§ 5 DDG, § 18 MStV, USt-IdNr., Kleinunternehmer) + Datenschutz der Webseite (keine Cookies, Server-Logs, GitHub Pages/USA mit DPF-Angemessenheitsbeschluss, YouTube nur als Link).
- `assets/` – Logo „Ringplanet“ (Pixel-Art, orange/türkis): `logo.svg`, `logo-white.svg`, `logo-black.svg`, `profile-800.png` (Profilbild), `wordmark-dark/light.png`, `favicon.png` (96), `apple-touch-icon.png`; Cover der Spielschachteln `cover-wolf.jpg` / `cover-pts.jpg` (aus den App-Icons, 420 px); Rückseiten-Screenshots `shot-wolf-1..3.jpg` (aus dem App-Store-Eintrag) und `shot-pts-1..3.jpg` (aus `sol-promo/screenshots/small`).
- `.github/workflows/deploy.yml` – GitHub Pages per Actions, kopiert `index.html impressum.html assets`.
- Stil wie die PTS-Promo-Seite: Schrift „Press Start 2P“, Hintergrund `#020205`, Akzente `#ffa02e` / `#3fd3c6`, Fokus-Rahmen, `prefers-reduced-motion`.

## Spiele

- **Populate the Stars** – `https://www.populate-the-stars.com/` (Promo-Seite: `~/Desktop/sol-promo`, Repo `ithie/populate-the-stars`, Spiel: `~/Desktop/sol`). Im App-Store-Review → auf der Startseite unter „COMING SOON“.
- **SAR: Callsign WOLF** – `https://callsign-wolf.de/` (Code: `~/Desktop/callsign-wolf`). Isometrischer Hubschrauber-Rettungssimulator, im App Store → „OUT NOW“.
- Startseite verlinkt nur auf die Spiel-Seiten, nicht direkt in den App Store.

## Stand (2026-11-09)

- GitHub-Repo: `https://github.com/ithie/ithie-softworks` (Branch `main`, Deploy per Actions). Lokaler Ordner war noch nicht damit verbunden; nichts deployed, keine Label-Domain.
- `www.populate-the-stars.com`: DNS korrekt (Strato), HTTPS-Zertifikat bei GitHub war noch ausstehend.
- Instagram-Konto fürs Label geplant; Satz dazu steht schon im Impressum.
- Impressum hat nur E-Mail als Kontakt; Telefonnummer als zweiter Kanal war offen.
