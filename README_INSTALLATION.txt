MplusKASSA PWA – INSTALLATION AUF SAMSUNG / CHROME

ZIEL-WEB-APP
https://script.google.com/macros/s/AKfycbyGVPiNk2--IrkN33Mi7etv9LZ8iFQk-kykct0eG8-zJuh9Icr4R3n7hlHFQgcA17TMyQ/exec

WAS DIESES PAKET MACHT
- eigenes MplusKASSA-Verwaltungsicon
- App-Name "MplusKASSA Verwaltung"
- echtes manifest.webmanifest
- Service Worker
- Android maskable icon
- Standalone-PWA-Start
- automatische Weiterleitung zur bestehenden Google-Apps-Script-Web-App

WICHTIG
Die Dateien müssen auf einer HTTPS-Webadresse liegen.
Die script.google.com-/exec-Adresse selbst kann diese PWA-Dateien nicht zuverlässig als
eigenständige Manifest-/Service-Worker-Ressourcen hosten.

DATEIEN HOCHLADEN
Den kompletten Inhalt dieses Ordners auf einen statischen HTTPS-Webspace hochladen.
index.html muss im Hauptverzeichnis liegen.

Danach bekommst du z. B. eine Adresse wie:
https://deine-domain.de/mpluskassa/
oder
https://<name>.github.io/mpluskassa/

SAMSUNG / GOOGLE CHROME
1. DIE PWA-ADRESSE öffnen – NICHT die script.google.com-/exec-Adresse.
2. Chrome-Menü ⋮ öffnen.
3. "App installieren" wählen.
   Falls nur "Zum Startbildschirm hinzufügen" erscheint, diese Option wählen.
4. Name "MplusKASSA Verwaltung" bestätigen.
5. Jetzt erscheint dein eigenes MplusKASSA-Icon auf dem Homescreen.
6. Icon antippen.
7. Der MplusKASSA-Launcher startet und öffnet automatisch die Verwaltung.

WENN DAS ALTE/FALSCHE ICON WEITERHIN KOMMT
- vorhandene Homescreen-Verknüpfung löschen
- Chrome komplett schließen
- neue PWA-Adresse wieder öffnen
- App neu installieren

HINWEIS
Da die eigentliche Apps-Script-App auf script.google.com liegt, verlässt die PWA beim
Weiterleiten ihren eigenen Origin. Das eigene Homescreen-Icon und der App-Name bleiben
für den installierten Launcher erhalten. Je nach Android-/Chrome-Version kann beim
Öffnen der externen Apps-Script-Seite Browser-/Origin-Chrome eingeblendet werden.

Für ein vollständig nahtloses PWA-Fenster müsste die eigentliche Anwendung später
unter derselben eigenen HTTPS-Domain ausgeliefert bzw. als kompatibler Wrapper
eingebettet werden.
