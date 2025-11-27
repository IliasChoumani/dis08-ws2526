# GenAI Documentation – Use of LLM (Lab 05: Web Scraping & Data Analysis)

## 1. Eigene Umsetzung
Für dieses Lab habe ich den Großteil der Aufgaben selbstständig umgesetzt.  
Dazu gehörten u. a.:

- Verständnis der Aufgabenstellung (Scraping aller NHL-Daten über 24 Seiten)
- Erstellen des Jupyter-Notebooks `nhl.ipynb`
- Ableiten einer geeigneten Lösung für die Pagination
- Schreiben der Funktionen für:
  - das Generieren aller Seiten-URLs,
  - das Scrapen einer einzelnen Seite,
  - das Zusammenführen aller Datensätze
- Aufbau der DataFrame-Struktur und Konvertieren der Spalten in die richtigen Datentypen
- Speichern der vollständigen Daten als `data.csv`
- Durchführung der beiden Analysen (Teams mit den meisten Wins; Anzahl der Teams pro Jahr)
- Kontrolle der Ergebnisse durch stichprobenartiges Vergleichen mit der Originalseite

Ich habe dabei bewusst versucht, den kompletten Workflow vom Abruf der HTML-Seiten über die Extraktion der Tabellen bis zur finalen Analyse nachzuvollziehen. Viele Schritte, wie z. B. die Entwicklung der Schleife, das Debuggen kleiner Fehler und das Prüfen der Zwischenergebnisse, habe ich aktiv selbst durchgeführt.

## 2. Unterstützung durch ein LLM
Ich habe ChatGPT (Modell: GPT-5.1, Stand November 2025) als unterstützendes Werkzeug genutzt, vor allem um:

- das Vorgehen beim Web Scraping besser zu verstehen,
- HTML-Strukturen und CSS-Selektoren zu interpretieren,
- zu prüfen, ob mein Ansatz zur Pagination technisch sinnvoll ist,
- Code-Strukturen klarer und robuster aufzubauen,
- Zwischenergebnisse zu validieren (z. B. Abgleich der `data.csv` mit realen Tabelleneinträgen),
- Hilfestellung beim Aufbau der Analysefunktionen in pandas zu bekommen.

Die konkrete Implementierung im Notebook, das Testen einzelner Funktionen und das Durchführen der vollständigen Scraping-Runde habe ich selbst ausgeführt.  
Das LLM hat mir vor allem dabei geholfen, Fehler schneller zu identifizieren und den Code sauber zu strukturieren, ohne mir die komplette Aufgabe abzunehmen.

### Beispiel-Prompts
Einige der Prompts, die ich verwendet habe, waren:

- „Wie erkenne ich, dass ich wirklich alle Seiten gescraped habe?“  
- „Warum wird in Jupyter eine Ausgabe angezeigt, obwohl ich kein `print` benutzt habe?“  
- „Kannst du mir helfen, die Tabelle auf Seite 9 testweise auszulesen?“  
- „Wie sollte ich die numerischen Spalten in pandas konvertieren?“  


Das Modell hat mir geholfen, einzelne Schritte klarer zu verstehen, aber **die Ausführung des Codes, das Debugging und der finale Aufbau des Notebooks waren meine Arbeit**.

## 3. Vergleich & Reflexion
Viele generierte Vorschläge habe ich angepasst oder umformuliert, damit sie in mein Notebook und meinen Stil passen.  
Einige Punkte, bei denen ich bewusst selbst entschieden habe:

- Ich habe entschieden, die Pagination über eine Schleife von 1 bis 24 zu lösen, weil das für diese Aufgabe am praktischsten ist.
- Die Tests für Seite 1 und Seite 9 habe ich bewusst eingefügt, um sicherzustellen, dass die Scraping-Funktion korrekt arbeitet.
- Die DataFrame-Analysen (Max-Wins und Team-Anzahl) habe ich so aufgebaut, dass sie möglichst klar und nachvollziehbar sind.
- Die Struktur der Notebook-Zellen (Scraping → CSV → Analyse) habe ich selbst bestimmt.

Das LLM hat oft formellere oder komplexere Lösungen vorgeschlagen, die ich dann vereinfacht habe, damit sie besser zur Aufgabenstellung passen.

## 4. Fazit
Das LLM war hilfreich für:

- schnelles Verstehen von HTML-Strukturen,
- das korrekte Anwenden von BeautifulSoup-Selektoren,
- das Strukturieren der Scraping-Logik,
- und das Validieren meiner Zwischenergebnisse.

Es hat jedoch keinen Code ausgeführt und die zentrale technische Umsetzung — Scraping, CSV-Erstellung und Analyse der `data.csv` — habe **ich selbst** im Notebook umgesetzt.

Die finale Lösung ist eine Mischung aus eigener Arbeit und punktueller Unterstützung durch das LLM, vergleichbar mit einer Zweitmeinung oder einem Tutor, der beim Verständnis hilft.
