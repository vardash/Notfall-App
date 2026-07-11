Notfall-App

«Eine diskrete, zuverlässige und datenschutzfreundliche Notfall-App für Android.»

Projektziel

Die Notfall-App soll Menschen in Gefahrensituationen dabei unterstützen, unauffällig Hilfe anzufordern, ohne das Smartphone sichtbar bedienen zu müssen.

Die Anwendung wird speziell für Stresssituationen entwickelt und folgt dem Grundsatz:

«So einfach wie möglich – so zuverlässig wie nötig.»

---

Leitprinzipien

Die Entwicklung orientiert sich an vier Grundprinzipien:

- 🛡️ Einfachheit – Unter Stress muss die Bedienung intuitiv sein.
- 🤫 Diskretion – Der Alarm soll möglichst unauffällig ausgelöst werden.
- ✅ Zuverlässigkeit – Die Kernfunktionen müssen jederzeit funktionieren.
- 🔒 Datenschutz – Alle sensiblen Daten bleiben ausschließlich auf dem Gerät.

---

Hauptfunktionen

- Diskrete Notfallauslösung über die Lautstärketasten
- Sicherheits-Countdown mit Abbruchmöglichkeit
- SMS-Versand an Notfallkontakte
- Optionale Standortübermittlung
- Optionaler Fake-Anruf als Ausstiegshilfe
- Lokale Speicherung aller Daten
- Offline-fähig

---

Technologie

Komponente| Technologie
Programmiersprache| Dart
Framework| Flutter
UI| Flutter (optional FlutterFlow zur UI-Erstellung)
Datenbank| SQLite

---

Zielplattformen

Aktuell

- Android

Geplant

- Wear OS

Zukunft

- iOS / Apple Watch (separates Konzept erforderlich)

---

Architektur

Die Anwendung basiert auf einer modularen Architektur.

App
 │
 ▼
Bootstrapper
 │
 ├── Capability Scanner
 ├── Core
 ├── Module Manager
 │
 ├── Trigger
 ├── SMS
 ├── Standort
 ├── Fake Call
 ├── Logging
 ├── Notification
 └── weitere Module

Der Bootstrapper erkennt die Plattform und die verfügbaren Gerätefähigkeiten und lädt anschließend automatisch die benötigten Module.

---

Dokumentation

Die technische Dokumentation befindet sich im Ordner docs/.

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

---

Projektstatus

Aktuelle Version: Master-Konzept 1.1

Der Schwerpunkt liegt derzeit auf der Konzeption und Entwicklung einer stabilen Android-Version mit modularer Architektur und zuverlässiger Notfallauslösung.

---

Entwicklungsphilosophie

Dieses Projekt verfolgt den Grundsatz:

«Eine Codebasis – viele Geräte.»

Die Geschäftslogik wird vollständig in Dart entwickelt.

Plattformabhängige Funktionen werden über klar definierte Schnittstellen gekapselt, sodass zukünftige Erweiterungen (z. B. Wear OS) mit möglichst geringem Aufwand integriert werden können.

Neue Funktionen werden nur aufgenommen, wenn sie die vier Leitprinzipien Einfachheit, Diskretion, Zuverlässigkeit und Datenschutz unterstützen.

---

Lizenz

Die Lizenz wird im weiteren Projektverlauf festgelegt. 
