# Token Meter by VI-IT 1.0.4

## English

Window-sizing, daily-usage, and quota-reset notification corrections for Windows.

- Fits the window to the visible accounts once at startup, then preserves every manual resize
- Keeps the user-selected window size unchanged during live and API refreshes
- Uses Codex account usage data when the current daily bucket is available
- Falls back to the minimum token usage observed locally today while the account API is delayed
- Shows `Today: awaiting API` instead of incorrectly reporting zero
- Notifies once when a regular weekly reset is within 24 hours
- Detects substantial quota refills and identifies simultaneous multi-account refills as a possible global reset

## Deutsch

Korrekturen für Fenstergröße, Tagesverbrauch und Kontingent-Reset-Mitteilungen unter Windows.

- Passt die Fensterhöhe beim Start einmalig an die sichtbaren Konten an und respektiert danach jede manuelle Größe
- Lässt die vom Benutzer gewählte Fenstergröße bei Live- und API-Aktualisierungen unverändert
- Verwendet den Codex-Kontotageswert, sobald dessen aktueller Tages-Bucket verfügbar ist
- Zeigt bei verzögerter Konto-API mindestens den heute lokal erfassten Tokenverbrauch
- Zeigt `Heute: API ausstehend` statt fälschlich null Verbrauch zu melden
- Meldet einmalig, wenn ein regulärer Wochenreset innerhalb der nächsten 24 Stunden bevorsteht
- Erkennt deutliche Kontingentauffüllungen und kennzeichnet gleichzeitige Auffüllungen mehrerer Konten als möglichen globalen Reset

## Verification / Prüfung

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `6E295F6948C662F220F6C19F2009FB282BFE0269BF8DF502A95EA85C3F4B179C`
