Food Controll – Hosting-Paket
Diese Dateien reichen aus, um die App als eigenständige Web-App mit eigenem
FC-App-Icon auf dem Handy-Startbildschirm zu betreiben.
Enthaltene Dateien
`index.html` – die komplette App (lädt React direkt im Browser, kein Build nötig)
`manifest.webmanifest` – Name, Farben und Icon-Verweise für "Zum Home-Bildschirm hinzufügen"
`icon-192.png`, `icon-512.png`, `icon-512-maskable.png` – Android/Chrome-Icons
`apple-touch-icon.png` – iOS-Icon
Hosting in 3 Schritten (Beispiel: Netlify)
Gehe auf netlify.com → kostenloses Konto erstellen (falls noch nicht vorhanden).
Auf der Startseite den Bereich "Deploy manually" nutzen: Ziehe genau
diese 6 Dateien (nicht in einen Unterordner gepackt, sondern direkt auf
oberster Ebene) per Drag & Drop in das Upload-Feld.
Netlify vergibt automatisch eine Adresse wie
`https://dein-projekt.netlify.app`. Fertig – die App ist live.
(Bei Vercel funktioniert es genauso: neues Projekt anlegen, die Dateien
hochladen, fertig. Ein Build-Schritt ist nicht nötig.)
FC-Icon auf dem Home-Bildschirm
Öffne die neue Adresse auf deinem Handy im Browser (Safari bei iPhone,
Chrome bei Android).
Tippe auf "Zum Home-Bildschirm hinzufügen" (Safari: Teilen-Symbol →
"Zum Home-Bildschirm") bzw. "App installieren" (Chrome).
Auf dem Home-Bildschirm erscheint jetzt der dunkelblaue FC-Button –
ein Klick öffnet die App im Vollbild, ganz ohne Browser-Leiste.
Hinweis zur Datenspeicherung
Die App speichert Produkte und Einkaufsliste jetzt im `localStorage` des
Browsers (statt im Claude-Artefakt-Speicher). Die Daten bleiben also auf dem
jeweiligen Gerät/Browser erhalten, werden aber nicht automatisch mit
anderen Geräten synchronisiert.
