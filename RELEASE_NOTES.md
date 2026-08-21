# Token Meter by VI-IT 1.0.21

## English

Fixes the explicit notification-area exit and the installer layout at high Windows scaling.

Also restores German changelog translation when Google's public JSON endpoint responds with HTTP 429 by automatically using Google's mobile translation page as a fallback.

- **Exit** in the Windows notification-area menu now always terminates the Token Meter process after bounded background cleanup
- Removes a dispatcher deadlock that could leave the executable running invisibly after Exit was selected
- Keeps the window X behavior unchanged: X still hides Token Meter in the notification area
- Stops a running Token Meter instance before the installer performs its file-in-use scan
- Prevents the unnecessary “applications are using files” installer page after Token Meter was already exited
- Renders the diagnostics checkbox caption separately so it is no longer clipped or struck through at 200% Windows scaling
- Preserves the user’s existing diagnostics preference; first-time consent remains off by default
- Keeps all linked accounts, authentication profiles, settings and quota history during the update

## Deutsch

Behebt das ausdrückliche Beenden über den Windows-Infobereich und die Installer-Darstellung bei hoher Windows-Skalierung.

Stellt außerdem die deutsche Changelog-Übersetzung wieder her, wenn Googles öffentlicher JSON-Endpunkt mit HTTP 429 antwortet; Token Meter verwendet dann automatisch Googles mobile Übersetzungsseite als Ausweichweg.

- **Beenden** im Menü des Windows-Infobereichs beendet den Token-Meter-Prozess nach einer zeitlich begrenzten Hintergrundbereinigung jetzt zuverlässig
- Entfernt eine Dispatcher-Verklemmung, durch die die EXE nach „Beenden“ unsichtbar weiterlaufen konnte
- Das Verhalten des Fenster-X bleibt unverändert: X legt Token Meter weiterhin im Infobereich ab
- Beendet eine laufende Token-Meter-Instanz, bevor der Installer seine Dateiverwendungsprüfung startet
- Verhindert dadurch die unnötige Installer-Seite „Anwendungen verwenden Dateien“, wenn Token Meter bereits beendet wurde
- Stellt die Beschriftung der Diagnose-Checkbox separat dar, damit sie bei 200-%-Windows-Skalierung nicht mehr abgeschnitten oder durchgestrichen erscheint
- Behält die vorhandene Diagnose-Einstellung des Benutzers bei; bei der Erstinstallation bleibt die Zustimmung standardmäßig ausgeschaltet
- Behält beim Update alle verknüpften Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

## Verification / Prüfung

The release build passed all 22 internal self-tests, the live official OpenAI changelog check and the live Google translation fallback check. A process-level regression test exercised the real installer shutdown signal and confirmed complete termination with zero remaining Token Meter processes.

Der Release-Build bestand alle 22 internen Selbsttests sowie die Live-Prüfungen des offiziellen OpenAI-Changelogs und des Google-Übersetzungs-Fallbacks. Ein Prozess-Regressionstest führte das echte Installer-Beendigungssignal aus und bestätigte die vollständige Beendigung ohne verbleibenden Token-Meter-Prozess.

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `AAC357C627CCE66483A1453B639C4E8A3B16DBC5F3FADD15C99EB2565D1AE623`
