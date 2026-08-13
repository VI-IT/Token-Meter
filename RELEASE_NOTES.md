# Token Meter by VI-IT 1.0.8

## English

Critical fixes for false refill alerts and opaque automatic updates.

- A quota-refill alert now requires an actual increase in remaining weekly capacity
- An unchanged 100% value can no longer generate a refill or reset event
- Stabilizes reset timestamps that incorrectly move forward on every refresh
- Automatically removes repeated rolling 100% events created by version 1.0.7 from reset history
- The **Dismiss** button now remains effective because no replacement event is generated one minute later
- Shows update download percentage and transferred megabytes inside the app
- Extends the update download timeout from 5 to 30 minutes for slower connections
- Reads the release-asset SHA-256 digest from GitHub and reuses a complete verified cached installer
- Uses an independent temporary update worker that waits for the app, runs the installer and explicitly restarts Token Meter
- Manual and legacy automatic installations start the application without the unreliable `runasoriginaluser` handoff
- Writes separate worker and installer diagnostic logs
- Accounts, authentication profiles, quota values and settings remain unchanged

## Deutsch

Wichtige Korrekturen für falsche Auffüllmeldungen und undurchsichtige automatische Updates.

- Eine Auffüllmeldung erfordert jetzt einen tatsächlichen Anstieg des verbleibenden Wochenkontingents
- Ein unveränderter Wert von 100 % kann keine Auffüll- oder Reset-Meldung mehr erzeugen
- Reset-Termine, die bei jeder Aktualisierung fälschlich weiterwandern, werden stabilisiert
- Von Version 1.0.7 erzeugte Serien gleicher 100-%-Meldungen werden automatisch aus dem Reset-Verlauf entfernt
- **Gesehen** bleibt wirksam, weil nicht eine Minute später ein neuer Ersatzeintrag entsteht
- Zeigt Download-Prozent und übertragene Megabyte direkt im Programm
- Verlängert das Download-Zeitlimit für langsamere Verbindungen von 5 auf 30 Minuten
- Liest die SHA-256-Prüfsumme des Release-Assets von GitHub und verwendet einen vollständig geprüften Cache weiter
- Verwendet einen unabhängigen temporären Update-Wächter, der auf das Programmende wartet, den Installer ausführt und Token Meter ausdrücklich neu startet
- Manuelle und ältere automatische Installationen starten die Anwendung ohne die unzuverlässige `runasoriginaluser`-Übergabe
- Schreibt getrennte Diagnoseprotokolle für Update-Wächter und Installer
- Konten, Anmeldeprofile, Kontingentwerte und Einstellungen bleiben unverändert

## Verification / Prüfung

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `3536F41878CBA3FD428F4FA8A50BD00F2639CC9F890B653B1C2FD1986F6D86C8`
