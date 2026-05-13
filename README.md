# 8 Moments Landingpage

Eigenständiges Git-Projekt für die statische 8 Moments Landingpage.

Das Projekt ist für Netlify vorbereitet und kann dort ohne Build-Schritt veröffentlicht werden.

## Projektinhalt

- `index.html` - Startseite
- `datenschutz.html` - öffentliche Datenschutzerklärung
- `konto-loeschen.html` - öffentliche Anleitung zur Konto- und Datenlöschung
- `impressum.html` - Anbieterkennzeichnung
- `nutzungsbedingungen.html` - Nutzungsbedingungen
- `styles.css` - gemeinsames Styling
- `assets/` - Bilder und Fonts
- `netlify.toml` - Netlify-Konfiguration

## Lokal starten

Im Projektordner:

```bash
npx serve .
```

## Git-Repository

Das Projekt wurde als eigenes Git-Repository initialisiert.

Typischer Ablauf:

```bash
git add .
git commit -m "Initial landingpage setup"
git branch -M main
git remote add origin <dein-repo-url>
git push -u origin main
```

## Netlify

Empfohlene Einstellungen in Netlify:

- Repository: dieses Projekt
- Build command: leer lassen
- Publish directory: `.`

## Domain

Die Seite ist dafür vorbereitet, über Netlify auf deiner Domain zu laufen.

Wenn die Domain `hellolydomain` oder eine echte Subdomain/Domain verwendet wird, hinterlegst du sie in Netlify unter:

- Site configuration
- Domain management
- Add custom domain

## Vor Veröffentlichung prüfen

1. Google-Play-Link in `index.html` prüfen:
   `https://play.google.com/store/apps/details?id=com.andreas.momentum`
2. Datenschutz-URL in der Play Console auf die veröffentlichte Domain setzen, z. B. `/datenschutz`
3. Konto-Löschungs-URL in der Play Console auf die veröffentlichte Domain setzen, z. B. `/konto-loeschen`
4. Support-Mail `sup-moment@outlook.com` prüfen
5. Falls AdMob live geschaltet wird, echte AdMob-App-ID und App-ads.txt-Domain abstimmen
