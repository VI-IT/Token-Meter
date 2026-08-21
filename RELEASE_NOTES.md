# Token Meter by VI-IT 1.0.17

## English

Makes changelog translation user-controlled and adds visible automatic-update progress.

- Adds a new updates button immediately to the left of the add-account button
- Reads the official OpenAI ChatGPT and Codex changelog directly from learn.chatgpt.com
- Counts previously unseen official entries from the latest seven calendar days
- Shows the unread count in a red badge; opening the view clears the count for the entries currently shown
- Re-enables the badge automatically when OpenAI publishes another entry
- Opens the changelog in a resizable window centered on the current screen
- Always opens every changelog entry with the English OpenAI original
- Adds one **Translate** button to every entry when Token Meter runs in German
- Places that button at the beginning of each card before the potentially long changelog body
- Contacts Google Translate only after the user selects that button and translates only the selected public entry
- Sends long translations sequentially instead of creating parallel Google requests
- Recognizes Google's HTTP 429 response, pauses further attempts for ten minutes and shows a precise per-entry message
- Caches successful German translations locally and lets the user switch the selected card back to its original
- Shows a failure only on the selected card while leaving all English originals available
- Opens a dedicated progress window while an automatic update is downloaded
- Shows the installer's progress during the unattended installation and restarts Token Meter afterwards
- Caches the most recently retrieved entries and read IDs locally for temporary offline use
- Sends only the public OpenAI changelog text for translation; no Token Meter account, token or authentication data is sent to Google
- Adds no bundled AI translation model and therefore no large model payload to the installer
- Keeps all existing accounts, authentication profiles, settings and quota history during the update

## Deutsch

Macht Changelog-Übersetzungen zur bewussten Benutzerauswahl und zeigt den Fortschritt automatischer Programmupdates sichtbar an.

- Fügt direkt links neben dem Plus für neue Konten einen Neuerungs-Button ein
- Liest den offiziellen ChatGPT- und Codex-Changelog direkt von learn.chatgpt.com
- Zählt bisher ungelesene offizielle Einträge aus den letzten sieben Kalendertagen
- Zeigt die Anzahl als rote Zahl; beim Öffnen gelten die aktuell dargestellten Einträge als gelesen
- Aktiviert die rote Zahl automatisch wieder, sobald OpenAI einen weiteren Eintrag veröffentlicht
- Öffnet den Changelog in einem größenveränderbaren Fenster mittig auf dem aktuellen Bildschirm
- Öffnet jeden Changelog-Eintrag grundsätzlich mit dem englischen OpenAI-Original
- Zeigt in der deutschen Oberfläche bei jedem Eintrag einen eigenen Button **Übersetzen**
- Platziert diesen Button direkt am Anfang jeder Karte vor dem möglicherweise langen Changelog-Text
- Kontaktiert Google Translate erst nach diesem Klick und übersetzt ausschließlich den ausgewählten öffentlichen Eintrag
- Übersetzt lange Texte nacheinander, statt mehrere Google-Anfragen parallel auszulösen
- Erkennt Googles HTTP-Status 429, pausiert weitere Versuche zehn Minuten und zeigt den konkreten Grund direkt am Eintrag
- Speichert erfolgreiche deutsche Übersetzungen lokal und erlaubt für die gewählte Karte den Wechsel zurück zum Original
- Zeigt einen Übersetzungsfehler ausschließlich an der ausgewählten Karte; alle englischen Originale bleiben verfügbar
- Öffnet beim Herunterladen eines automatischen Programmupdates ein eigenes Fortschrittsfenster
- Zeigt anschließend den Installationsfortschritt, installiert weiterhin unbeaufsichtigt und startet Token Meter danach neu
- Speichert den zuletzt geladenen Stand und gelesene IDs lokal für vorübergehenden Offlinebetrieb
- Übermittelt zur Übersetzung ausschließlich öffentlichen OpenAI-Changelog-Text; keine Token-Meter-Konten, Tokenstände oder Anmeldedaten gehen an Google
- Enthält kein lokales KI-Übersetzungsmodell und vergrößert den Installer daher nicht um ein Modellpaket
- Behält beim Update alle bestehenden Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

## Verification / Prüfung

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `73FFDA9D4793D757566F9B892487E044F6BF5650A2CB3922EE0D86A3C92049B9`
