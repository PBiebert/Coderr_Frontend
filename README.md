# Coderr Frontend Project

![Coderr Logo](assets/logo/logo_coderr.svg)

Coderr ist das Frontend für eine Freelancer-Plattform. Das Backend wird separat
mit Django umgesetzt. Ziel des Projekts ist es, Frontend und Backend sauber zu
verbinden, damit die Plattform vollständig funktioniert.

---

## Voraussetzungen

- Ein laufendes Django-Backend für Coderr, das die API bereitstellt.
- Visual Studio Code mit der Live-Server-Erweiterung oder eine ähnliche
    Möglichkeit, die `index.html` lokal im Browser zu starten.

---

## Schnellstart

1. Stelle sicher, dass das Backend läuft.
2. Öffne dieses Frontend-Projekt in Visual Studio Code.
3. Starte die oberste `index.html` mit Live Server.
4. Registriere dich als Kunde oder Anbieter oder melde dich mit einem Gastzugang an.

> In der App gibt es vorbereitete Gast-Logins für zwei Rollen: Kunde und Anbieter.

---

## Ziel des Projekts

Dieses Frontend wurde bewusst mit Vanilla JavaScript erstellt, damit die
Integration mit dem Django-Backend möglichst direkt und nachvollziehbar bleibt.

- **Registrierung und Login**: Nutzer können sich als Kunde oder Anbieter anmelden.
- **Angebote verwalten**: Angebote lassen sich mit verschiedenen Varianten erstellen.
- **Aufträge abbilden**: Aus Angeboten können Aufträge erstellt, abgelehnt und im Status angepasst werden.
- **Filter und Auswertungen**: Listen und Statistiken zeigen wichtige Kennzahlen wie Anbieter, Aufträge und mehr.
- **Bewertungen**: Kunden können Anbieter bewerten.
- **Einfacher Einstieg**: Ohne Frameworks bleibt der Code leicht lesbar und schnell anpassbar.

---

## Features

| Bereich | Funktion |
|---|---|
| **Auth** | Login, Registrierung als Kunde oder Anbieter, Gastlogin, Token-Authentifizierung |
| **Profile** | Kunden- und Anbieter-Profile anzeigen und bearbeiten |
| **Angebote** | Angebote mit Varianten erstellen, auflisten und Details anzeigen |
| **Aufträge** | Aufträge aus Angeboten erstellen, ablehnen, Status ändern und filtern |
| **Statistiken** | Kennzahlen wie Anbieter, Aufträge und Statusübersichten anzeigen |
| **Bewertungen** | Kunden können Anbieter bewerten |

---

## API-Anbindung

Die API-URLs sind in `shared/scripts/config.js` definiert. Dort sind unter anderem
die Endpunkte für Login, Registrierung, Profile, Angebote, Aufträge, Bewertungen,
Filter und Statistiken hinterlegt.

Die Authentifizierung erfolgt über Token, die im Frontend gespeichert und bei
API-Requests verwendet werden.

---

## Architektur & Konventionen

- **Kein Build-Step** - die Dateien werden direkt vom Browser geladen.
- **Shared JS/CSS** - wiederverwendbare Module liegen in `shared/`.
- **Template-Funktionen** - HTML-Strukturen werden per JavaScript erzeugt.
- **localStorage** - Token und Nutzerinfos werden nach dem Login gespeichert.
- **Rollenbasiert** - Kunden und Anbieter arbeiten mit unterschiedlichen Ansichten und Funktionen.

---

## Hinweis

Dieses Projekt ist ausschliesslich für Schüler der Developer Akademie gedacht
und nicht zur freien Nutzung oder Weitergabe freigegeben.

---

## JSDoc ansehen

1. Navigiere in den Ordner `docs/`.
2. Öffne das Projekt mit Doppelklick auf `docs/index.html` oder im Terminal:
     - Windows: `start docs/index.html`
     - macOS: `open docs/index.html`
     - Linux: `xdg-open docs/index.html`
