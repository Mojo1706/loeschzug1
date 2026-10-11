# Personalverwaltung · Löschzug 1 · Feuerwehr Kempten

Funktionsfähige lokale Erstversion für Personal, Anwesenheit bei Übungen und Alarmen sowie Ausbildungsstand. Kein offizielles Produkt der Feuerwehr Kempten.

## Starten
`index.html` im Browser öffnen oder über GitHub Pages bereitstellen. Keine Installation oder Build-Schritte nötig.

## GitHub Pages
1. Auf GitHub ein neues Repository `loeschzug1` erstellen.
2. Diese ZIP entpacken. `index.html`, `style.css`, `app.js`, `.nojekyll` und `README.md` in das Hauptverzeichnis des Repositorys hochladen und committen.
3. Unter **Settings → Pages → Build and deployment** die Quelle **Deploy from a branch** auswählen.
4. Branch **main**, Ordner **/(root)** auswählen und speichern.
5. Nach der Bereitstellung steht dort die Website-Adresse.

Offizielle Anleitung: https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site

## Funktionen
- Personal anlegen und bearbeiten, Gruppe und Funktion hinterlegen, Aktivstatus setzen.
- Übung oder Alarm anlegen; Übungen optional als 6 oder 13 Termine im Abstand von genau 14 Tagen.
- Anwesenheit pro Person und Termin: offen, anwesend, entschuldigt, abwesend.
- Die Personenliste eines Termins bleibt erhalten, auch wenn Personen später inaktiv werden. Neues aktives Personal lässt sich ausdrücklich ergänzen.
- Ausbildung mit individuellem Lehrgang, geplant / in Ausbildung / abgeschlossen, Abschlussdatum und optionaler Gültigkeit.
- Vollständiger JSON-Export und validierter Import; Druckansicht der Anwesenheit.

## Grenzen dieser Erstversion
Speicherung ausschließlich in localStorage des jeweiligen Browsers. Keine Anmeldung, keine Rollen, keine zentrale Datenbank und kein automatischer Abgleich. Browserdaten können gelöscht werden; regelmäßig exportieren. GitHub Pages liefert statische Dateien und ist keine Personaldatenbank. Zunächst nur Testdaten verwenden. Personen-, Anwesenheits- und Einsatzdaten oder Sicherungen niemals ins Repository laden.

Für eine betriebliche gemeinsame Version: GitHub Pages als Oberfläche beibehalten und eine zugriffsgeschützte API mit Datenbank anschließen. Benutzerkonten für Zugführung und Führungskräfte, serverseitige Rechteprüfung, Sicherungen und ein Änderungsprotokoll ergänzen. Zugriffssicherung muss im Backend erfolgen; ein Passwortfeld im Browser genügt nicht.

Keine echten Personal- oder Einsatzdaten sind enthalten. Es wurden keine Feuerwehrqualifikationen oder Diensttermine erfunden. Ersttermin und Lehrgangsbezeichnungen werden von euch festgelegt.
