---
datum: 2026-10-08
quellen: AInauten Newsletter Februar 2026 (sevdesk + Claude) und 08.10.2026 (Buchhaltung mit AI, Teil 1 + Kosten und Aufwand)
status: Entwurf, Abgleich mit dem Vault steht noch aus
ablage-vorschlag: 01-Business/Buchhaltung/ (am PC prüfen, ob es dort schon eine passende Notiz gibt)
---

# Buchhaltung mit Claude: Was wir aus zwei AInauten-Newslettern für lexoffice mitnehmen

Hinweis: lexoffice heißt inzwischen offiziell "Lexware Office". Gemeint ist dasselbe Programm.

## Die Entwicklung in einem Satz

Im Februar hieß es noch: Claude erfasst und bucht alles selbst. Im Oktober sind die AInauten vorsichtiger: Claude bereitet vor, der Mensch prüft und bucht, Fremdwährung bleibt liegen. Wir übernehmen die vorsichtigere Oktober-Fassung.

## Die 11 Tipps, übersetzt auf lexoffice

**Aus dem Oktober-Newsletter**

1. **Ein fester Befehl für den Belege-Lauf.** Bei uns gibt es dafür noch keinen Skill (die Haushaltsabrechnung ist nur privat). Vorschlag: Skill `belege-lexoffice`.
2. **Nie selbst Währungen umrechnen.** Belege in Dollar (Midjourney, Ideogram, Canva, Domains, Amazon-Tantiemen in Dollar oder Pfund) bleiben liegen, bis der echte Euro-Betrag auf dem Konto oder der Kreditkarte steht.
3. **Doppelte Belege aussortieren.** Rechnungsnummer, Betrag und Datum schon vorhanden? Dann nicht nochmal anlegen.
4. **Auffälligkeiten-Bericht nach jedem Lauf.** Drei Stapel: erledigt, doppelt, bewusst liegen gelassen (mit Grund). Dazu Warnungen wie "Summe stimmt, Mehrwertsteuer nicht".
5. **lexoffice setzt die Grenzen, nicht Claude.** Buchen, Umsatzsteuer-Voranmeldung und Absenden bleiben bei René in der lexoffice-Oberfläche.
6. **Erst prüfen, was lexoffice allein kann.** lexoffice liest Belege selbst aus (App, Upload, Beleg-E-Mail-Adresse) und schlägt beim Bankabgleich passende Belege vor. Vielleicht reicht das für die meisten Fälle.
7. **Aufwand-Regler bewusst wählen.** Buchhaltung auf "Hoch", E-Mails auf "Niedrig". Pro Aufgabe ein Modell, im Chat nicht wechseln.

**Zusätzlich aus dem Februar-Newsletter**

8. **Regelwerk für Claude schriftlich festhalten.** Welche Konten, welche Kategorien, welche Sonderfälle. Bei uns gehört das in den Vault (`_AI-Bridge/CLAUDE.md` oder eine eigene Buchhaltungsnotiz), nicht in einen losen Projektordner.
9. **Zweite KI prüft die ersten Durchläufe.** Die AInauten nehmen Gemini. Bei uns ginge das per `/gemini`. Vorsicht: Belege enthalten persönliche Daten. Alternative: die lokale KI (LM Studio), die schon bei der Haushaltsabrechnung Bons ausliest.
10. **Erst einmal von Hand sauber durchspielen, dann Skill daraus machen.** Passt zu unserer SOP-skill-ablage.
11. **Auswertungen fragen.** "Wie hoch ist der Gewinn bisher?", "Wofür geben wir am meisten aus?" Das ändert nichts in der Buchhaltung und ist ein guter, risikoloser Einstieg (mit einer Export-Datei aus lexoffice).

## Wo wir bewusst anders handeln

- **Zugangsschlüssel nie in den Chat.** Die AInauten geben Claude den Schlüssel einfach im Gespräch. Bei uns gilt: Zugangsdaten legt René selbst an und hinterlegt sie selbst. Claude fordert sie nicht an.
- **lexoffice statt sevdesk.** Kein Wechsel. Rabattcodes in beiden Newslettern ignorieren (der Februar-Code ist ohnehin abgelaufen).
- **Rechnungen schreiben lassen** ist für uns vermutlich unwichtig, weil Amazon per Gutschrift auszahlt. Am PC prüfen.
- **Umsatzsteuer bei ausländischen Anbietern** klärt der Steuerberater, nicht Claude.

## Vorschlag in drei Stufen (Empfehlung zuerst)

- **A (Empfehlung): Claude als Vorprüfer.** Claude liest den Belegordner und liefert die Prüfliste (doppelt, Fremdwährung, Auffälligkeiten). René bucht selbst in lexoffice. Dazu Auswertungen aus einer Export-Datei. Kein Zugriff von Claude auf lexoffice.
- **B: Claude lädt Belege hoch.** Über die Schnittstelle (eine Art Steckdose, über die Claude direkt in lexoffice arbeiten kann). Gebucht wird weiter von René. Vorher klären, ob unser lexoffice-Tarif diese Schnittstelle enthält.
- **C: Claude bucht Entwürfe vor.** Erst, wenn A und B ein paar Monate sauber laufen.

## Was René tun soll

1. Heute Abend am PC: diese Datei in die Outbox legen und den Startsatz unten in eine neue Sitzung kopieren.
2. Nach dem Abgleich entscheiden: A, B oder C.
3. Festlegen, wo die Belege künftig gesammelt werden (ein Ordner für alles).
4. Nur bei B oder C: im lexoffice-Tarif nachsehen, ob die Schnittstelle dabei ist. Keine Kosten ohne Rückfrage.

## Prüfliste für den Abgleich am PC

- [ ] `_AI-Bridge/CLAUDE.md` lesen: Was steht dort zu Buchhaltung, lexoffice, Belegen, Zugangsdaten?
- [ ] Im Vault suchen nach: lexoffice, Lexware, Buchhaltung, Beleg, Steuer, Kleinunternehmer, Umsatzsteuer
- [ ] Skills im Vault prüfen (`03-Wissen/Skills/`): gibt es schon etwas zu Belegen oder Buchhaltung?
- [ ] Widersprüche zu den 11 Tipps notieren (der Vault gilt)
- [ ] Erst nach Renés Entscheidung: Skill `belege-lexoffice` als Master im Vault anlegen

## Startsatz für die Sitzung am PC

> Lies `2026-10-08_buchhaltung-ainauten-abgleich.md` aus der Outbox, gleiche die 11 Tipps mit `_AI-Bridge/CLAUDE.md`, den Buchhaltungsnotizen und den Skills im Vault ab und zeig mir als Tabelle: Tipp, steht schon im Vault (ja/nein/Widerspruch), Vorschlag. Noch nichts ändern.
