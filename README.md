# Gemeinsame Agentenregeln

Dieses Repository bündelt allgemeine Arbeitsregeln und deren Übernahme in Projekte der Organisation.

| Datei | Zweck |
|---|---|
| [agents/BASELINE.md](agents/BASELINE.md) | Gemeinsame Mindestregeln, Version 1.0 |
| [docs/ADOPTION.md](docs/ADOPTION.md) | Projektlokale Übernahme und Versionsbindung |
| [AGENTS.md](AGENTS.md) | Arbeitsanweisungen für Änderungen an diesem Repository |

Die Dokumente erteilen keine technischen Berechtigungen und starten keine Agenten. Die Übernahme in Projekte erfolgt ausdrücklich und nachvollziehbar; sie wird nicht allein durch den Repositorynamen aktiviert.

Dieses Repository ist öffentlich. Es enthält allgemeine Regeln; kundenspezifische Informationen und interne Betriebsdetails werden im jeweiligen Projekt geführt.

Es sind in diesem Stand keine gemeinsamen Deployment-Workflows oder automatischen Richtlinien-Synchronisierungen eingerichtet.

## Rollenprofile

Die Vorlagen in [agents/](agents/) ergänzen die Baseline: planner, core-developer,
platform-developer, infra-developer, test-engineer und reviewer. Sie beschreiben
Aufgaben und erwartete Nachweise. Ein ausdrücklich eingerichteter Runner muss
Profile laden, Ausführungsgrenzen durchsetzen und technische Rechte begrenzen.
Andere Projekte installieren ihre Kopien ausdrücklich unter `.github/agents/`.
Die Profile sind keine gestarteten Dienste oder GitHub-Identitäten.
