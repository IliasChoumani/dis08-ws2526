# GenAI Documentation – Use of LLM (Lab 04: Version Control)

## 1. Eigene Umsetzung
Für dieses Lab habe ich den Großteil der Aufgaben selbstständig ausgeführt.  
Dazu gehörten unter anderem:

- Arbeiten mit Git auf der Kommandozeile (Branching, Merging, Committen, Pushen)
- Durchführen der einzelnen Shell-Aufgaben in `get_info.sh`
- Erstellen der Dateien `bio.md` und `facts.md`
- Lösen des Merge-Konflikts in der Datei `bio.md`
- Verständnis des Git-Workflows zwischen lokalem Repository und GitHub

Ich habe bewusst versucht, jeden Schritt selbst auszuführen, um besser zu verstehen, wie Git in der Praxis funktioniert. Vor allem das Wechseln zwischen Branches, das manuelle Bearbeiten von Konflikten und das stufenweise Committen der Shell-Aufgaben habe ich eigenständig durchgeführt.

## 2. Unterstützung durch ein LLM
Ich habe ChatGPT (Modell: GPT‑5.1, Stand November 2025) als unterstützendes Werkzeug verwendet, um bestimmte Schritte besser zu verstehen.  
Dabei ging es vor allem um:

- Erklärungen zu Git-Konzepten (Branches, Merge, Konflikte)
- Hinweise zur korrekten Reihenfolge der Git-Befehle
- Unterstützung bei der Fehlersuche (z. B. Konflikte, Push-Probleme)
- Strukturierung des Workflows, damit die Aufgabenstellung sauber erfüllt wird
- Teilweise Erstellung von Textbausteinen für Markdown-Dateien (z. B. *conflict-resolution.md*)

Die inhaltlichen Entscheidungen und die tatsächliche Ausführung der Befehle habe ich jedoch selbst vorgenommen.

### Beispiel-Prompts
Einige typische Prompts, die ich verwendet habe:

- „Kannst du mir Schritt für Schritt erklären, wie ich einen neuen Branch erstelle?“  
- „Warum kommt bei `git push` dieser Fehler? Was bedeutet das?“  
- „Kannst du mir eine konfliktfreie Beispielversion von `bio.md` geben?“  
- „Ich brauche eine Markdown-Datei für die Konfliktdokumentation – kannst du mir eine Vorlage machen?“

ChatGPT hat mir dabei geholfen, die Abläufe besser zu verstehen und Fehler zu vermeiden, aber **die Git-Befehle, die Konfliktlösung und das Arbeiten im Repository habe ich aktiv selbst gemacht**.

## 3. Vergleich & Reflexion
Viele Vorschläge des Modells habe ich angepasst oder vereinfacht.  
Ich habe häufig den generierten Text gekürzt oder umformuliert, damit er zu meinem eigenen Stil passt.

Beispiele:

- Die *conflict-resolution.md* wurde von ChatGPT vorgeschlagen, aber ich habe selbst entschieden, wie sie inhaltlich eingebunden wird.
- Bei Shell-Befehlen habe ich verstanden, was passiert, bevor ich sie ausgeführt habe.
- Merge-Konflikte habe ich selbst in der Datei gelöst und danach committen müssen — das konnte das Modell nicht übernehmen.

Der größte Unterschied zwischen meinen eigenen Formulierungen und den LLM-Vorschlägen war der Stil:

- Das LLM schreibt tendenziell formeller.
- Ich habe vieles umformuliert, damit es natürlicher klingt.


## 4. Fazit
Das LLM war hilfreich, um:

- Git besser zu verstehen,
- Fehler schneller zu identifizieren,
- und sicherzustellen, dass die Aufgabenstellung vollständig erfüllt wurde.

Es hat jedoch keinen automatisierten Code ausgeführt – alle Git-Schritte, Konfliktlösungen und Uploads habe **ich selbst** durchgeführt.

Die finale Lösung ist eine Mischung aus eigener Arbeit und punktueller Unterstützung durch das LLM.
