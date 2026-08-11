# Token Meter by VI-IT

**Global Codex reset alerts, weekly quota and live token monitoring for multiple ChatGPT accounts on Windows.**

[English](#english) · **[Deutsche Anleitung](#deutsch)** · [Download](https://github.com/VI-IT/Token-Meter/releases/latest) · [Privacy](PRIVACY.md) · [Support](SUPPORT.md)

| Support development |
| --- |
| [<img src="assets/kofi-icon.png" alt="Ko-fi" width="24"> **Ko-fi**](https://ko-fi.com/viitde) &nbsp;&nbsp; [<img src="assets/paypal-icon.png" alt="PayPal" width="24"> **PayPal**](https://paypal.me/viitde) |

---

<a id="english"></a>

## English

Token Meter by VI-IT alerts Windows users when a newly reported global Codex usage reset appears in the public Codex Reset Timeline. The compact desktop widget also monitors remaining weekly quota, exact reset times, account token totals and live Codex activity across multiple ChatGPT accounts.

<img src="assets/token-meter-live-en.png" alt="Token Meter English interface with live local Codex activity" width="480">

### Download for Windows

**[Download the latest installer](https://github.com/VI-IT/Token-Meter/releases/latest/download/Token-Meter-by-VI-IT-Setup.exe)**

- Windows 10 or Windows 11, 64-bit
- Self-contained installer; no separate .NET runtime required
- Future releases can be installed automatically at startup

> The installer is currently not Authenticode-signed. Windows SmartScreen may therefore display an unknown-publisher warning. Only download releases from this repository and verify the published SHA-256 checksum.

### Main feature: global Codex reset alerts

Token Meter checks the public Codex Reset Timeline directly every two minutes. When a new global reset post linked to `@thsottiaux` appears, it shows a one-time Windows notification that opens the original X source when clicked. No VI-IT server, user registration or paid API is required.

### Features

- Receive automatic Windows alerts for newly reported global Codex usage resets
- Monitor multiple separately authenticated ChatGPT/OpenAI accounts
- Compare remaining Codex weekly quota and exact reset time
- See token totals and consumption changes reported for each account
- See the current daily value from the account service, with a clearly marked local minimum while that value is delayed
- See how many Codex chats are actively processing on this Windows PC
- Automatically rank accounts with the most remaining capacity first
- Keep depleted accounts collapsed until you need them
- Receive a one-time Windows notification on the exact 11% → 10% transition
- Receive one-time notifications for regular resets within 24 hours and detected quota refills
- Rename accounts locally and reopen the official sign-in flow when needed
- Use German automatically on German Windows; English on all other Windows display languages
- Run in the Windows notification area and optionally start with Windows
- Install future GitHub releases automatically and silently at startup

### How it works

Each account is authenticated separately through the OpenAI/Codex sign-in flow. Quota and account token totals are requested for the linked account. The green LIVE indicator and active-chat count are derived from Codex session files on the Windows PC where Token Meter is running.

The account service can publish the current daily-usage bucket later than the lifetime total. Until that bucket arrives, Token Meter shows `Today: awaiting API` or, when local Codex activity is available, a clearly marked local minimum. The local minimum covers this PC only; the server value can later include usage from other devices.

Activity on another PC is **not included in the LIVE chat count**. Usage from another device can later change the account's quota or token total when OpenAI reports an updated value, but Token Meter cannot identify how many chats are currently active on that other device. The underlying OpenAI endpoints and local session formats are not public stable APIs and can change.

When the account token total increases because of activity on another device, Token Meter shows the newly detected token difference in red on the next successful account refresh. OpenAI does not label that difference with a source device, so Token Meter cannot separate PC 1 from PC 2.

Regular weekly reset timestamps can be announced up to 24 hours in advance. For extraordinary service-wide resets, Token Meter also reads the public `codex-reset.com` timeline directly every two minutes and shows a one-time Windows notification when it publishes a new global reset post linked to `@thsottiaux`. Existing timeline entries are silently remembered on first use, so historical posts do not trigger old alerts. This optional public signal requires no VI-IT server, account or API key; if it is unavailable, normal quota and LIVE monitoring continue unaffected.

The central ChatGPT button opens the existing official ChatGPT desktop app. OpenAI does not currently provide Token Meter with an official Windows account-handoff interface, so ChatGPT opens with the account that was last active in ChatGPT itself.

### Privacy and security

- No passwords are requested or stored by Token Meter
- No analytics, advertising or VI-IT cloud service is used
- Account profiles, authentication material and usage snapshots remain on the local Windows device
- The distributed installer contains no developer accounts, cookies, sessions, caches or access tokens
- Removing an account from Token Meter removes only its local Token Meter profile

Read the complete [privacy information](PRIVACY.md) and [security policy](SECURITY.md).

### Installation

1. Download `Token-Meter-by-VI-IT-Setup.exe` from the latest release.
2. Run the installer for the current Windows user.
3. Start Token Meter and select **+** to add an account.
4. Complete the official OpenAI sign-in in your browser.

When a newer GitHub release is available, Token Meter downloads and installs it automatically when the app starts.

### Support development

[Say thanks via Ko-fi](https://ko-fi.com/viitde) · [Support via PayPal](https://paypal.me/viitde)

Support is voluntary and does not unlock features.

---

<a id="deutsch"></a>

## Deutsch

Token Meter by VI-IT benachrichtigt Windows-Nutzer, sobald in der öffentlichen Codex Reset Timeline ein neuer globaler Codex-Kontingentreset gemeldet wird. Das kompakte Desktop-Widget überwacht zusätzlich Wochenkontingent, genaue Reset-Zeiten, kontobezogene Tokenstände und lokale Codex-Liveaktivität für mehrere ChatGPT-Konten.

<img src="assets/token-meter-live-de.png" alt="Deutsche Token-Meter-Oberfläche mit lokaler Codex-Liveaktivität" width="480">

### Download für Windows

**[Aktuellen Installer herunterladen](https://github.com/VI-IT/Token-Meter/releases/latest/download/Token-Meter-by-VI-IT-Setup.exe)**

- Windows 10 oder Windows 11, 64 Bit
- Vollständiger Installer; keine separate .NET-Laufzeit erforderlich
- Zukünftige Versionen können beim Start automatisch installiert werden

> Der Installer ist derzeit nicht mit einem Authenticode-Zertifikat signiert. Windows SmartScreen kann deshalb einen Hinweis auf einen unbekannten Herausgeber anzeigen. Lade die Datei ausschließlich aus diesem Repository herunter und vergleiche bei Bedarf die veröffentlichte SHA-256-Prüfsumme.

### Hauptfunktion: globale Codex-Reset-Meldungen

Token Meter prüft alle zwei Minuten direkt die öffentliche Codex Reset Timeline. Erscheint dort ein neuer globaler Reset-Beitrag von `@thsottiaux`, zeigt das Programm einmalig eine Windows-Mitteilung und öffnet beim Anklicken die ursprüngliche X-Quelle. Dafür sind weder ein VI-IT-Server noch eine Benutzerregistrierung oder kostenpflichtige API erforderlich.

### Funktionen

- Automatische Windows-Mitteilungen über neu gemeldete globale Codex-Kontingentresets erhalten
- Mehrere getrennt angemeldete ChatGPT-/OpenAI-Konten überwachen
- Verbleibendes Codex-Wochenkontingent und genaue Reset-Zeit vergleichen
- Kontobezogene Tokenstände und Verbrauchsänderungen anzeigen
- Aktuellen Tageswert des Kontodienstes sehen; bei Verzögerung mit klar gekennzeichnetem lokalen Mindestwert
- Anzeigen, wie viele Codex-Chats auf diesem Windows-PC gerade verarbeitet werden
- Konten mit dem größten verbleibenden Kontingent automatisch nach oben sortieren
- Verbrauchte Konten platzsparend einklappen
- Einmalige Windows-Warnung ausschließlich beim exakten Übergang von 11 % auf 10 %
- Einmalige Mitteilungen bei regulären Resets innerhalb von 24 Stunden und bei erkannten Kontingentauffüllungen
- Konten lokal umbenennen und bei Bedarf die offizielle Browser-Anmeldung erneut öffnen
- Deutsche Oberfläche unter deutschem Windows, sonst automatisch Englisch
- Betrieb im Windows-Infobereich und optionaler Windows-Autostart
- Zukünftige GitHub-Versionen beim Programmstart automatisch und still installieren

### Funktionsweise

Jedes Konto wird getrennt über den OpenAI-/Codex-Anmeldeablauf authentifiziert. Kontingent und kontobezogene Tokenstände werden für das verknüpfte Konto abgefragt. Die grüne LIVE-Anzeige und die Zahl aktiver Chats werden dagegen aus Codex-Sitzungsdateien auf genau dem Windows-PC ermittelt, auf dem Token Meter läuft.

Der Kontodienst kann den aktuellen Tages-Bucket später bereitstellen als den gesamten Tokenstand. Bis dahin zeigt Token Meter `Heute: API ausstehend` oder – falls lokale Codex-Aktivität vorhanden ist – einen klar gekennzeichneten lokalen Mindestwert. Dieser Mindestwert umfasst nur diesen PC; der spätere Serverwert kann auch Nutzung anderer Geräte enthalten.

Aktivität auf einem zweiten PC wird **nicht in der LIVE-Chat-Anzahl mitgezählt**. Deren Verbrauch kann sich später im Kontingent oder Tokenstand bemerkbar machen, sobald OpenAI einen aktualisierten Wert liefert. Token Meter kann jedoch nicht erkennen, wie viele Chats auf dem anderen Gerät gerade aktiv sind. Die zugrunde liegenden OpenAI-Endpunkte und lokalen Sitzungsformate sind keine stabilen öffentlichen APIs und können sich ändern.

Steigt der kontobezogene Tokenstand durch Aktivität auf einem anderen Gerät, zeigt Token Meter die neu erkannte Token-Differenz nach der nächsten erfolgreichen Kontoaktualisierung rot an. OpenAI kennzeichnet diese Differenz nicht mit einem Ursprungsgerät; deshalb kann Token Meter PC 1 und PC 2 dabei nicht auseinanderhalten.

Reguläre Wochenreset-Termine können bis zu 24 Stunden vorher angekündigt werden. Bei außergewöhnlichen dienstweiten Resets liest Token Meter zusätzlich alle zwei Minuten direkt die öffentliche Timeline von `codex-reset.com` und zeigt einmalig eine Windows-Mitteilung, sobald dort ein neuer globaler Reset-Beitrag von `@thsottiaux` erscheint. Beim ersten Abruf werden vorhandene Einträge still vorgemerkt, damit keine alten Meldungen erscheinen. Dieses optionale öffentliche Signal benötigt weder einen VI-IT-Server noch ein Konto oder einen API-Schlüssel; fällt die Timeline aus, laufen Kontingent- und LIVE-Überwachung unverändert weiter.

Der zentrale ChatGPT-Button öffnet die bereits installierte offizielle ChatGPT-Desktop-App. OpenAI stellt Token Meter derzeit keine offizielle Windows-Schnittstelle zur Kontoübergabe bereit. Deshalb öffnet ChatGPT mit dem zuletzt innerhalb von ChatGPT aktiven Konto.

### Datenschutz und Sicherheit

- Token Meter fragt keine Passwörter ab und speichert keine Passwörter
- Keine Analysefunktionen, Werbung oder VI-IT-Cloud
- Kontoprofile, Authentifizierungsdaten und Nutzungsstände bleiben lokal auf dem Windows-Gerät
- Der veröffentlichte Installer enthält keine Entwicklerkonten, Cookies, Sitzungen, Caches oder Zugriffstoken
- Das Entfernen eines Kontos löscht ausschließlich dessen lokales Token-Meter-Profil

Lies die vollständigen [Datenschutzinformationen](PRIVACY.md) und die [Sicherheitsrichtlinie](SECURITY.md).

### Installation

1. `Token-Meter-by-VI-IT-Setup.exe` aus dem neuesten Release herunterladen.
2. Installer für den aktuellen Windows-Benutzer ausführen.
3. Token Meter starten und über **+** ein Konto hinzufügen.
4. Die offizielle OpenAI-Anmeldung im Browser abschließen.

Wenn ein neueres GitHub-Release verfügbar ist, lädt Token Meter es beim Programmstart automatisch herunter und installiert es.

### Entwicklung unterstützen

[Über Ko-fi Danke sagen](https://ko-fi.com/viitde) · [Mit PayPal unterstützen](https://paypal.me/viitde)

Die Unterstützung ist freiwillig und schaltet keine zusätzlichen Funktionen frei.

---

## Contact / Kontakt

- Website: [www.vi-it.de](https://www.vi-it.de)
- Email: [info@vi-it.de](mailto:info@vi-it.de)
- Issues: [GitHub Issues](https://github.com/VI-IT/Token-Meter/issues)

Token Meter by VI-IT is distributed as closed-source Windows software. Source code is not included in this public release repository.

ChatGPT and Codex are trademarks of OpenAI. Token Meter by VI-IT is independent software and is not affiliated with, sponsored, certified, or endorsed by OpenAI.

ChatGPT und Codex sind Marken von OpenAI. Token Meter by VI-IT ist unabhängige Software und nicht mit OpenAI verbunden, von OpenAI gesponsert, zertifiziert oder empfohlen.
