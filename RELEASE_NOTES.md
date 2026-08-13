# Token Meter by VI-IT 1.0.7

## English

Critical reliability fix for automatic updates.

- Fixes an update failure where the old Token Meter instance could remain hidden in the background and prevent the new version from being installed
- The automatic installer now waits for the exact parent process to exit before replacing application files
- Token Meter now stops all account sidecars in parallel during a normal shutdown
- A 15-second exit fail-safe prevents a blocked WPF shutdown from keeping the installer waiting indefinitely
- The installer requests a graceful shutdown first and terminates only the Token Meter process tree if an older version remains unresponsive
- Unexpected installer errors are no longer silently suppressed
- Automatic installations write `update-install.log` to the temporary Token Meter update folder for diagnostics
- Accounts, authentication profiles, quota history and settings are preserved during the update

## Deutsch

Wichtige Zuverlässigkeitskorrektur für automatische Aktualisierungen.

- Behebt den Fehler, bei dem eine alte Token-Meter-Instanz unsichtbar im Hintergrund bleiben und die Installation der neuen Version verhindern konnte
- Der automatische Installer wartet nun auf das Ende des exakten Elternprozesses, bevor Programmdateien ersetzt werden
- Token Meter beendet die Hintergrunddienste aller Konten beim normalen Herunterfahren parallel
- Eine 15-sekündige Notabschaltung verhindert, dass ein blockierter WPF-Abschluss den Installer unbegrenzt warten lässt
- Der Installer fordert zuerst ein sauberes Beenden an und beendet nur dann den Token-Meter-Prozessbaum, wenn eine ältere Version nicht reagiert
- Unerwartete Installationsfehler werden nicht mehr still unterdrückt
- Automatische Installationen schreiben zur Diagnose `update-install.log` in den temporären Token-Meter-Updateordner
- Konten, Anmeldeprofile, Kontingentverlauf und Einstellungen bleiben bei der Aktualisierung erhalten

## Verification / Prüfung

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `D263F5D40AF1100BB6A4CD7268F941965806E9FDCE07A2A37E9BE52B503987FE`
