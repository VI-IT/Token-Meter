# Token Meter by VI-IT 1.0.26

[English](#english) · [Deutsch](#deutsch)

## English

Improves sign-in resilience and shows only the quota windows actually reported for an account.

- Hides unavailable five-hour limits in both the manager and compact monitor. A single available limit fills the compact monitor's width; missing values are not invented as 100%.
- Shows five-hour quota on the left and weekly quota on the right when both exist.
- Uses the reported monthly or other longer quota with its correct label when no weekly window exists.
- Keeps the compact monitor mouse-resizable, remembers its dimensions and position, and restores the manager on double-click without immediately shrinking again.
- Preserves the last confirmed account and quotas during temporary service, network or background-process errors, with a clear stale-data warning. Stale values cannot trigger fresh quota alerts.
- Retries an explicit HTTP 401 once after a targeted managed-session refresh, with a five-minute cooldown. Normal polling does not force token rotation. Revoked or expired refresh tokens can still require signing in again.
- Serializes background-process startup, restart and per-account refreshes to prevent duplicate processes and old responses interfering with a replacement process.
- Reports damaged or unreadable settings instead of silently replacing saved accounts with an empty list.
- Waits for complete local session-log lines before counting them, preventing split UTF-8 records from losing token activity or completion events.
- Defers the immediate automatic-update retry after a cancelled or unsuccessful installation.
- Preserves linked accounts and existing diagnostic-data preferences during the update.

## Deutsch

Verbessert die Zuverlässigkeit der Anmeldung und zeigt ausschließlich tatsächlich gemeldete Kontingentfenster eines Kontos an.

- Blendet nicht vorhandene 5-Stunden-Limits im Hauptfenster und Minifenster aus. Ein einzelnes vorhandenes Limit nutzt die volle Breite des Minifensters; fehlende Werte werden nicht als 100% erfunden.
- Zeigt bei zwei vorhandenen Limits das Stundenkontingent links und das Wochenkontingent rechts.
- Nutzt bei fehlendem Wochenfenster das gemeldete Monats- oder andere längere Kontingent mit passender Beschriftung.
- Lässt das Minifenster per Maus skalieren, merkt sich Größe und Position und öffnet die große Ansicht per Doppelklick, ohne sofort wieder klein zu werden.
- Erhält bei vorübergehenden Dienst-, Netzwerk- oder Hintergrundprozessfehlern den zuletzt bestätigten Kontostatus und kennzeichnet veraltete Werte. Daraus entstehen keine neuen Kontingentwarnungen.
- Erneuert bei einem eindeutigen HTTP 401 die verwaltete Sitzung gezielt und wiederholt den Abruf einmal; weitere Erneuerungsversuche sind für fünf Minuten gesperrt. Normale Abrufe erzwingen keine Token-Erneuerung. Widerrufene oder abgelaufene Refresh-Tokens können weiterhin eine Neuanmeldung erfordern.
- Koordiniert Start, Neustart und kontobezogene Abrufe der Hintergrundprozesse, damit keine doppelten Prozesse oder verspäteten Antworten alter Prozesse stören.
- Meldet beschädigte oder unlesbare Einstellungen, statt gespeicherte Konten unbemerkt durch eine leere Liste zu ersetzen.
- Verarbeitet lokale Sitzungsprotokolle erst nach vollständigem Schreiben einer Zeile. Geteilte UTF-8-Zeichen verlieren dadurch keine Tokenaktivität oder Abschlussereignisse mehr.
- Verhindert den unmittelbaren erneuten automatischen Installationsversuch nach einem abgebrochenen oder fehlgeschlagenen Update.
- Erhält verknüpfte Konten und die bestehende Entscheidung zu Diagnosedaten beim Update.

## Verification / Prüfung

The release build passed all 26 internal test groups, including optional-quota WPF layout, authentication recovery and cooldown, concurrent background-process restart, settings-read failures, update cancellation and partially written session logs. Live linked-profile checks confirmed both dual-window and weekly-only responses; some upstream HTTP 401 responses persisted after recovery, so this release does not claim to prevent every OpenAI session or authorization failure. No credentials or private account diagnostics are published.

Der Release-Build bestand alle 26 internen Testgruppen, einschließlich WPF-Layout bei optionalen Limits, Sitzungswiederherstellung und Sperrzeit, parallelem Hintergrundprozess-Neustart, Einstellungs-Lesefehlern, Update-Abbruch und teilweise geschriebenen Sitzungsprotokollen. Live-Prüfungen bestätigten Antworten mit beiden Limits sowie ausschließlich mit Wochenlimit; einzelne HTTP-401-Antworten des Dienstes blieben trotz Wiederherstellungsversuch bestehen. Die Version verspricht daher keine Verhinderung sämtlicher OpenAI-Sitzungs- oder Berechtigungsfehler. Zugangsdaten und private Kontodiagnosen werden nicht veröffentlicht.

Installer: `Token-Meter-by-VI-IT-Setup.exe` · SHA-256: see attached `SHA256.txt` / siehe angehängte `SHA256.txt`.
