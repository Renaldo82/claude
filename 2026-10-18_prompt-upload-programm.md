# Prompt für die Sitzung am PC: eigenes Upload-Programm für die Website

Stand: 18.10.2026. Entstanden in einer Claude-Code-Sitzung in der Cloud, die keinen Zugriff auf Renés PC und Vault hatte.

Anlass: Ein LinkedIn-Beitrag (Florian Knust, „CleverFTP“) zeigt ein selbst gebautes Programm zum Hochladen von Dateien auf die eigene Website, das Claude über einen lokalen Anschluss (MCP-Server) selbst bedienen kann. René will so etwas für seine Website bei All-Inkl, ohne sich jedes Mal im Browser bei All-Inkl einloggen zu müssen.

So nutzen: Den Block unten komplett in den Claude-Chat am PC kopieren (dort, wo Claude Zugriff auf den Vault und die Dateien hat).

---

```
Auftrag: Baue mir ein eigenes, kleines Upload-Programm für meine Website bei All-Inkl, inklusive Anschluss für Claude (lokaler MCP-Server), damit du im Claude-Chat Dateien selbst auf meine Website hochladen kannst. Ziel: Ich muss mich nie wieder im Browser bei All-Inkl einloggen, um Dateien hochzuladen.

Arbeite so autonom wie möglich, ich bin oft 30 bis 60 Minuten nicht am PC.

SCHRITT 1: Selbst klären (nicht mich fragen, sondern nachsehen)
- Lies START.md, _AI-Bridge/CLAUDE.md und _AI-Bridge/kontext.md im Vault.
- Finde im Vault heraus, um welche Website(s) bei All-Inkl es geht (Adresse, Zweck, ggf. Ordner auf dem Server). Suche nach „All-Inkl“, „all-inkl“, „kasserver“, „Webspace“, „FTP“, „Website“, „Domain“.
- Prüfe am PC: Windows-Version, ob Python (python --version, py --version) und/oder Node.js installiert sind, ob der Claude-Desktop-Konfigurationsordner existiert (%APPDATA%\Claude\).
- Prüfe, ob es schon lokale Kopien der Website-Dateien gibt (z. B. ein Ordner mit index.html, impressum.html).
- Fasse das Ergebnis in 5 Sätzen zusammen. Nur wenn etwas wirklich nicht herauszufinden ist, frag mich mit Buchstaben-Optionen (Empfehlung zuerst).

SCHRITT 2: Bauen
Technik (Vorschlag, begründet abweichen ist ok):
- Python, weil die Bausteine dafür schon eingebaut oder klein sind:
  ftplib (FTP_TLS, verschlüsselte Übertragung, All-Inkl unterstützt das), keyring (speichert das Passwort im Windows-Passwortspeicher, der „Anmeldeinformationsverwaltung“), tkinter für das Fenster, das offizielle Paket „mcp“ (FastMCP) für den Claude-Anschluss.
- Ablageort für den Programmcode: C:\Users\Rene\AI-Kontext\Tools\website-upload\ (nicht im Vault). Eine kurze Anleitung als Notiz in den Vault legen.
- Neutraler Name, keine Marke (z. B. „Website-Upload“).

Funktionen Programmfenster:
- Server verwalten (mehrere Zugänge möglich: Name, Server, Benutzer, Startordner).
- Links mein PC, rechts der Server; hochladen, herunterladen, Ordner wechseln.
- Passwortfeld: Ich tippe das Passwort EINMAL selbst ein, es wird nur im Windows-Passwortspeicher abgelegt, nie in einer Datei, nie im Klartext, nie im Chat.

Funktionen Claude-Anschluss (MCP):
- Ordner auf dem Server auflisten.
- Datei oder Ordner hochladen, IMMER zuerst als Vorschau („diese 4 Dateien würden hochgeladen, diese 2 überschrieben“) und erst nach meiner Freigabe im Chat wirklich hochladen.
- Vor dem Überschreiben die alte Fassung vom Server herunterladen und nach _backups/JJJJ-MM-TT/ sichern.
- Datei herunterladen.
- KEIN Löschen auf dem Server über Claude.
- Das Passwort wird nie an Claude zurückgegeben.

Anschluss an Claude: Den MCP-Server in der Claude-Desktop-Konfiguration eintragen. Vorher Backup der Konfigurationsdatei nach _backups/JJJJ-MM-TT/, bestehende Einträge nicht verändern, nur ergänzen.

SCHRITT 3: Übergabe an mich
- Sag mir, wo ich im All-Inkl-Kundenmenü (KAS) den FTP-Zugang finde oder einen eigenen anlege (am besten einen eigenen Zugang nur für den Website-Ordner, nicht den Hauptzugang). Den Login im KAS mache ich selbst.
- Sag mir, wo ich das Passwort im Programm einmal eintrage.
- Erster Test: nur Ordner auflisten, nichts hochladen.
- Danach ein Probe-Upload einer harmlosen Testdatei (z. B. test-upload.txt), nach meiner Freigabe.

Regeln:
- Nie Zugangsdaten eingeben, speichern oder von mir anfordern. Das Passwort tippe ich selbst ins Programm.
- Nichts auf der Website live schalten ohne meine Freigabe.
- Keine Kosten, keine Abos.
- Antworten kurz, kein Fachjargon, Fachbegriffe mit Alltagsvergleich erklären.
- Ergebnis-Zusammenfassung zusätzlich in die Outbox (Dateiname mit Datum) und den Pfad nennen.
```
