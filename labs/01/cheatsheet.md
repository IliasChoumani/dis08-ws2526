# 📝 Markdown Cheatsheet  
**Erstellt von:** Ilias Choumani  
**Kurs:** DIS08 – Data Modeling  
**Aufgabe:** 1 – Open Source Software and Hosting  
**Datum:** 19. Oktober 2025  

---

> **Hinweis:**  
> Dieses Cheatsheet wurde im Rahmen der Aufgabe *Open Source Software and Hosting* erstellt.  
> Es erklärt die wichtigsten Funktionen von **Markdown** in klarer, leicht verständlicher Form – mit Beispielen, Erklärungen und dem sichtbaren Ergebnis.

---

## 1. Grundlegende Formatierungen

### 1.1 Überschriften
Mit `#` werden Überschriften erstellt.  
Je mehr `#`, desto kleiner ist die Überschrift.

**Markdown-Code:**
```markdown
# Überschrift 1
## Überschrift 2
### Überschrift 3
```
**Ergebnis:**
# Überschrift 1
## Überschrift 2
### Überschrift 3

---

### 1.2 Absätze & Zeilenumbrüche
Absätze werden durch eine Leerzeile getrennt.  
Für einen manuellen Zeilenumbruch füge zwei Leerzeichen am Ende einer Zeile hinzu.

**Markdown-Code:**
```markdown
Das ist ein Absatz.

Das ist ein neuer Absatz.  
Hier ist ein Zeilenumbruch.
```
**Ergebnis:**
Das ist ein Absatz.

Das ist ein neuer Absatz.  
Hier ist ein Zeilenumbruch.

---

### 1.3 Fett
**Markdown-Code:**
```markdown
**Fetter Text**
__Auch fetter Text__
```
**Ergebnis:**  
**Fetter Text**  
__Auch fetter Text__

---

### 1.4 Kursiv
**Markdown-Code:**
```markdown
*Kursiver Text*
_Kursiver Text_
```
**Ergebnis:**  
*Kursiver Text*  
_Kursiver Text_

---

### 1.5 Fett + Kursiv
**Markdown-Code:**
```markdown
***Fett und kursiv***
```
**Ergebnis:**  
***Fett und kursiv***

---

### 1.6 Durchgestrichen
**Markdown-Code:**
```markdown
~~Durchgestrichen~~
```
**Ergebnis:**  
~~Durchgestrichen~~

---

### 1.7 Inline-Code
Inline-Code wird genutzt, wenn du **einzelne Befehle oder Codewörter innerhalb eines Satzes hervorheben** möchtest.  
Der Code wird zwischen zwei **Backticks** (`) geschrieben.

**Markdown-Code:**
```markdown
Um Text in Python auszugeben, benutzt man den Befehl `print()`.
```
**Ergebnis:**  
Um Text in Python auszugeben, benutzt man den Befehl `print()`.

💡 **Erklärung:**  
Alles, was zwischen den Backticks steht, erscheint in einer Schreibmaschinenschrift (Monospace) und wird nicht weiter formatiert.  
Das ist ideal, um kurze Codeausschnitte wie `for`, `if`, `SELECT * FROM users;` oder `echo "Hallo"` zu zeigen.

---

## 2. Listen

### 2.1 Ungeordnete Listen
**Markdown-Code:**
```markdown
- Punkt 1
- Punkt 2
  - Unterpunkt 2.1
```
**Ergebnis:**
- Punkt 1
- Punkt 2
  - Unterpunkt 2.1

---

### 2.2 Geordnete Listen
**Markdown-Code:**
```markdown
1. Erster Punkt
2. Zweiter Punkt
3. Dritter Punkt
```
**Ergebnis:**
1. Erster Punkt
2. Zweiter Punkt
3. Dritter Punkt

---

### 2.3 Verschachtelte Listen
**Markdown-Code:**
```markdown
1. Punkt 1
   - Unterpunkt 1.1
   - Unterpunkt 1.2
2. Punkt 2
```
**Ergebnis:**
1. Punkt 1
   - Unterpunkt 1.1
   - Unterpunkt 1.2
2. Punkt 2

---

## 3. Links & Bilder

### 3.1 Inline-Links
**Markdown-Code:**
```markdown
[OpenAI](https://www.openai.com)
```
**Ergebnis:**  
[OpenAI](https://www.openai.com)

---

### 3.2 Referenz-Links
**Markdown-Code:**
```markdown
[GitHub][1]

[1]: https://github.com
```
**Ergebnis:**  
[GitHub][1]

[1]: https://github.com

---

### 3.3 Bilder
**Markdown-Code:**
```markdown
![Markdown Logo](https://markdown-here.com/img/icon256.png)
```
**Ergebnis:**  
![Markdown Logo](https://markdown-here.com/img/icon256.png)

---

### 3.4 Bild + Link Kombination
**Markdown-Code:**
```markdown
[![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)](https://github.com)
```
**Ergebnis:**  
[![GitHub Logo](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)](https://github.com)

---

## 4. Code & Technischer Inhalt

Dieser Bereich ist besonders wichtig für Entwickler:innen, die Code in Markdown dokumentieren wollen.  
Es gibt **drei Hauptarten**, Code darzustellen:

### 4.1 Inline-Code (einzeilig)
Für **kurze Codewörter innerhalb eines Satzes**.  
Beispiel: „Der Befehl `print()` gibt Text auf dem Bildschirm aus.“

---

### 4.2 Codeblöcke (mehrzeilig)
Wenn du **mehrere Zeilen Code** zeigen willst, nutzt du **drei Backticks (` ``` )** oben und unten um den Codeblock.

**Markdown-Code:**
```markdown
```
print("Hallo Welt!")
x = 10
print(x * 2)
```
```
**Ergebnis:**
```
print("Hallo Welt!")
x = 10
print(x * 2)
```

💡 **Tipp:** Codeblöcke werden automatisch in einer Monospace-Schrift dargestellt, behalten Einrückungen und Zeilen bei.

---

### 4.3 Syntax Highlighting
Wenn du nach den Backticks eine **Programmiersprache** angibst (z. B. `python`, `html`, `bash`), wird der Code farblich hervorgehoben.

**Markdown-Code:**
```markdown
```python
def begruessung(name):
    print(f"Hallo {name}!")

begruessung("Ilias")
```
```
**Ergebnis (mit Syntax-Highlighting):**
```python
def begruessung(name):
    print(f"Hallo {name}!")

begruessung("Ilias")
```

---

## 5. Zitate & Hinweise

Mit dem Zeichen `>` kann man Zitate, Notizen oder Kommentare einfügen.  
Das ist praktisch für **Hinweise, Erklärungen oder wichtige Informationen**.

### 5.1 Einfaches Zitat
**Markdown-Code:**
```markdown
> Markdown ist eine einfache Auszeichnungssprache.
```
**Ergebnis:**  
> Markdown ist eine einfache Auszeichnungssprache.

---

### 5.2 Verschachtelte Zitate
**Markdown-Code:**
```markdown
> Ebene 1
>> Ebene 2
```
**Ergebnis:**
> Ebene 1
>> Ebene 2

---

### 5.3 Formatierte Hinweise
Du kannst in Zitaten auch **fetten, kursiven Text oder Emojis** nutzen, um wichtige Infos hervorzuheben.

**Markdown-Code:**
```markdown
> 💡 **Tipp:** Markdown ist ideal für Dokumentationen auf GitHub!
```
**Ergebnis:**  
> 💡 **Tipp:** Markdown ist ideal für Dokumentationen auf GitHub!

---

## 6. Tabellen

### 6.1 Einfache Tabellen
**Markdown-Code:**
```markdown
| Name  | Alter |
|-------|-------|
| Ilias | 22    |
```
**Ergebnis:**
| Name  | Alter |
|-------|-------|
| Ilias | 22    |

---

### 6.2 Ausrichtung
**Markdown-Code:**
```markdown
| Links | Mitte | Rechts |
|:------|:-----:|-------:|
| a     | b     | c      |
```
**Ergebnis:**
| Links | Mitte | Rechts |
|:------|:-----:|-------:|
| a     | b     | c      |

---

### 6.3 Komplexe Tabellen
**Markdown-Code:**
```markdown
| Produkt | Beschreibung     | Preis |
|----------|------------------|------:|
| 🍎 Apfel | Frischer Apfel   | 1,20€ |
| 🍌 Banane| Reife Banane     | 0,80€ |
```
**Ergebnis:**
| Produkt | Beschreibung     | Preis |
|----------|------------------|------:|
| 🍎 Apfel | Frischer Apfel   | 1,20€ |
| 🍌 Banane| Reife Banane     | 0,80€ |

---

## 7. Aufgabenlisten (Checkboxen)

**Markdown-Code:**
```markdown
- [x] Markdown gelernt
- [ ] Datei auf GitHub hochladen
```
**Ergebnis:**
- [x] Markdown gelernt
- [ ] Datei auf GitHub hochladen

---

## 8. Trennlinien & Layout

### 8.1 Horizontale Linie
Verwende `---`, `***` oder `___`.

**Markdown-Code:**
```markdown
---
```
**Ergebnis:**
---

---

## 9. Online-Editoren

Beispiele für Online-Editoren zum Schreiben von Markdown:
- [Dillinger](https://dillinger.io)
- [StackEdit](https://stackedit.io)
- [Typora](https://typora.io)

---

## 10. GitHub-spezifische Funktionen

### 10.1 Aufgabenlisten
GitHub macht Checkboxen anklickbar.

**Ergebnis:**
- [x] Beispiel erledigt
- [ ] Noch offen

---

### 10.2 Benutzer erwähnen
**Markdown-Code:**
```markdown
@benutzername
```
**Ergebnis:**  
@benutzername

---

### 10.3 Automatische Verlinkungen
**Markdown-Code:**
```markdown
Fixes #12
```
**Ergebnis:**  
Fixes #12

---

### 10.4 Emojis
**Markdown-Code:**
```markdown
:smile: :rocket: :tada:
```
**Ergebnis:**  
:smile: :rocket: :tada:

---

✅ **Ende des Markdown Cheatsheets**
