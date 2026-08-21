# Token Meter by VI-IT 1.0.20

## English

Fixes incorrect LIVE account attribution after switching the account or workspace in the ChatGPT desktop app.

- Reads the fresh ChatGPT/Codex desktop identity before every local LIVE refresh
- Invalidates the previous account assignment immediately when the desktop account or workspace changes
- Restarts the internal account reader so a cached old identity cannot remain attached to the former account
- Treats the fresh local desktop identity as authoritative when a background response is stale
- Distinguishes workspaces that use the same e-mail address through a privacy-preserving, one-way in-memory fingerprint
- Keeps ambiguous local activity unassigned instead of showing it on the wrong account
- Adds a sanitized installed integration check for the real mapping path; the report contains no e-mail addresses or account identifiers
- Keeps all linked accounts, authentication profiles, settings and quota history during the update

## Deutsch

Behebt eine falsche LIVE-Kontozuordnung nach dem Wechsel des Kontos oder Arbeitsbereichs in der ChatGPT-Desktop-App.

- Liest die aktuelle ChatGPT-/Codex-Desktop-Identität vor jeder lokalen LIVE-Aktualisierung frisch ein
- Verwirft die bisherige Kontozuordnung sofort, sobald das Desktop-Konto oder der Arbeitsbereich wechselt
- Startet den internen Kontoleser neu, damit keine zwischengespeicherte alte Identität am vorherigen Konto hängen bleibt
- Behandelt die frisch gelesene lokale Desktop-Identität als maßgeblich, wenn eine Hintergrundantwort veraltet ist
- Unterscheidet Arbeitsbereiche mit derselben E-Mail-Adresse über einen datensparsamen, nicht umkehrbaren Fingerabdruck im Arbeitsspeicher
- Lässt mehrdeutige lokale Aktivität bewusst ohne Kontozuordnung, statt sie beim falschen Konto anzuzeigen
- Ergänzt einen bereinigten Installationstest für den echten Zuordnungsweg; der Bericht enthält weder E-Mail-Adressen noch Konto-IDs
- Behält beim Update alle verknüpften Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

## Verification / Prüfung

The release build passed all 22 internal self-tests and the installed-account mapping integration check. The integration report confirmed that the current desktop identity was linked to the matching Token Meter account without exposing account data.

Der Release-Build bestand alle 22 internen Selbsttests sowie die Integrationsprüfung mit den installierten Konten. Der bereinigte Bericht bestätigte, dass die aktuelle Desktop-Identität dem passenden Token-Meter-Konto zugeordnet wurde, ohne Kontodaten auszugeben.

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `3207CBE3ECABC7BEFF5440011A5F1BB3B8AFF7CEAA801E8A9509E37CCA6FB932`
