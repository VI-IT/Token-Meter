# Token Meter by VI-IT 1.0.18

## English

Adds privacy-first, optional technical diagnostics for improving Token Meter.

- Adds an unchecked diagnostics opt-in to normal installer runs
- Keeps automatic updates silent and preserves the user's existing choice
- Adds the same setting to the **About Token Meter by VI-IT** window so it can be changed at any time
- Reports one installation/start event for each newly installed Token Meter version only after opt-in
- Reports sanitized technical details when Token Meter terminates because of an unhandled application error
- Sends only Token Meter version, Windows version/build, processor architecture, consent version, event time and a random installation identifier
- Stores only a one-way SHA-256 hash of the random installation identifier on the VI-IT service
- Removes Windows usernames, email-address patterns, bearer tokens, OpenAI-style keys and JWT-shaped credentials from crash text before transmission and again on the server
- Never sends OpenAI accounts, account aliases, email addresses, quotas, token values, prompts, conversations, files, cookies or authentication material
- Uses the encrypted `telemetry.vi-it.de` endpoint backed by Cloudflare Workers and an EU-jurisdiction D1 database
- Retains sanitized crash reports for 90 days and removes inactive installation summaries after 365 days
- Updates the English and German privacy documentation with the exact payload, retention and opt-out behavior
- Keeps all existing accounts, authentication profiles, settings and quota history during the update

Technical diagnostics remain completely disabled unless the user actively enables them.

## Deutsch

Ergänzt datensparsame, freiwillige technische Diagnosedaten zur Verbesserung von Token Meter.

- Fügt bei einer normalen Installation ein nicht vorausgewähltes Diagnose-Kontrollkästchen hinzu
- Führt automatische Updates weiterhin unbeaufsichtigt aus und behält die vorhandene Auswahl des Benutzers bei
- Fügt dieselbe Einstellung im Fenster **Info zu Token Meter by VI-IT** hinzu, sodass sie jederzeit geändert werden kann
- Meldet erst nach Zustimmung je neu installierter Token-Meter-Version ein Installations-/Startereignis
- Meldet bereinigte technische Informationen, wenn Token Meter wegen eines unbehandelten Programmfehlers beendet wird
- Übermittelt ausschließlich Token-Meter-Version, Windows-Version/Build, Prozessorarchitektur, Einwilligungsversion, Ereigniszeitpunkt und eine zufällige Installationskennung
- Speichert auf dem VI-IT-Dienst nur einen nicht umkehrbaren SHA-256-Hash der zufälligen Installationskennung
- Entfernt Windows-Benutzernamen, E-Mail-Muster, Bearer-Tokens, OpenAI-ähnliche Schlüssel und JWT-förmige Zugangsdaten vor der Übertragung und erneut auf dem Server aus Absturztexten
- Übermittelt niemals OpenAI-Konten, Kontobezeichnungen, E-Mail-Adressen, Kontingente, Tokenwerte, Eingaben, Unterhaltungen, Dateien, Cookies oder Authentifizierungsdaten
- Verwendet den verschlüsselten Endpunkt `telemetry.vi-it.de` mit Cloudflare Workers und einer D1-Datenbank in EU-Gerichtsbarkeit
- Bewahrt bereinigte Absturzberichte 90 Tage auf und löscht inaktive Installationszusammenfassungen nach 365 Tagen
- Aktualisiert die deutsche und englische Datenschutzerklärung mit dem exakten Datenumfang, den Fristen und dem Abschaltverhalten
- Behält beim Update alle bestehenden Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

Technische Diagnosedaten bleiben vollständig ausgeschaltet, solange der Benutzer sie nicht selbst aktiviert.

## Verification / Prüfung

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `2E078F9176C42DB1F3433DA61D37279C3F8E716C6ABB4D24979B54F1B1C496FD`
