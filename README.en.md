<p align="center">
  <img src="https://omnipacto.de/assets/mark.svg" width="72" alt="">
</p>

<h1 align="center">Omnipacto</h1>

<p align="center">
  Contract management for families, individuals and small businesses –
  on your own server.<br>
  <a href="https://omnipacto.de/en/">omnipacto.de</a> ·
  <a href="https://demo.omnipacto.de">Live demo</a> ·
  <a href="README.md">Deutsch</a>
</p>

---

Omnipacto keeps your running contracts – insurance, electricity, gas, mobile plans,
subscriptions – in one place and **works out the last day you can cancel**, from the
minimum term, the renewal and the notice period. It reminds you in time, has the
cancellation letter ready, and shows what your household actually pays.

It runs on your own hardware. **No vendor account, no telemetry, no access to your bank
account** – even the licence check works without calling home.

<p align="center">
  <img src="https://omnipacto.de/assets/img/en/dashboard.webp" width="820" alt="Dashboard: running contracts, monthly total, next cancellation deadlines and costs by area">
</p>

## Install

```bash
curl -O https://omnipacto.de/docker-compose.yml
docker compose up -d
```

Then open **http://localhost:8000**. The setup wizard creates your first account and
household; Omnipacto generates keys and passwords itself. There is no configuration file
you need to touch first.

Your data lives in the `data/` folder next to the compose file – one folder, one backup.

### What you can add later

All inside the application under **Settings → Documents / Reminders**, each with a
"Test connection" button:

| | |
|---|---|
| **Paperless-ngx** | Link documents straight from your archive. Without an archive Omnipacto uses its own document store – nothing is missing. |
| **Ollama** | A language model on your network reads linked documents and proposes values, each with the passage it came from. Nothing is applied until you confirm it. |
| **Outgoing mail** | For e-mail reminders and password resets. |

## What it does

- **Cancellation deadlines**, calculated from the contract data – with a traffic light and a reminder
- **Cancelling as a process**: generate the letter, send it, confirm it
- **Price history** per contract, and the special right to cancel after a price increase
- **Costs** by area, line and year, plus the yearly total for your tax return
- **Documents** per contract with a role (policy, terms, amendment, invoice …)
- **Dates that are not cancellation deadlines**: inspections, boiler service, end of warranty
- **Coverage overview** per person and an **emergency dossier** as PDF
- **Calendar subscription** for iPhone, Google or Outlook, status endpoint for Home Assistant
- **Several people** per household with roles, several households per person
- German and English, chosen per person; installable like an app on a phone

<p align="center">
  <img src="https://omnipacto.de/assets/img/en/deadlines-full.webp" width="410" alt="Deadlines: what needs doing, every cancellation deadline and your own dates">
  <img src="https://omnipacto.de/assets/img/en/costs-full.webp" width="410" alt="Costs by area, line and year">
</p>

## Price

**Up to ten contracts free** – no time limit, no account, no payment details. This is not
a trial that expires.

Beyond that, a **one-off licence for €39**: unlimited contracts, server and desktop
edition, updates included, no subscription.
→ [omnipacto.de/en/buy.html](https://omnipacto.de/en/buy.html)

## Questions and bugs

Bug reports and requests as an **issue** here in the repository – that is the fastest way
to reach me. Otherwise by mail to info@omnipacto.de.

## Licence

Omnipacto is **not open-source software**. This repository holds the installation
instructions and the issue tracker, not the source code.
Terms: [omnipacto.de/bedingungen.html](https://omnipacto.de/bedingungen.html)
