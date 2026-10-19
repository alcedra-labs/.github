# Zentrale Regeln in Projekten verwenden

Dieses Repository hält allgemeine Agentenregeln bereit. Ihre Verwendung in einem Projekt wird ausdrücklich eingerichtet und versioniert.

## Repository und Verzeichnis unterscheiden

| Ort | Bedeutung |
|---|---|
| Organisations-Repository .github | Gemeinsame Dokumente und Vorlagen |
| AGENTS.md im Zielprojekt | Lokale Arbeitsanweisungen für unterstützende Coding-Agenten |
| Verzeichnis .github/workflows im Zielprojekt | Dort ausdrücklich eingerichtete GitHub-Actions-Workflows |
| Ein Link auf eine zentrale Richtlinie | Verweis auf eine Quelle; kein universeller Mechanismus zum Laden dieser Datei |

GitHub übernimmt bestimmte unterstützte Community-Dateien aus dem öffentlichen .github-Repository. Daraus folgt keine automatische Übernahme beliebiger Agentendateien oder Workflows. Für Agentenhinweise sieht das offene AGENTS.md-Format projektlokale Dateien vor; der verwendete Agent muss dieses Format tatsächlich unterstützen.

## Vorgeschlagener Übernahmeweg

1. Eine geprüfte Version der Datei agents/BASELINE.md auswählen.
2. Den vollständigen Quellcommit dokumentieren.
3. Die benötigten Mindestregeln in einer AGENTS.md im Zielprojekt hinterlegen und dort um projektspezifische Hinweise ergänzen.
4. Den Quellcommit verlinken. Ein Verweis auf einen beweglichen Branch ersetzt die festgelegte Version nicht.
5. In einem neuen Arbeitslauf prüfen, dass der verwendete Agent die lokale Datei erkennt und beachtet.
6. Änderungen der zentralen Baseline über einen eigenen Projekt-PR übernehmen.

Eine zentrale Änderung wirkt damit erst nach bewusster Übernahme in ein Projekt. Ein reiner URL-Verweis garantiert nicht, dass ein Agent die entfernte Datei liest. Die lokale Datei muss die zum Arbeiten erforderlichen Regeln enthalten.

Eine spätere Synchronisierung kann diese Übernahme automatisieren und einen überprüfbaren PR erzeugen. In diesem Dokumentationsstand ist kein Synchronisierungsworkflow eingerichtet.

## Grenzen

Die Regeln beschreiben Zusammenarbeit und Qualitätsanforderungen. Konten, Cloudrollen, Repositoryrechte, Agenteninstallationen und Betriebsfreigaben werden technisch separat eingerichtet.

Öffentliche Regeln enthalten allgemeine Arbeitsweisen. Projektspezifische Architekturen, Kostenrechnungen und interne Betriebsdaten werden im dafür vorgesehenen Projekt dokumentiert.

## Quellen

- [GitHub: Unterstützte gemeinsame Community-Dateien](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file)
- [AGENTS.md: Format und projektlokale Verwendung](https://agents.md/)
