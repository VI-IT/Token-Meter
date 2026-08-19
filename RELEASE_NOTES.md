# Token Meter by VI-IT 1.0.11

## English

Restores reliable per-account LIVE activity and prevents unnecessary repeated sign-in requests.

- Stops forcing an OAuth token refresh during every periodic account check
- Uses the passive account status read recommended by the Codex app-server protocol
- Matches ChatGPT/Codex desktop activity to the correct linked account when the result is unambiguous
- Shows local LIVE chat count and local consumption inside that account card again
- Keeps an unassigned local row only when several workspaces cannot be distinguished safely
- Replaces the unclear `Today: awaiting API` text with `Consumed today: not yet reported by OpenAI`
- Clarifies that the account token figure is total consumption, not a remaining token balance
- Explains that OpenAI supplies remaining weekly percentage and reset time, but no fixed absolute token capacity
- Preserves all existing accounts, authentication profiles, settings and quota history during the update

## Deutsch

Stellt die zuverlässige LIVE-Anzeige pro Konto wieder her und verhindert unnötige wiederholte Anmeldeaufforderungen.

- Erzwingt bei der regelmäßigen Kontoprüfung nicht mehr jedes Mal einen OAuth-Token-Refresh
- Verwendet die passive Kontoabfrage des Codex-App-Server-Protokolls
- Ordnet ChatGPT-/Codex-Desktop-Aktivität wieder dem richtigen verknüpften Konto zu, wenn das Ergebnis eindeutig ist
- Zeigt lokale LIVE-Chats und lokalen Verbrauch wieder direkt in dieser Kontokarte
- Behält die getrennte lokale Zeile nur dann bei, wenn mehrere Arbeitsbereiche nicht sicher unterschieden werden können
- Ersetzt den unklaren Text `Heute: API ausstehend` durch `Heute verbraucht: von OpenAI noch nicht gemeldet`
- Stellt klar, dass die Tokenzahl den Gesamtverbrauch und kein verbleibendes Token-Guthaben darstellt
- Erklärt, dass OpenAI Restprozent und Reset-Zeit, aber keine feste absolute Token-Gesamtmenge liefert
- Behält beim Update alle bestehenden Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

## Verification / Prüfung

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `FBEA72C60D85C3031A1856A2E1CA96F2ACF821FB59A7D34623C5C4AFD9275F64`
