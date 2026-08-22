# Token Meter by VI-IT 1.0.22

## English

Fixes frozen or incorrectly assigned local LIVE activity after new Codex session records, desktop exit, sign-out or a later account sign-in.

- Safely accepts new Codex rollout records whose JSON root or payload is not an object instead of silently stopping the two-second LIVE refresh loop
- Detects whether the unified ChatGPT/Codex desktop app is running
- Clears the previous desktop account mapping and local LIVE state when Codex is closed
- Detects sign-out and removes stale activity from the account that was previously active
- Confirms the current Codex sign-in before assigning LIVE activity after a new sign-in, account switch or workspace switch
- Keeps activity unassigned if the current account cannot be identified safely instead of guessing an old or unrelated account
- Ends an incomplete local turn after Codex exits instead of leaving LIVE green indefinitely
- Handles non-object app-server responses defensively so future optional fields cannot freeze the display
- Keeps all linked accounts, authentication profiles, settings and quota history during the update

## Deutsch

Behebt eingefrorene oder falsch zugeordnete lokale LIVE-Aktivität nach neuen Codex-Sitzungseinträgen, dem Beenden der Desktop-App, einer Abmeldung oder einer späteren Kontoanmeldung.

- Verarbeitet neue Codex-Rollout-Einträge mit einem nicht objektförmigen JSON-Stamm oder Payload sicher, statt die zweisekündliche LIVE-Aktualisierung unbemerkt anzuhalten
- Erkennt, ob die gemeinsame ChatGPT-/Codex-Desktop-App läuft
- Löscht die bisherige Desktop-Kontozuordnung und den lokalen LIVE-Zustand, sobald Codex beendet wird
- Erkennt eine Abmeldung und entfernt veraltete Aktivität vom zuvor aktiven Konto
- Bestätigt die aktuelle Codex-Anmeldung, bevor LIVE nach einer neuen Anmeldung sowie einem Konto- oder Arbeitsbereichswechsel zugeordnet wird
- Lässt Aktivität ohne Kontozuordnung, wenn das aktive Konto nicht sicher erkannt werden kann, statt ein altes oder fremdes Konto zu erraten
- Beendet einen unvollständigen lokalen Turn nach dem Ende von Codex, statt LIVE unbegrenzt grün zu lassen
- Behandelt nicht objektförmige App-Server-Antworten defensiv, damit zukünftige optionale Felder die Anzeige nicht einfrieren
- Behält beim Update alle verknüpften Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

## Verification / Prüfung

The published single-file build passed all 22 internal self-tests. Installed integration checks confirmed the current desktop identity maps to the matching linked account and the embedded Codex 0.148.0 component can read the signed-in account, account usage and local active-thread list. No account data is included in the reports.

Der veröffentlichte Einzeldatei-Build bestand alle 22 internen Selbsttests. Installierte Integrationstests bestätigten die Zuordnung der aktuellen Desktop-Identität zum passenden verknüpften Konto sowie das Lesen des angemeldeten Kontos, des Kontoverbrauchs und der lokalen aktiven Thread-Liste über die eingebettete Codex-Komponente 0.148.0. Die Prüfberichte enthalten keine Kontodaten.

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `7A25B16000C04489CC6F60D5432937DD0F60F0244A52B3F9004C8C8241EA23B7`
