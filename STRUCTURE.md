# 📦 Projektstruktur – GitHub Pages Website

Hier ist eine vollständige Übersicht aller Dateien und deren Funktion.

```
github-pages/
│
├── index.html              ← 🏠 Startseite (Einstiegspunkt)
├── about.html              ← ℹ️  Über uns / Unternehmensprofil
├── services.html           ← 💼 Leistungen / Services
├── contact.html            ← 📧 Kontakt / Kontaktformular
│
├── css/
│   └── style.css           ← 🎨 Alle Styles (Farben, Layout, Responsive)
│
├── assets/
│   ├── logo-simple-400x100.png      ← 🔵 Logo (Standard, für Header)
│   ├── logo-simple-300x80.png       ← 🔵 Logo (Tablet-Größe)
│   ├── logo-simple-240x60.png       ← 🔵 Logo (Mobile-Größe)
│   ├── favicon.ico                  ← 🔗 Browser-Tab Icon
│   └── favicon.svg                  ← 🔗 Modernes favicon Format
│
├── README.md               ← 📝 Dokumentation (allgemein)
├── DEPLOYMENT.md           ← 🚀 Schritt-für-Schritt Deployment-Guide
├── .gitignore              ← 🚫 Git-Konfiguration
└── _config.yml             ← ⚙️  GitHub Pages / Jekyll Konfiguration
```

---

## **Dateiübersicht**

### **HTML-Dateien (Seiten)**

| Datei | Funktion | Inhalt |
|-------|----------|---------|
| `index.html` | Startseite | Hero-Section, Highlights, Call-to-Action |
| `about.html` | Über uns | Kurzprofil, Kompetenzen, Arbeitsweise |
| `services.html` | Leistungen | 4 Service-Cards (Beratung, Entwicklung, Schulung, Support) |
| `contact.html` | Kontakt | Kontaktinformationen, Kontaktformular |

**Verlinkt durch:** Navigation im Header auf jeder Seite

---

### **CSS-Styling**

| Datei | Funktion |
|-------|----------|
| `css/style.css` | Master-Stylesheet: Farben, Typografie, Layout, Responsive Design |

**Farben:**
- Blau (Primary): `#0b5fff` (vom Logo)
- Dunkelblau (Gradient): `#003f9a`
- Weiß & Grautöne: Navigation, Cards, Footer

**Responsive Breakpoints:**
- Desktop: 1200px+
- Tablet: 768px–1199px
- Mobile: < 768px
- Extra Small: < 480px

---

### **Assets (Bilder & Icons)**

| Datei | Größe | Verwendung |
|-------|-------|-----------|
| `logo-simple-400x100.png` | 400×100px | Desktop Header, Print |
| `logo-simple-300x80.png` | 300×80px | Tablet |
| `logo-simple-240x60.png` | 240×60px | Mobile |
| `favicon.ico` | 32×32px | Browser-Tab Icon |
| `favicon.svg` | Vektor | Alternative (moderne Browser) |

**Hinweis:** Das Logo ist in **blau** (#0b5fff) mit **weißem K** Symbol. Alle Formate sind für Ihre Website optimiert.

---

### **Konfigurationsdateien**

| Datei | Funktion |
|-------|----------|
| `_config.yml` | Jekyll-Konfiguration für GitHub Pages (Theme, Plugins, Metadaten) |
| `.gitignore` | Git-Konfiguration (welche Dateien ignoriert werden) |
| `README.md` | Dokumentation für GitHub Repository (Projektübersicht) |
| `DEPLOYMENT.md` | Detaillierte Deployment-Anleitung (Schritt-für-Schritt) |

---

## **Workflow beim Bearbeiten**

### **Szenario 1: Text ändern**
1. Öffnen Sie die entsprechende HTML-Datei (z. B. `services.html`)
2. Bearbeiten Sie den Text
3. Speichern Sie die Datei
4. Lokal: Aktualisieren Sie den Browser (F5)
5. GitHub: Committen Sie die Änderung

### **Szenario 2: Design ändern**
1. Bearbeiten Sie `css/style.css`
2. Ändern Sie Farben, Abstände, Schriftarten, etc.
3. Der Browser zeigt die Änderungen in Echtzeit (mit Live-Server)
4. Nach GitHub: Änderungen sind automatisch live

### **Szenario 3: Logo/Bilder ändern**
1. Ersetzen Sie die Datei in `assets/`
2. **Wichtig:** Verwenden Sie den gleichen Dateinamen!
3. Aktualisieren Sie den Browser-Cache (Strg+Shift+Löschen)

---

## **Anpassungen am häufigsten gemacht**

### **Farbe des Themes ändern** (z. B. von Blau zu Grün)
1. Öffnen Sie `css/style.css`
2. Suchen Sie: `#0b5fff` (blau)
3. Ersetzen Sie alle Vorkommen mit Ihrer Farbe (z. B. `#28a745` für grün)
4. Speichern

**Alle Vorkommen:**
```css
.btn-primary       /* Buttons */
.nav-links a:hover /* Link-Hover */
.hero              /* Hero-Gradient */
.card h3           /* Card-Titel */
/* etc. */
```

### **Schriftart ändern**
1. Öffnen Sie `css/style.css` (Zeile ~17)
2. Ändern Sie die `font-family`:
```css
font-family: 'Segoe UI', Roboto, 'Courier New', monospace;
```

### **Breite des Layouts ändern**
1. Öffnen Sie `css/style.css`
2. Suchen Sie: `.container { max-width: 1200px; }`
3. Ändern Sie zu z. B. `1400px` oder `1000px`

---

## **Testing vor Deployment**

### **Lokal testen:**
1. Öffnen Sie `index.html` im Browser (Doppelklick)
2. Navigieren Sie durch alle Seiten
3. Prüfen Sie auf Desktops, Tablets und Mobiles
4. Testen Sie Links und Buttons

### **Mobile testen:**
- Im Browser: F12 → Responsive Design Mode (Strg+Shift+M)
- Geräte-Presets: iPhone, iPad, etc.

### **Barrierefreiheit:**
- Tab-Navigation prüfen
- Kontrast testen (WCAG AA Standard)
- Screenreader testen (optional)

---

## **Häufige Probleme**

| Problem | Lösung |
|---------|--------|
| Logo wird nicht angezeigt | Prüfen Sie: Logo in `assets/` vorhanden? Pfad korrekt? |
| Seite sieht anders aus als lokal | Browser-Cache: Strg+Shift+Löschen drücken |
| Änderungen nicht sichtbar | Warten Sie 30 Sekunden, dann aktualisieren Sie |
| Styling verschwindet | Prüfen Sie: `css/style.css` Link in HTML korrekt? |
| Mobile-View sieht verkehrt aus | Prüfen Sie: `meta viewport` Tag in HTML vorhanden? |

---

## **Nächste Schritte**

1. ✅ **Website live gehen** → Siehe `DEPLOYMENT.md`
2. 📧 **Kontaktformular aktivieren** → Siehe `contact.html` Kommentare
3. 🎨 **Design personalisieren** → Farben, Schriften anpassen
4. 📱 **Mobile optimieren** → Screenshots auf verschiedenen Geräten
5. 📊 **Analytics hinzufügen** → Google Analytics (optional)

---

**Fragen? README.md oder DEPLOYMENT.md lesen!**

© 2026 KLOPF IT-Solutions GmbH
