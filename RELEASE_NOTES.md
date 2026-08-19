# Token Meter by VI-IT 1.0.13

## English

Updates the embedded Codex component and adds truthful, capability-based credit and session-usage details.

- Replaces the embedded Codex component with the official stable Codex CLI 0.148.0
- Shows the separate OpenAI credit balance only when the account service reports an actual balance
- Requests optional active-session token and estimated credit/USD figures introduced with Codex 0.148
- Keeps those optional details hidden for accounts or workspaces where OpenAI does not provide them
- Uses local session metadata to keep the LIVE count assigned to the matching account, with a separate local row when the match is ambiguous
- Adds compatibility checks for the 0.148 app-server handshake, account usage, thread listing and per-thread usage response
- Includes the authentication, reconnect and Windows reliability fixes shipped in Codex 0.148
- Keeps all existing accounts, authentication profiles, settings and quota history during the update

## Deutsch

Aktualisiert die integrierte Codex-Komponente und ergänzt ehrliche, nur bei vorhandener Unterstützung sichtbare Credit- und Sitzungsdaten.

- Ersetzt die integrierte Codex-Komponente durch die offizielle stabile Codex CLI 0.148.0
- Zeigt das separate OpenAI-Credit-Guthaben nur, wenn der Kontodienst ein echtes Guthaben meldet
- Fragt die mit Codex 0.148 eingeführten optionalen Token- sowie geschätzten Credit-/USD-Werte aktiver Sitzungen ab
- Blendet diese Zusatzdaten bei Konten oder Workspaces ohne OpenAI-Unterstützung vollständig aus
- Ordnet die lokale LIVE-Anzahl weiterhin anhand lokaler Sitzungsmetadaten dem passenden Konto zu und verwendet bei Mehrdeutigkeit eine getrennte lokale Zeile
- Ergänzt Kompatibilitätsprüfungen für 0.148-Handshake, Kontoauskunft, Sitzungsliste und sitzungsbezogene Nutzung
- Übernimmt die in Codex 0.148 enthaltenen Verbesserungen für Anmeldung, Wiederverbindung und Windows-Zuverlässigkeit
- Behält beim Update alle bestehenden Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

## Verification / Prüfung

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `AC96814B0A302C8383984D90227B130DFAAEAD482552A0D07C310B45FCCD6DC0`
