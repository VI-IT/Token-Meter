# Token Meter by VI-IT 1.0.24

## English

Adds flexible browser sign-in and keeps the currently confirmed ChatGPT/Codex desktop account at the top of the account list.

- Adds **Copy sign-in link** when creating a new account
- Adds the same **Copy sign-in link** action to every existing account menu
- Copies a freshly generated official OpenAI/Codex sign-in URL while Token Meter keeps the matching local sign-in attempt active
- Keeps **Sign in using browser** as the direct one-click option
- Shows a visible confirmation after the link has reached the Windows clipboard
- Pins the uniquely confirmed current ChatGPT/Codex desktop account above every other account, regardless of remaining quota
- Keeps the current account visible even at 0% instead of moving it into the collapsed depleted section
- Preserves the existing remaining-capacity order for every other account
- Keeps all linked accounts, authentication profiles, settings and quota history during the update

## Deutsch

Ergänzt eine flexible Browser-Anmeldung und hält das aktuell bestätigte ChatGPT-/Codex-Desktop-Konto ganz oben in der Kontenliste.

- Fügt beim Erstellen eines Kontos **Anmeldelink kopieren** hinzu
- Fügt dieselbe Aktion **Anmeldelink kopieren** im Menü jedes bestehenden Kontos hinzu
- Kopiert einen frisch erzeugten offiziellen OpenAI-/Codex-Anmeldelink, während Token Meter den passenden lokalen Anmeldeversuch aktiv hält
- Behält **Im Browser anmelden** als direkte Ein-Klick-Option bei
- Zeigt eine sichtbare Bestätigung, sobald der Link in der Windows-Zwischenablage liegt
- Fixiert das eindeutig bestätigte aktuelle ChatGPT-/Codex-Desktop-Konto unabhängig vom Restkontingent über allen anderen Konten
- Lässt das aktuelle Konto selbst bei 0% sichtbar, statt es in den eingeklappten Bereich für verbrauchte Konten zu verschieben
- Behält für alle übrigen Konten die bisherige Sortierung nach Restkontingent bei
- Behält beim Update alle verknüpften Konten, Anmeldeprofile, Einstellungen und den Kontingentverlauf bei

## Verification / Prüfung

The published single-file build passed all 22 internal self-tests, including the new current-account ordering checks and the official sign-in-link start flow. Integration checks confirmed that the current desktop identity maps to the matching linked account and that the embedded Codex 0.148.0 component can read the signed-in account, account usage and local active-thread list. No account data is included in the reports.

Der veröffentlichte Einzeldatei-Build bestand alle 22 internen Selbsttests einschließlich der neuen Prüfung für die Sortierung des aktuellen Kontos und des offiziellen Anmeldelink-Ablaufs. Integrationstests bestätigten die Zuordnung der aktuellen Desktop-Identität zum passenden verknüpften Konto sowie das Lesen des angemeldeten Kontos, des Kontoverbrauchs und der lokalen aktiven Thread-Liste über die eingebettete Codex-Komponente 0.148.0. Die Prüfberichte enthalten keine Kontodaten.

`Token-Meter-by-VI-IT-Setup.exe`

SHA-256: `9492C1554A3A4635C7F1765607CBF00CA2E950AB48BC8308E5A2E27BE5869CB5`
