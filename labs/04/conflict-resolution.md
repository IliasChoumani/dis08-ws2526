# Conflict Resolution: bio.md

## Ausgangssituation
Während der Bearbeitung von Lab 04 wurden zwei Branches verwendet, die beide Änderungen an derselben Datei `bio.md` vorgenommen haben:

- **Branch `main`** enthielt eine Version mit der Überschrift **"About Me"**, ergänzt um Details über mein Studium an der TH Köln.
- **Branch `feature-facts`** enthielt eine alternative Version mit der Überschrift **"Biography"**, inhaltlich anders formuliert.

Beim Versuch, den Branch `feature-facts` in `main` zu mergen, erkannte Git, dass beide Branches denselben Teil der Datei verändert hatten. Dadurch entstand ein **klassischer Merge-Konflikt**.

## Art des Konflikts
Git fügte in `bio.md` typische Konflikt-Markierungen ein:

```
<<<<<<< HEAD
... Version von main ...
=======
... Version von feature-facts ...
>>>>>>> feature-facts
```

Das zeigt, dass Git die Änderungen nicht automatisch zusammenführen konnte, weil sich beide Branches an identischen Zeilen unterschieden.

## Vorgehen zur Konfliktlösung
Ich habe den Konflikt manuell gelöst:

1. Beide Versionen der `bio.md` verglichen.
2. Eine **neue, kombinierte Version** der Biografie erstellt, die Inhalte aus beiden Varianten sinnvoll zusammenführt.
3. Alle Konflikt-Markierungen  
   (`<<<<<<<`, `=======`, `>>>>>>>`)  
   manuell entfernt.
4. Die bereinigte, finale Version gespeichert.

Anschließend habe ich Git mit folgenden Befehlen informiert, dass der Konflikt gelöst wurde:

```
git add bio.md
git commit -m "Resolve merge conflict in bio.md between main and feature-facts"
```

## Ergebnis
- Der Merge-Konflikt wurde erfolgreich gelöst.
- `feature-facts` konnte vollständig in `main` gemergt werden.
- Die Datei `bio.md` enthält jetzt eine zusammengeführte, konsistente Version.
- Der gesamte Konflikt ist nun sowohl im Commitverlauf als auch in dieser Datei dokumentiert.
