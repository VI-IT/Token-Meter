# Privacy / Datenschutz

## English

Token Meter by VI-IT is a local Windows application. It contains no advertising and does not sell personal data.

### Local account data

Accounts are added through the OpenAI/Codex authentication flow. Local account profiles, authentication material, quota snapshots, reset history, selected compact-monitor account, window positions and application settings remain on the Windows device. They are used only to authenticate the accounts selected by the user, refresh best-effort Codex quota information, detect quota-window changes and display local Codex activity.

The public installer is built without developer accounts, user accounts, passwords, cookies, browser caches, sessions or access tokens. VI-IT does not receive OpenAI account credentials, account names, email addresses, quota values or token usage through Token Meter.

### Optional technical diagnostics

Sharing technical diagnostics with VI-IT is **off by default**. The installer provides an unchecked opt-in box, and the same setting can be changed later under **About Token Meter by VI-IT**. Automatic updates preserve the existing choice and never enable diagnostics.

When enabled, Token Meter sends only:

- a randomly generated installation identifier; the VI-IT service stores only its one-way SHA-256 hash
- Token Meter version
- operating-system family, version/build and processor architecture
- one install/start record for each newly installed Token Meter version
- on an unhandled application crash: exception type, a sanitized message and sanitized stack trace
- telemetry consent schema version and event time

Before transmission, user-directory names, email-address patterns, bearer tokens, OpenAI-style secret keys and JWT-shaped credentials are removed from crash text. Full log files are not uploaded. Token Meter never includes account aliases, OpenAI email addresses, quota or token values, authentication data, cookies, prompts, conversations, file contents, computer username, hardware serial numbers or advertising identifiers in the telemetry payload.

Diagnostics are sent over HTTPS to `telemetry.vi-it.de`, a VI-IT service running on Cloudflare Workers with an EU-jurisdiction D1 database. Cloudflare necessarily processes normal connection data such as the public IP address at its network edge, but the VI-IT Worker does not read or store that address in the telemetry database. Sanitized crash reports are retained for 90 days. Inactive installation summaries are removed after 365 days; non-identifying aggregate counts may remain.

Turning diagnostics off stops future transmission immediately. The local random installation identifier is retained so enabling the option again does not create misleading duplicate installation counts. To request deletion of an installation summary, contact [info@vi-it.de](mailto:info@vi-it.de); because VI-IT stores only a hash, include the local installation identifier shown on request by VI-IT support.

### Other network connections

Network connections are made to OpenAI/ChatGPT for authentication, usage refresh and the public official changelog; to GitHub Releases for automatic application updates; and to the public `codex-reset.com` timeline for optional global-reset notifications. The changelog always displays the English original first. On a German interface, Google Translate (`translate.googleapis.com`, with `translate.google.com` as a fallback when Google throttles that endpoint) is contacted only after the user selects **Translate** for a specific entry; only that public OpenAI text is sent. The result is cached locally and reused until the OpenAI source changes. English installations do not offer or make this translation request. No Token Meter account data, authentication material, token values or usage snapshots are sent to Google Translate or the public reset timeline. These services can receive standard connection data such as the public IP address and apply their own privacy policies.

## Deutsch

Token Meter by VI-IT ist eine lokale Windows-Anwendung. Sie enthält keine Werbung und verkauft keine personenbezogenen Daten.

### Lokale Kontodaten

Konten werden über den OpenAI-/Codex-Anmeldeablauf hinzugefügt. Lokale Kontoprofile, Authentifizierungsdaten, Kontingentstände, Reset-Verlauf, das für den Kompaktmonitor ausgewählte Konto, Fensterpositionen und Programmeinstellungen verbleiben auf dem Windows-Gerät. Sie werden ausschließlich verwendet, um die vom Nutzer hinzugefügten Konten zu authentifizieren, bestmöglich verfügbare Codex-Kontingentinformationen zu aktualisieren, Änderungen des Kontingentzeitraums zu erkennen und lokale Codex-Aktivität anzuzeigen.

Der öffentliche Installer enthält keine Entwicklerkonten, Benutzerkonten, Passwörter, Cookies, Browser-Caches, Sitzungen oder Zugriffstoken. VI-IT erhält über Token Meter keine OpenAI-Zugangsdaten, Kontonamen, E-Mail-Adressen, Kontingentwerte oder Tokenverbräuche.

### Optionale technische Diagnosedaten

Das Teilen technischer Diagnosedaten mit VI-IT ist **standardmäßig ausgeschaltet**. Der Installer zeigt ein nicht vorausgewähltes Kontrollkästchen; dieselbe Einstellung kann später unter **Info zu Token Meter by VI-IT** geändert werden. Automatische Updates behalten die vorhandene Auswahl bei und aktivieren Diagnosedaten niemals selbstständig.

Bei Zustimmung sendet Token Meter ausschließlich:

- eine zufällig erzeugte Installationskennung; der VI-IT-Dienst speichert davon nur einen nicht umkehrbaren SHA-256-Hash
- die Token-Meter-Version
- Betriebssystemfamilie, Version/Build und Prozessorarchitektur
- je neu installierter Token-Meter-Version einen Installations-/Startdatensatz
- bei einem unbehandelten Programmabsturz: Ausnahmetyp, bereinigte Fehlermeldung und bereinigten Stacktrace
- Version der Einwilligungserklärung und Ereigniszeitpunkt

Vor der Übertragung werden Namen aus Benutzerverzeichnissen, Muster von E-Mail-Adressen, Bearer-Tokens, OpenAI-ähnliche geheime Schlüssel und JWT-förmige Zugangsdaten aus Absturztexten entfernt. Vollständige Protokolldateien werden nicht hochgeladen. Kontobezeichnungen, OpenAI-E-Mail-Adressen, Kontingent- oder Tokenwerte, Authentifizierungsdaten, Cookies, Eingaben, Unterhaltungen, Dateiinhalte, Windows-Benutzername, Hardware-Seriennummern und Werbekennungen sind technisch nicht Bestandteil des Telemetrieformats.

Diagnosedaten gehen verschlüsselt per HTTPS an `telemetry.vi-it.de`, einen VI-IT-Dienst auf Cloudflare Workers mit einer D1-Datenbank in EU-Gerichtsbarkeit. Cloudflare verarbeitet am Netzwerkrand technisch übliche Verbindungsdaten wie die öffentliche IP-Adresse; der VI-IT-Worker liest oder speichert diese Adresse jedoch nicht in der Telemetriedatenbank. Bereinigte Absturzberichte werden nach 90 Tagen gelöscht. Zusammenfassungen inaktiver Installationen werden nach 365 Tagen entfernt; nicht identifizierende Gesamtstatistiken dürfen erhalten bleiben.

Das Ausschalten beendet weitere Übertragungen sofort. Die lokale zufällige Installationskennung bleibt erhalten, damit ein späteres erneutes Aktivieren keine irreführenden Doppelzählungen erzeugt. Eine Löschung der Installationszusammenfassung kann über [info@vi-it.de](mailto:info@vi-it.de) angefragt werden. Da VI-IT nur einen Hash speichert, wird dafür auf Nachfrage des VI-IT-Supports die lokale Installationskennung benötigt.

### Weitere Netzwerkverbindungen

Netzwerkverbindungen erfolgen zu OpenAI/ChatGPT für Anmeldung, Kontingentaktualisierung und den öffentlichen offiziellen Changelog, zu GitHub Releases für automatische Programmupdates sowie zur öffentlichen Timeline `codex-reset.com` für optionale Mitteilungen über globale Resets. Der Changelog zeigt zunächst immer das englische Original. Bei deutscher Programmoberfläche wird Google Translate (`translate.googleapis.com`, bei Drosselung dieses Endpunkts ersatzweise `translate.google.com`) erst kontaktiert, nachdem der Benutzer bei einem bestimmten Eintrag **Übersetzen** gewählt hat; übermittelt wird ausschließlich dieser öffentliche OpenAI-Text. Das Ergebnis wird lokal gespeichert und bis zu einer Änderung des OpenAI-Quelltexts wiederverwendet. Englische Installationen bieten diese Übersetzungsanfrage nicht an. An Google Translate oder die öffentliche Reset-Timeline gehen keine Token-Meter-Kontodaten, Authentifizierungsdaten, Tokenwerte oder Nutzungsstände. Diese Dienste können übliche Verbindungsdaten wie die öffentliche IP-Adresse erhalten; für sie gelten die jeweiligen Datenschutzbestimmungen.
