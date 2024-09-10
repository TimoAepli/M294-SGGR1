# 2024-25 | Modul 294 - SG - GR1
Frontend einer interaktiven Webapplikation realisieren
1. Richtet die lokale Entwicklungs- und Laufzeitumgebung so ein, dass ein vorgegebenes Projekt entwickelt werden kann. [g5.1]
2. Programmiert mittels vorgegebener Technologie und mit Hilfe eines existierenden, dokumentierten Back-Ends ein effizientes, strukturiertes Front-End einer interaktiven Webapplikation, welches die Verwaltung (Create, Read, Update, Delete) von Daten ermöglicht und hält sich dabei an relevante Vorgaben. [g5.3, g2.6, g2.4, g2.2]
3. Programmiert das Front-End einer interaktiven Webapplikation so, dass die einzelnen CRUD-Elemente des Front-Ends über einen permanenten Link erreichbar sind. [g5.3]
4. Überprüft Zwischenergebnisse mit den Anforderungen (funktional, nichtfunktional, Sicherheit) und nimmt laufend Korrekturen vor. [g5.4, g2.6]
5. Hält vorgegebene Coderichtlinien ein und überprüft laufend deren Einhaltung. [g5.5]
6. Legt Änderungen und Erweiterungen der Implementierung übersichtlich und zuverlässig in einem Softwareverwaltungssystem ab. [g5.6]
7. Schützt mindestens einen Bereich des Front-Ends vor anonymen Zugriffen. [g5.3]


## Git - Versionskontrollsystem

Git ist ein verteiltes Versionskontrollsystem, das Entwicklern hilft, den Überblick über Änderungen im Code zu behalten und an gemeinsamen Projekten zu arbeiten.

### Installation
1. Lade Git von der offiziellen Webseite herunter: [Download Git für Windows](https://git-scm.com/download/win)
2. Überprüfe die Installation:
   ```bash
   git --version
   ```
3. Aktualisiere Git (optional):
   ```bash
   git update-git-for-windows
   ```

### Git konfigurieren
Nach der Installation von Git ist es wichtig, die Benutzerdaten zu konfigurieren. Diese Informationen werden in jedem Commit protokolliert.

```bash
git config --global user.name "Dein Name"
git config --global user.email "Deine eMail"
```

### Ein neues Git-Projekt erstellen
1. Erstelle ein neues Verzeichnis:
   ```bash
   mkdir projekt1
   cd projekt1
   ```
2. Initialisiere ein neues Git-Repository:
   ```bash
   git init
   ```

3. Füge eine Datei hinzu und überprüfe den Status des Repositories:
   ```bash
   git status
   git add hallo.txt
   git status
   ```

4. Erstelle den ersten Commit:
   ```bash
   git commit -m "erstes Dokument"
   ```

### Git pull & push - Mit einem Remote-Repository arbeiten
- Aktualisiere dein lokales Repository mit den neuesten Änderungen vom Remote-Repository:
   ```bash
   git pull
   ```

- Lade deine Änderungen zum Remote-Repository hoch:
   ```bash
   git push
   ```

- Klone ein bestehendes Repository von einer URL:
   ```bash
   git clone "url"
   ```

- Verknüpfe dein lokales Repository mit einem Remote-Repository:
   ```bash
   git remote add origin "url"
   ```

- Ändere den Branch-Namen (z. B. auf `main`):
   ```bash
   git branch -M main
   ```

- Push den aktuellen Branch und setze ihn als Standard-Branch:
   ```bash
   git push -u origin main
   ```

### Nützliche Git-Links
- [Git Tutorial - In 40 Minuten Git lernen für Anfänger](https://youtu.be/uGLQF2kUwOA)
- [7 häufigste Git-Probleme und wie Du sie löst (Tutorial für Git-Anfänger)](https://youtu.be/nkDq2qGk_II)

---

## Grundgerüst einer HTML-Datei

Wenn du eine Webseite erstellst, ist die Struktur einer HTML-Datei entscheidend. Hier sind einige grundlegende Punkte, die du beachten solltest:

### Grundlegende Struktur
1. Die Datei `index.html` oder `default.html` ist normalerweise die Startseite deiner Webseite.
2. Stelle sicher, dass die Sprache im `html`-Tag korrekt gesetzt ist, zum Beispiel:
   ```html
   <html lang="de">
   ```
3. Füge einen beschreibenden Titel in den `<title>`-Tag ein:
   ```html
   <title>Meine Webseite</title>
   ```

4. Binde ein Favicon (kleines Icon in der Tab-Leiste des Browsers) ein:
   ```html
   <link rel="icon" href="favicon.ico">
   ```

5. Vervollständige die Metatags für SEO und Responsiveness:
   ```html
   <meta charset="UTF-8">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   <meta name="description" content="Beschreibung deiner Webseite">
   ```

6. Binde dei eigene CSS - Datei ein:
   ```html
   <link rel="stylesheet" href="css/index.css">
   ```

### Verwendung von Google Fonts und Icons
1. Google Fonts ist eine großartige Ressource, um deiner Webseite schöne Schriftarten hinzuzufügen. Beispiel:
   ```html
   <link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">
   ```

2. Material Icons & Symbols können verwendet werden, um deiner Webseite Icons hinzuzufügen:
   ```html
   <link href="https://fonts.googleapis.com/icon?family=Material+Icons" rel="stylesheet">
   ```


