<p align="center">
  <img src="https://omnipacto.de/assets/mark.svg" width="72" alt="">
</p>

<h1 align="center">Omnipacto</h1>

<p align="center">
  Vertragsverwaltung für Familien, Privatpersonen und kleine Unternehmen –
  auf deinem eigenen Server.<br>
  <a href="https://omnipacto.de">omnipacto.de</a> ·
  <a href="https://demo.omnipacto.de">Demo ansehen</a>
</p>

---

Omnipacto sammelt deine laufenden Verträge – Versicherungen, Strom, Gas, Mobilfunk,
Abonnements – an einem Ort und **rechnet den letzten Kündigungstag selbst aus**, aus
Laufzeit, Verlängerung und Kündigungsfrist. Es erinnert dich rechtzeitig, legt das
Kündigungsschreiben fertig vor und zeigt, was dein Haushalt tatsächlich zahlt.

Es läuft auf deiner eigenen Hardware. **Kein Konto beim Hersteller, keine Telemetrie,
kein Zugriff auf dein Bankkonto** – auch die Lizenzprüfung kommt ohne Verbindung nach
außen aus.

## Installieren

```bash
curl -O https://omnipacto.de/docker-compose.yml
docker compose up -d
```

Dann **http://localhost:8000** im Browser öffnen. Der Assistent legt dein erstes Konto
und deinen Haushalt an; Schlüssel und Passwörter erzeugt Omnipacto selbst. Es gibt keine
Konfigurationsdatei, die du vorher anfassen müsstest.

Deine Daten liegen im Ordner `data/` neben der Compose-Datei – ein Ordner, eine Sicherung.

### Was danach optional dazukommt

Alles in der Anwendung unter **Einstellungen → Instanz**, jeweils mit einem Knopf
„Verbindung prüfen":

| | |
|---|---|
| **Paperless-ngx** | Dokumente direkt aus deinem Archiv verknüpfen. Ohne Archiv nutzt Omnipacto seinen eigenen Dokumentenspeicher – es fehlt nichts. |
| **Ollama** | Ein Sprachmodell in deinem Netz liest verknüpfte Dokumente und schlägt Werte vor, jeder mit Fundstelle. Übernommen wird nur, was du bestätigst. |
| **Mailversand** | Für Erinnerungen per E-Mail und das Zurücksetzen von Passwörtern. |

## Was es kann

- **Kündigungsfristen**, aus den Vertragsdaten berechnet – mit Ampel und Erinnerung
- **Kündigen als Vorgang**: Schreiben erzeugen, verschicken, bestätigen
- **Preisverlauf** je Vertrag und das Sonderkündigungsrecht nach einer Preiserhöhung
- **Kosten** nach Bereich, Sparte und Jahr, dazu die Jahressumme für die Steuer
- **Dokumente** je Vertrag mit Rolle (Police, Bedingungen, Nachtrag, Rechnung …)
- **Termine**, die kein Kündigungstag sind: HU, Heizungswartung, Garantieende
- **Absicherungsübersicht** je Person und ein **Notfalldossier** als PDF
- **Kalender-Abo** für iPhone, Google oder Outlook, Status-Aufruf für Home Assistant
- **Mehrere Personen** je Haushalt mit Rollen, mehrere Haushalte je Person
- Deutsch und Englisch, je Person wählbar; auf dem Smartphone wie eine App installierbar

## Preis

**Bis zu zehn Verträge kostenlos** – ohne Zeitlimit, ohne Konto, ohne Zahlungsdaten. Das
ist keine Testphase, die abläuft.

Wer mehr verwaltet, kauft **einmalig eine Lizenz für 39 €**: unbegrenzt viele Verträge,
Server- und Desktop-Fassung, Updates inklusive, kein Abonnement.
→ [omnipacto.de/kaufen.html](https://omnipacto.de/kaufen.html)

## Fragen und Fehler

Fehlerberichte und Wünsche bitte als **Issue** hier im Repository – das ist der
schnellste Weg zu mir. Sonst per Mail an info@omnipacto.de.

## Lizenz

Omnipacto ist **keine Open-Source-Software**. Dieses Repository enthält die
Installationsanleitung und den Fehler-Tracker, nicht den Quellcode.
Bedingungen: [omnipacto.de/bedingungen.html](https://omnipacto.de/bedingungen.html)
