# Open Data Lab – Datensatzdokumentation

## 1. Datensatzbeschreibung

### Titel & Quelle
**Hauptdatensatz:** FIFA World Cup Statistics (1930–2014)  
**Quelle:** [Kaggle – FIFA World Cup 1930–2014 Dataset](https://www.kaggle.com/datasets/abecklas/fifa-world-cup)  

**Zusatzdatensatz:** World Population by Country  
**Quelle:** [Kaggle – World Population Dataset (1960–2023)](https://www.kaggle.com/datasets/iamsouravbanerjee/world-population-dataset)  

---

### Dateiformate
Beide Datensätze liegen im **CSV-Format** vor und sind **UTF-8-kodiert**.  
Sie können problemlos mit Programmen wie Excel, Python (pandas) oder R geöffnet werden.

---

### Größe & Struktur
| Datensatz | Zeilen | Spalten | Dateigröße |
|------------|---------|----------|-------------|
| WorldCups.csv | 20 | 10 | ca. 4 KB |
| world_population.csv | 234 | 17 | ca. 45 KB |

**Beispielhafte Spalten im WorldCups-Datensatz:**
`Year`, `Country`, `Winner`, `Runners-Up`, `GoalsScored`, `MatchesPlayed`, `Attendance`

**Beispielhafte Spalten im Population-Datensatz:**
`Country/Territory`, `Continent`, `1970 Population`, `2022 Population`, `Area (km²)`, `Growth Rate`

---

### Grundlegende Statistiken
**WorldCups.csv**  
- Zeitraum: 1930 – 2014  
- Durchschnittliche Anzahl an Toren pro Turnier: **≈ 119 Tore**  
- Minimum: **70 Tore** (1930), Maximum: **171 Tore** (1998)  
- Anzahl der Turniere: **20**

**world_population.csv**  
- Zeitraum (abgedeckt durch Spalten): **1970 – 2022**  
- Durchschnittliche Bevölkerungszahl (2022): ca. **33 Mio. pro Land**  
- Min: **≈ 10 000**, Max: **1,4 Mrd.**  
- Enthält über 230 Länder mit historischen Bevölkerungswerten.

---

### Räumliche und zeitliche Abdeckung
- **WorldCups:** Weltweite Turniere von 1930 bis 2014  
- **Population:** Bevölkerungsentwicklung pro Land von 1970 bis 2022  
- Gemeinsamer sinnvoller Analysezeitraum: **1970–2014**, da ab 1970 verlässliche Bevölkerungsdaten vorhanden sind.

---

### Lizenz
Beide Datensätze stehen unter einer **offenen Lizenz (CC BY 4.0 / Open Data License)** und dürfen für nicht-kommerzielle, wissenschaftliche Zwecke frei verwendet, analysiert und weiterverarbeitet werden.

---

## 2. Datensatz-Erweiterung (Augmentation)

### Zweiter Datensatz & Verbindung
Der zweite Datensatz („World Population“) kann direkt über die Spalte **Land / Country** mit dem FIFA-Datensatz verknüpft werden.  
Dadurch kann analysiert werden, **ob Länder mit einer größeren Bevölkerung tendenziell erfolgreicher bei Fußball-Weltmeisterschaften sind.**

---

### Mögliche Forschungsfragen
- Haben Länder mit mehr Einwohnern häufiger den Weltmeistertitel gewonnen?  
- Gibt es eine Korrelation zwischen Bevölkerungsgröße und WM-Erfolg (z. B. Platzierung oder Teilnahmen)?  
- Wie haben sich kleinere Länder (z. B. Kroatien, Uruguay) im Verhältnis zu großen Nationen entwickelt?  
- Welche Kontinente stellen überdurchschnittlich erfolgreiche Teams im Verhältnis zur Bevölkerungsgröße?

---

### Nächste Schritte zur Verknüpfung
1. **Standardisierung der Ländernamen** (z. B. „Germany“ ↔ „Federal Republic of Germany“)  
2. **Einschränkung auf Jahre ab 1970** (da Bevölkerungsdaten erst dann verfügbar sind)  
3. **Merging der Datensätze** anhand der Länderspalte  
4. **Berechnung neuer Kennzahlen**, z. B. durchschnittliche Bevölkerung pro Titel oder pro Finalteilnahme  
5. **Visualisierung** (Scatterplot: Bevölkerung vs. Titelanzahl, Heatmap nach Kontinenten)

---

## 3. FAIR-Bewertung

| Prinzip | Frage | Bewertung |
|----------|--------|------------|
| **Findable (Auffindbar)** | Sind die Datensätze leicht zu finden und mit Metadaten versehen? | ✅ Ja, beide sind auf Kaggle gut dokumentiert und über Suchmaschinen auffindbar. |
| **Accessible (Zugänglich)** | Können die Daten frei heruntergeladen werden? | ✅ Ja, beide sind öffentlich ohne Login zugänglich. |
| **Interoperable (Kompatibel)** | Liegen sie in standardisierten, maschinenlesbaren Formaten vor? | ✅ Ja, CSV ist universell nutzbar. |
| **Reusable (Wiederverwendbar)** | Ist die Lizenz eindeutig und die Dokumentation ausreichend? | ⚠️ Teilweise: Die Population-Datei enthält gute Metadaten, die FIFA-Daten weniger Kontext zu Quellen. Beide aber grundsätzlich offen und wiederverwendbar. |

---

## 4. Reflexion

Die Arbeit mit offenen Datensätzen wie diesen zeigt gut, wie unterschiedlich Datenquellen in Umfang und Struktur sein können.  
Während der FIFA-Datensatz kompakt und klar strukturiert ist, liefert der Bevölkerungsdatensatz viele zusätzliche Variablen und Zeitdimensionen.  
Eine kleine Einschränkung besteht darin, dass die Bevölkerungsdaten erst ab 1970 beginnen, sodass frühere Weltmeisterschaften nicht direkt vergleichbar sind.  
Trotzdem bietet der kombinierte Datensatz eine gute Grundlage, um statistische Zusammenhänge zwischen Bevölkerung und sportlichem Erfolg zu untersuchen.  
Besonders spannend ist dabei die Erkenntnis, dass auch kleinere Länder mit weniger Einwohnern überdurchschnittliche Leistungen erzielen können.  

Insgesamt sind beide Datensätze **gut zugänglich, offen lizenziert** und lassen sich **einfach kombinieren**, was sie zu einem idealen Beispiel für Open-Data-Arbeiten macht.

---
