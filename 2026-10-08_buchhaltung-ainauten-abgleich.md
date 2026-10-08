---
datum: 2026-10-08
quelle: AInauten Newsletter vom 08.10.2026 (Buchhaltung mit AI, Teil 1 + Kosten und Aufwand)
status: Entwurf, Abgleich mit dem Vault steht noch aus
ablage-vorschlag: 01-Business/Buchhaltung/ (am PC prüfen, ob es dort schon eine passende Notiz gibt)
---

# Buchhaltung mit Claude: Was wir aus dem AInauten-Newsletter für lexoffice mitnehmen

Hinweis: lexoffice heißt inzwischen offiziell "Lexware Office". Gemeint ist dasselbe Programm.

## Die 7 Tipps, übersetzt auf lexoffice

1. **Ein fester Befehl für den Belege-Lauf.** Die AInauten tippen `/belege-buchen`, und Claude arbeitet den Belegordner ab. Bei uns gibt es dafür noch keinen Skill (die Haushaltsabrechnung ist nur privat). Vorschlag: Skill `belege-lexoffice` anlegen.
2. **Nie selbst Währungen umrechnen.** Belege in Dollar (Midjourney, Ideogram, Canva, Domains, Tools aus den USA) bleiben liegen, bis der echte Euro-Betrag auf dem Kontoauszug oder der Kreditkarte steht. Für uns besonders wichtig, weil viele Design-Werkzeuge in Dollar abrechnen.
3. **Doppelte Belege aussortieren.** Claude prüft vor jedem Lauf: Rechnungsnummer, Betrag und Datum schon vorhanden? Dann nicht nochmal anlegen.
4. **Ein Auffälligkeiten-Bericht nach jedem Lauf.** Drei Stapel: erledigt, doppelt, bewusst liegen gelassen (mit Grund). Dazu Warnungen wie "Summe stimmt, Mehrwertsteuer nicht" oder "Rechnung an falsche Adresse".
5. **Das Programm setzt die Grenzen, nicht Claude.** lexoffice bleibt das führende Werkzeug. Claude liest, ordnet zu und meldet. Buchen, Umsatzsteuer-Voranmeldung und Absenden bleiben bei René in der lexoffice-Oberfläche.
6. **Erst prüfen, ob lexoffice es schon allein kann.** lexoffice liest Belege selbst aus (App, Upload, Beleg-E-Mail-Adresse) und schlägt beim Bankabgleich passende Belege vor. Vielleicht reicht das schon für 80 Prozent der Fälle. Claude dann nur für Sonderfälle und Auswertungen.
7. **Aufwand-Regler bewusst wählen.** Für Buchhaltung den Aufwand auf "Hoch" stellen, weil Fehler teuer sind und nicht sofort auffallen. Für E-Mails und Umformulieren reicht "Niedrig". Pro Aufgabe ein Modell wählen und im Chat nicht wechseln, sonst wird der ganze Verlauf nochmal teuer neu eingelesen.

## Was bei uns anders ist als bei den AInauten

- **lexoffice statt sevdesk.** Kein Wechsel nötig. Die Werbung im Newsletter (Rabattcode sevdesk) ignorieren.
- **Amazon-Auszahlungen.** Merch- und KDP-Tantiemen kommen teils in Dollar oder Pfund. Auch hier gilt Tipp 2: erst buchen, wenn der Euro-Betrag auf dem Konto ist.
- **Ausländische Anbieter.** Bei Rechnungen aus dem Ausland gelten oft Sonderregeln für die Umsatzsteuer. Das klärt der Steuerberater, nicht Claude. Am PC prüfen, was dazu schon im Vault steht.

## Vorschlag in drei Stufen (Empfehlung zuerst)

- **A (Empfehlung): Claude als Vorprüfer.** Claude liest den Belegordner und liefert eine Prüfliste (doppelt, Fremdwährung, Auffälligkeiten). René bucht selbst in lexoffice. Kein Zugriff von Claude auf lexoffice, kein Risiko.
- **B: Claude lädt Belege hoch.** Claude lädt geprüfte Belege per Schnittstelle (eine Art Steckdose, über die Claude direkt in lexoffice arbeiten kann) hoch. Gebucht wird weiter von René. Vorher klären, ob unser lexoffice-Tarif diese Schnittstelle enthält. Den Zugangsschlüssel legt René selbst an.
- **C: Claude bucht Entwürfe vor.** Erst sinnvoll, wenn A und B ein paar Monate sauber laufen.

## Abgleich heute Abend am PC (Prüfliste)

- [ ] `_AI-Bridge/CLAUDE.md` lesen: Was steht dort zu Buchhaltung, lexoffice, Belegen?
- [ ] Im Vault suchen nach: lexoffice, Lexware, Buchhaltung, Beleg, Steuer, Kleinunternehmer, Umsatzsteuer
- [ ] Skills im Vault prüfen (`03-Wissen/Skills/`): gibt es schon etwas zu Belegen oder Buchhaltung?
- [ ] Widersprüche zu den 7 Tipps notieren (der Vault gilt)
- [ ] Wo liegen die Belege heute? (Ordner, E-Mail, Google Drive)
- [ ] Entscheidung von René: A, B oder C
- [ ] Erst danach: Skill `belege-lexoffice` als Master im Vault anlegen (SOP-skill-ablage)

## Startsatz für die Sitzung am PC

> Lies `2026-10-08_buchhaltung-ainauten-abgleich.md` aus der Outbox, gleiche die 7 Tipps mit `_AI-Bridge/CLAUDE.md`, den Buchhaltungsnotizen und den Skills im Vault ab und zeig mir als Tabelle: Tipp, steht schon im Vault (ja/nein/Widerspruch), Vorschlag. Noch nichts ändern.
