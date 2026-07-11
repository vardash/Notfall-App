# Notfall-App

> Eine diskrete, zuverlässige und datenschutzfreundliche Notfall-App für Android.

---

## Projektziel

Die **Notfall-App** soll Menschen in Gefahrensituationen dabei unterstützen, unauffällig Hilfe anzufordern, ohne das Smartphone sichtbar bedienen zu müssen.

Die Anwendung wird speziell für Stresssituationen entwickelt und folgt dem Grundsatz:

> **So einfach wie möglich – so zuverlässig wie nötig.**

---

# Leitprinzipien

Die Entwicklung orientiert sich an vier unveränderlichen Grundprinzipien.

- 🛡️ **Einfachheit**  
  Unter Stress muss die Bedienung intuitiv und leicht merkbar sein.

- 🤫 **Diskretion**  
  Die Notfallauslösung erfolgt möglichst unauffällig.

- ✅ **Zuverlässigkeit**  
  Die Kernfunktionen müssen jederzeit funktionieren.

- 🔒 **Datenschutz**  
  Alle sensiblen Daten verbleiben ausschließlich auf dem Gerät.

---

# Hauptfunktionen

- Diskrete Notfallauslösung über die Lautstärketasten
- Sicherheits-Countdown mit Abbruchmöglichkeit
- SMS an Notfallkontakte
- Optionale Standortübermittlung
- Optionaler Fake-Anruf als soziale Ausstiegshilfe
- Lokale Datenspeicherung
- Offline-Betrieb

---

# Technologie

| Komponente | Technologie |
|------------|-------------|
| Framework | Flutter |
| Programmiersprache | Dart |
| Datenbank | SQLite |
| UI | Flutter (optional FlutterFlow als UI-Designer) |

---

# Zielplattformen

## Aktuell

- Android

## Geplant

- Wear OS

## Zukunft

- iOS / Apple Watch (separates Konzept)

---

# Architektur

Die Anwendung basiert auf einer modularen Architektur.

```text
App
 │
 ▼
Bootstrapper
 │
 ├── Capability Scanner
 ├── Config Manager
 ├── Core
 ├── Module Manager
 │
 ├── Trigger
 ├── SMS
 ├── Standort
 ├── Fake Call
 ├── Notification
 ├── Logging
 └── weitere Module
```

Der Bootstrapper erkennt die Plattform sowie die technischen Fähigkeiten des Geräts und initialisiert anschließend nur die benötigten Module.

Dadurch folgt die Anwendung dem Grundsatz:

> **Eine Codebasis – viele Geräte**

---

# Trigger

Die Standardauslösung erfolgt über:

- **3× Volume Down innerhalb von 3 Sekunden**

Alternativ kann **Volume Up** gewählt werden.

Es werden bewusst **keine frei konfigurierbaren Tastenkombinationen** unterstützt.

Unter Stress soll sich der Nutzer nur **eine einzige Aktion merken müssen**.

---

# Datenschutz

Die Notfall-App arbeitet vollständig lokal.

- Keine Cloud
- Keine Server
- Keine Benutzerkonten
- Keine Telemetrie
- Keine Analyse

Standortdaten werden ausschließlich für den Notfall verwendet.

---

# Dokumentation

Die Projektdokumentation befindet sich im Verzeichnis `docs/`.

Geplante Dokumente:

```text
docs/
├── master-concept.md
├── architecture.md
├── bootstrapper.md
├── modules.md
├── trigger.md
├── fake-call.md
├── privacy.md
├── roadmap.md
└── changelog.md
```

---

# Projektstatus

## Aktuelle Konzeptversion

**Master-Konzept Version 1.1**

Der Schwerpunkt liegt aktuell auf der Architekturplanung und der Entwicklung einer stabilen Android-Version.

---

# Entwicklungsphilosophie

Die Notfall-App soll nicht möglichst viele Funktionen besitzen.

Sie soll Menschen in einer Ausnahmesituation schnell, diskret und zuverlässig helfen.

Neue Funktionen werden nur aufgenommen, wenn sie die vier Grundprinzipien

- Einfachheit
- Diskretion
- Zuverlässigkeit
- Datenschutz

unterstützen und die Bedienung nicht unnötig erschweren.

---

# Roadmap

## Version 1

- Android
- SMS
- Standort
- Trigger
- Fake-Anruf
- Testmodus

## Spätere Versionen

- Wear OS
- mehrere Notfallkontakte
- SMS-Wiederholung
- Check-in-Funktion
- Geofencing
- Import / Export
- Barrierefreiheit

---

# Lizenz

Die Lizenz wird im weiteren Projektverlauf festgelegt.
