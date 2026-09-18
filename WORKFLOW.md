# GitHub-Workflow für App-Projekte

Dieser Ablauf ist eine Vorlage für die Zusammenarbeit an eigenen Apps und Kundenprojekten. Er wird pro Projekt an dessen Risiko, Tests und Freigaben angepasst.

## 1. Ein Repository pro eigenständigem Produkt

- Produktcode, technische Dokumentation und zugehörige Issues liegen zusammen.
- Wiederverwendbare Grundlagen bekommen nur dann ein eigenes Repository, wenn sie tatsächlich unabhängig gepflegt werden.
- Kundencode und interne Konfiguration bleiben privat. Öffentliche Demos enthalten ausschließlich dafür geeignete Inhalte.
- Eine neue Demo bekommt eine Preview-URL oder einen Unterordner im passenden Projekt. Tausende automatisch erzeugte Einzel-Repositories sind kein sinnvoller Standard.

## 2. Die Aufgabe beginnt mit einem Issue

Eine brauchbare Aufgabe beantwortet vier Fragen:

1. Welches konkrete Problem hat der Nutzer?
2. Was soll danach anders funktionieren?
3. Woran erkennen wir, dass es erledigt ist?
4. Welche Grenzen müssen erhalten bleiben?

Beispiel: „Nach dem Speichern eines Profils sehe ich die aktualisierten Daten auch nach einem Neuladen. Bei einem Speicherfehler bleibt meine Eingabe erhalten.“

## 3. Ein kleiner Branch, ein nachvollziehbarer Pull Request

- Branch aus dem aktuellen Hauptstand erstellen.
- Nur Änderungen für die konkrete Aufgabe aufnehmen.
- Pull Request mit dem Issue verknüpfen.
- Problem, geändertes Verhalten und tatsächliche Prüfungen kurz beschreiben.
- Bei sichtbaren Änderungen einen Screenshot oder eine kurze Demonstration ergänzen.

## 4. Prüfen, was sich wirklich geändert hat

- Passende bestehende Tests, Lint und Typecheck verwenden.
- Den wesentlichen Nutzerablauf und einen sinnvollen Fehlerfall prüfen.
- Bei UI-Änderungen die tatsächliche Oberfläche ansehen.
- Änderungen an Anmeldung, Berechtigungen, Zahlungen oder Daten gesondert prüfen.
- Keine Zugangsdaten oder Kundendaten in Issues, Screenshots, Logs oder Beispielkonfigurationen schreiben.

## 5. Review, Merge und Auslieferung gehören zusammen

- Mindestens ein fachlicher Gegencheck: Ist die Lösung richtig, und löst sie das richtige Problem?
- Erforderliche Prüfungen müssen erfolgreich sein.
- Pull Request mergen, anschließend die vorgesehene Zielumgebung prüfen.
- Das Issue erst schließen, wenn die vereinbarten Abschlusskriterien erfüllt sind.
- Ergebnis und offene Einschränkungen dokumentieren. Ein erfolgreicher Build allein beweist keinen funktionierenden Kundenablauf.

## Ein einfaches Project-Board

**Backlog → Bereit → In Arbeit → Review → Erledigt**

Eine Aufgabe hat einen Verantwortlichen, ein Repository und ein überprüfbares Ergebnis. Dringlichkeit, Aufwand und Projektbereich reichen als erste Zusatzfelder.

## Sinnvolle Labels

`bug` · `feature` · `design` · `docs` · `security` · `blocked`

Nur Labels hinzufügen, die Entscheidungen erleichtern. Zustände gehören ins Board; technische Details in das jeweilige Issue.

## Sichtbarkeit durch nützliche Arbeit

Ein öffentliches Projekt braucht eine verständliche README, ein reproduzierbares Beispiel, klare Voraussetzungen und eine passende Lizenz. Kleine Beiträge zu bereits genutzten Open-Source-Projekten, nachvollziehbare Releases und konkrete technische Erfahrungsberichte geben anderen einen Grund, wiederzukommen.
