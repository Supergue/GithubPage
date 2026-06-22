# 🚀 GitHub Pages Deployment Anleitung

Diese Anleitung beschreibt Schritt für Schritt, wie Sie die Website auf GitHub Pages hochladen und online stellen.

---

## **Schritt 1: GitHub Konto**

Falls Sie noch kein GitHub Konto haben:
1. Gehen Sie zu [github.com](https://github.com)
2. Klicken Sie **Sign up**
3. Folgen Sie der Registrierung (E-Mail, Passwort, etc.)
4. Bestätigen Sie Ihre E-Mail-Adresse

---

## **Schritt 2: Neues Repository erstellen**

1. Melden Sie sich bei GitHub an
2. Klicken Sie auf das **+**-Symbol (oben rechts)
3. Wählen Sie **New repository**
4. Tragen Sie ein:
   - **Repository name**: `klopf-it-solutions` (oder: `websites` oder `portfolio`)
   - **Description**: `Professionelle Website für KLOPF IT-Solutions GmbH` (optional)
5. Wählen Sie **Public** (muss public sein für GitHub Pages)
6. ❌ NICHT ankreuzen: "Initialize this repository with a README" (ich habe schon einen)
7. Klicken Sie **Create repository**

---

## **Schritt 3: Dateien hochladen (Methode A – Einfach, via Browser)**

1. Sie sind jetzt im neuen, leeren Repository
2. Klicken Sie **Add file** → **Upload files**
3. Sie sehen jetzt einen Upload-Bereich
4. Ziehen Sie alle Dateien und Ordner aus dem `github-pages` Verzeichnis hierher:
   - `index.html`
   - `about.html`
   - `services.html`
   - `contact.html`
   - Ordner `css` (mit `style.css`)
   - Ordner `assets` (mit Logos und Favicon)
   - `.gitignore`
   - `_config.yml`
   - `README.md`

5. **Optional**: Kommentar eingeben: `Initial website setup`
6. Wählen Sie **Commit directly to the main branch**
7. Klicken Sie **Commit changes**

⏳ Die Dateien werden hochgeladen. Das dauert wenige Sekunden.

---

## **Schritt 3 Alternative: Dateien hochladen (Methode B – Mit Git CLI)**

Falls Sie Git auf Ihrem Computer installiert haben:

```bash
# 1. Repository klonen
git clone https://github.com/YOUR_USERNAME/klopf-it-solutions.git
cd klopf-it-solutions

# 2. Alle Dateien aus github-pages kopieren:
#    (Kopieren Sie manuell alle Dateien von github-pages in diesen Ordner)

# 3. Änderungen commiten und hochladen
git add .
git commit -m "Initial website setup"
git push origin main
```

Ersetzen Sie `YOUR_USERNAME` durch Ihren GitHub-Benutzernamen.

---

## **Schritt 4: GitHub Pages aktivieren**

1. Gehen Sie zu Ihrem Repository
2. Klicken Sie auf **Settings** (Reiter oben)
3. Scrollen Sie in der Sidebar nach unten bis **Pages**
4. Unter "Build and deployment":
   - **Source**: Wählen Sie `Deploy from a branch`
   - **Branch**: Wählen Sie `main` aus dem Dropdown
   - **Folder**: `/root` (nicht verwechseln mit `/root`)
5. Klicken Sie **Save**

⏳ GitHub Pages wird jetzt bereitgestellt (dauert 1–2 Minuten).

---

## **Schritt 5: Website testen**

Nachdem GitHub Pages bereitgestellt wurde, erhalten Sie:

```
https://YOUR_USERNAME.github.io/klopf-it-solutions
```

Diese URL finden Sie auch unter:
- **Settings** → **Pages** → Sie sehen hier die Live-URL

Geben Sie diese URL in Ihren Browser ein. 🎉 Ihre Website ist jetzt live!

---

## **Danach: Inhalt bearbeiten**

Sie können Inhalte direkt auf GitHub bearbeiten, ohne Terminal zu nutzen:

### **Text/Inhalt ändern:**
1. Gehen Sie zum Repository
2. Klicken Sie auf die Datei, die Sie ändern möchten (z. B. `index.html`)
3. Klicken Sie auf das **Stift-Icon** (✎ Edit this file)
4. Nehmen Sie Ihre Änderungen vor
5. Scrollen Sie nach unten und klicken Sie **Commit changes**

✅ Die Änderungen sind sofort live (kann 10–30 Sekunden dauern).

### **Kontaktinformationen aktualisieren:**
1. Öffnen Sie `contact.html` zum Bearbeiten
2. Suchen Sie diese Zeilen und ersetzen Sie mit Ihren Daten:
   ```html
   kontakt@klopf-it.de        → Ihre E-Mail
   +49 (0) XXX XXXXXXX        → Ihre Telefonnummer
   [Straße und Hausnummer]    → Ihre Adresse
   [PLZ und Ort]              → Ihre Stadt
   ```
3. **Commit changes**

### **Logo austauschen:**
1. Klicken Sie auf **assets** im Repository
2. Klicken Sie auf eine Logo-Datei (z. B. `logo-simple-400x100.png`)
3. Klicken Sie auf das **Mülleimer-Icon**, um die alte Datei zu löschen
4. Gehen Sie zurück zu assets und klicken Sie **Add file** → **Upload files**
5. Laden Sie Ihr neues Logo hoch (gleicher Name wie die alte Datei!)
6. **Commit changes**

---

## **Häufig gestellte Fragen**

### **Wie lange dauert es, bis die Website live ist?**
- Beim ersten Mal: 1–2 Minuten
- Nach Änderungen: 10–30 Sekunden

### **Kann ich die Domain ändern?**
Ja, Sie können eine Custom Domain einrichten (z. B. `www.klopf-it.de`). Das ist unter **Settings** → **Pages** → **Custom domain** möglich. Dafür brauchen Sie Zugriff auf Ihren Domain-Provider.

### **Wie kann ich die Website offline anschauen?**
Öffnen Sie einfach die `index.html` Datei in Ihrem Browser (Rechtsklick → Open with → Browser).

### **Das Kontaktformular funktioniert nicht?**
Das Formular ist momentan statisch. Für volle Funktionalität brauchen Sie einen externen Service:
- **Formspree** (empfohlen): formspree.io
- **Netlify Forms**: netlify.com
- **Oder E-Mail-Link**: `mailto:kontakt@klopf-it.de`

Siehe README.md für Anweisungen.

### **Wer kann die Website sehen?**
Jeder mit der URL. Es gibt keine Zugriffsbeschränkung.

### **Können mehrere Personen bearbeiten?**
Ja! Sie können unter **Settings** → **Collaborators** andere GitHub-Benutzer hinzufügen.

---

## **Nächste Schritte (Optional)**

- 📧 Kontaktformular mit Formspree aktivieren
- 🌐 Custom Domain einrichten
- 📱 Mobile Optimierung prüfen (Sie können die Website auch mobil testen)
- 🎨 Farben und Schriftarten nach Bedarf anpassen (in `css/style.css`)
- 📊 Google Analytics hinzufügen (für Besucherstatistiken)

---

**Fragen? Kontaktieren Sie mich: kontakt@klopf-it.de**

© 2026 KLOPF IT-Solutions GmbH
