# Open Data Lab – Datensatzdokumentation

## 1. Beschreibung der Datensätze

### Hauptdatensatz: FIFA World Cup Statistics
- **Titel:** FIFA World Cup 1930–2014  
- **Quelle:** [Kaggle – FIFA World Cup Dataset](https://www.kaggle.com/datasets/abecklas/fifa-world-cup)  
- **Format:** CSV-Datei  
- **Größe:** 20 Zeilen, 10 Spalten  
- **Wichtige Spalten:** Jahr, Gastgeberland, Gewinner, Zweiter, Dritter, Tore gesamt, Anzahl Teams, gespielte Spiele  
- **Lizenz:** *Kaggle Dataset License* (frei für nicht-kommerzielle Nutzung, Quelle muss angegeben werden)  

In der Datei stehen alle Weltmeisterschaften von 1930 bis 2014 mit den jeweiligen Ländern und Ergebnissen.  
Man sieht also pro Jahr, welches Land gewonnen hat, wo das Turnier stattfand und wie viele Tore insgesamt gefallen sind.  

---

### Zusatzdatensatz: World Population Dataset
- **Titel:** World Population by Country (1960–2023)  
- **Quelle:** [Kaggle – World Population Dataset](https://www.kaggle.com/datasets/iamsouravbanerjee/world-population-dataset)  
- **Format:** CSV-Datei  
- **Größe:** 234 Zeilen, 17 Spalten  
- **Wichtige Spalten:** Land, Kontinent, Bevölkerung (1970, 1980, 1990, 2000, 2010, 2020, 2022), Fläche, Dichte, Weltbevölkerungsanteil  
- **Lizenz:** *CC BY 4.0 License* (freie Nutzung unter Nennung der Quelle)

In dieser Datei ist für jedes Land angegeben, wie viele Einwohner es in verschiedenen Jahren hatte.  
Die letzte Spalte zeigt den Anteil an der Weltbevölkerung in Prozent (z. B. Afghanistan hat dort 0.52 %, nicht 52 %).  
Der Datensatz startet ab 1970, weshalb frühere Jahre (z. B. ältere Weltmeisterschaften) nicht direkt vergleichbar sind.  

---

## 2. Verbindung der Datensätze (Augmentation)

Ich habe die beiden Datensätze ausgewählt, weil sie sich gut miteinander verbinden lassen.  
In beiden steht jeweils ein Land, also kann man sie über den Ländernamen zusammenführen.  
Dadurch kann man zum Beispiel untersuchen, ob Länder mit einer größeren Bevölkerung im Durchschnitt erfolgreicher bei Fußball-Weltmeisterschaften sind.

### Idee für Forschungsfragen:
- Gibt es einen Zusammenhang zwischen der Bevölkerungsgröße eines Landes und seinem sportlichen Erfolg?  
- Haben Länder mit vielen Einwohnern häufiger den WM-Titel gewonnen?  
- Wie schneiden kleinere Länder im Vergleich ab (z. B. Kroatien, Uruguay)?  

### Nächste Schritte:
1. Ländernamen angleichen (z. B. „Germany“ vs. „Federal Republic of Germany“)  
2. Zeitraum auf 1970–2014 beschränken, da ab 1970 Populationsdaten vorhanden sind  
3. Datensätze zusammenführen (Merge über Land)  
4. Erste Auswertung (z. B. Häufigkeit von Titeln vs. Bevölkerung)  
5. Darstellung der Ergebnisse mit einer einfachen Grafik (z. B. Balkendiagramm oder Scatterplot)

---

## 3. FAIR-Bewertung

### FIFA World Cup Dataset
| Prinzip | Frage | Bewertung |
|----------|--------|-----------|
| **Findable (auffindbar)** | Lässt sich der Datensatz leicht finden und sind Metadaten vorhanden? | Ja, der Datensatz ist auf Kaggle öffentlich und über die Suche leicht zu finden. |
| **Accessible (zugänglich)** | Kann jeder die Daten herunterladen? | Ja, der Download ist ohne Anmeldung möglich. |
| **Interoperable (kompatibel)** | Liegt er in einem standardisierten, maschinenlesbaren Format vor? | Ja, als CSV-Datei. |
| **Reusable (wiederverwendbar)** | Ist die Lizenz klar und die Quelle angegeben? | Ja, über die Kaggle Dataset License. Es fehlen aber Hintergrundinfos zu den genauen Datenquellen (z. B. FIFA-Website). |

---

### World Population Dataset
| Prinzip | Frage | Bewertung |
|----------|--------|-----------|
| **Findable (auffindbar)** | Ist der Datensatz leicht zu finden? | Ja, über Kaggle öffentlich auffindbar, mit Beschreibung und Metadaten. |
| **Accessible (zugänglich)** | Kann man ihn ohne Barrieren herunterladen? | Ja, der Datensatz ist frei zugänglich. |
| **Interoperable (kompatibel)** | Wird ein gängiges Datenformat verwendet? | Ja, es handelt sich um CSV-Dateien mit klaren Spalten. |
| **Reusable (wiederverwendbar)** | Ist die Lizenz offen und die Dokumentation ausreichend? | Ja, CC BY 4.0 erlaubt Wiederverwendung mit Quellenangabe. Die Spalten sind klar dokumentiert. |

---

## 4. Reflexion

Ich finde die Kombination der beiden Datensätze ganz passend, weil sie sich thematisch leicht verknüpfen lässt und man mit wenig Aufwand interessante Fragen stellen kann.  
Was man aber beachten muss, ist, dass die Bevölkerungsdaten erst ab 1970 starten, während die Weltmeisterschaften schon 1930 beginnen.  
Für die Analyse würde ich mich deswegen nur auf den Zeitraum ab 1970 konzentrieren.  

Mir gefällt, dass beide Datensätze offen zugänglich und in einem verständlichen Format sind.  
Beide sind klein genug, um sie einfach mit Tools wie Python oder Excel zu analysieren, und gleichzeitig umfangreich genug, um sinnvolle Zusammenhänge zu finden.  
Insgesamt also eine gute Grundlage, um im nächsten Schritt eine kleine Datenpipeline aufzubauen und visuell auszuwerten.
