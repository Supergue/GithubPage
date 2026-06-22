# KLOPF IT-Solutions GmbH – Website

Statische Website für KLOPF IT-Solutions GmbH, gehostet auf GitHub Pages.

## 📋 Projektstruktur

```
.
├── index.html              # Startseite
├── about.html              # Über uns
├── services.html           # Leistungen
├── contact.html            # Kontakt
├── css/
│   └── style.css           # Haupt-Stylesheet (responsive Design)
├── assets/
│   ├── favicon.ico         # Website-Icon
│   ├── logo-simple-400x100.png
│   ├── logo-simple-300x80.png
│   └── logo-simple-240x60.png
├── README.md               # Diese Datei
└── .gitignore              # Git-Ausschlüsse
```

## 🚀 Deployment auf GitHub Pages

### Schritt 1: Repository erstellen
1. Gehen Sie zu [GitHub.com](https://github.com) und melden sich an
2. Klicken Sie auf das **+**-Symbol → **New repository**
3. Geben Sie als Repository-Name ein: `klopf-it-solutions` (oder ähnlich)
4. Setzen Sie auf **Public** (erforderlich für GitHub Pages)
5. Klicken Sie **Create repository**

### Schritt 2: Dateien hochladen
1. Klicken Sie auf **Add file** → **Upload files**
2. Laden Sie folgende Dateien/Ordner hoch:
   - `index.html`
   - `about.html`
   - `services.html`
   - `contact.html`
   - Den Ordner `css/` mit `style.css`
   - Den Ordner `assets/` mit Logos und Favicon
3. Klicken Sie **Commit changes**

Alternativ mit Git CLI:
```bash
git clone https://github.com/YOUR_USERNAME/klopf-it-solutions.git
cd klopf-it-solutions
# Kopieren Sie alle Dateien in diesen Ordner
git add .
git commit -m "Initial website setup"
git push origin main
```

### Schritt 3: GitHub Pages aktivieren
1. Gehen Sie zu Repository-Einstellungen: **Settings** → **Pages**
2. Unter "Build and deployment":
   - **Source**: Wählen Sie `Deploy from a branch`
   - **Branch**: Wählen Sie `main` und `/root`
3. Klicken Sie **Save**

GitHub Pages wird automatisch bereitgestellt. Die Website ist dann erreichbar unter:
```
https://YOUR_USERNAME.github.io/klopf-it-solutions
```

## 🎨 Anpassungen

### Kontaktinformationen aktualisieren
Öffnen Sie `contact.html` und ersetzen Sie:
- `kontakt@klopf-it.de` → Ihre E-Mail-Adresse
- `+49 (0) XXX XXXXXXX` → Ihre Telefonnummer
- Adresse und Ort

### Logo aktualisieren
Ersetzen Sie die PNG-Dateien im `assets/`-Ordner mit Ihrem Logo (behalten Sie die Dateinamen bei).

### Inhalt bearbeiten
Alle Inhalte befinden sich in den HTML-Dateien (`index.html`, `about.html`, etc.). Sie können diese direkt in GitHub bearbeiten:
1. Klicken Sie auf die Datei
2. Klicken Sie auf das Bleistift-Icon (✎ Edit)
3. Nehmen Sie Ihre Änderungen vor
4. Klicken Sie **Commit changes**

### Kontaktformular aktivieren
Das Kontaktformular in `contact.html` ist momentan ein Platzhalter. Um es funktional zu machen:

**Option A: Mit Formspree** (empfohlen)
1. Gehen Sie zu [formspree.io](https://formspree.io)
2. Registrieren Sie sich
3. Erstellen Sie ein neues Formular für Ihre E-Mail
4. Kopieren Sie den Action-Link
5. Bearbeiten Sie `contact.html`, zeile ~73:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

**Option B: Mit E-Mail-Link**
Ersetzen Sie das Formular mit:
```html
<a href="mailto:kontakt@klopf-it.de?subject=Kontaktanfrage">
  <button class="btn btn-primary">E-Mail schreiben</button>
</a>
```

## 📱 Funktionen

- ✅ Vollständig responsive Design (Desktop, Tablet, Mobile)
- ✅ Schnelle Ladezeiten (statische HTML/CSS)
- ✅ SEO-optimiert
- ✅ Modernes, professionelles Design
- ✅ Sticky Navigation
- ✅ Smooth Scrolling
- ✅ Accessible (barrierearm)

## 🔧 Technische Details

- **HTML5** semantisches Markup
- **CSS3** mit Grid und Flexbox für responsive Layout
- **Keine Abhängigkeiten** (kein Node, kein Build-Tool notwendig)
- **Farbe**: Blau (#0b5fff) – angepasst an Ihr Logo

## 📞 Support

Bei Fragen zur Website oder Anpassungen kontaktieren Sie mich unter:
- **E-Mail**: kontakt@klopf-it.de
- **Telefon**: [Ihre Nummer eintragen]

---

**© 2026 KLOPF IT-Solutions GmbH. Alle Rechte vorbehalten.**
