# Projekttitel:  
**Marktwert und Gesamtleistung der Spieler**

## Fragestellung:  
**Gibt es einen Zusammenhang zwischen dem Marktwert eines Spielers und seiner Gesamtleistung (z. B. Tackles, Passgenauigkeit, Ballgewinne) in der Champions League?**

---

## Mit welchen Daten arbeiten wir?  
Wir nutzen die **UCL 2021/22 Datenbank** von Kaggle, die Informationen zu Matches und Spielern enthält. Die Daten umfassen:

- Spieler- und Mannschaftsstatistiken  
- Tore und deren Eigenschaften (z. B. wie geschossen: rechts, links, Kopfball etc.)  
- Spielinformationen wie Datum, Ergebnisse und Events  
- Webscraping: Transfermarkt | Marktwerte der ersten 4 Teams in der UCL-Saison:
  - Manchester City
  - Real Madrid
  - Liverpool FC
  - Villarreal CF

### Erklärung:  
Die Leistung eines Spielers in einem Fußballturnier wie der UEFA Champions League lässt sich durch eine Vielzahl von Kennzahlen messen. Dazu gehören sowohl offensive als auch defensive Beiträge, z. B. Tore, Assists, aber auch Tackles, Ballgewinne, Passgenauigkeit, Schüsse und viele andere Aspekte. Der Marktwert eines Spielers ist ein Indikator für seinen geschätzten Wert auf dem Transfermarkt und kann durch Faktoren wie Leistung, Alter, Potenzial und Bekanntheitsgrad beeinflusst werden.  

Diese Fragestellung zielt darauf ab, zu untersuchen, ob Spieler mit einem höheren Marktwert tatsächlich auch bessere Gesamtleistungen zeigen, gemessen an ihren individuellen Statistiken, oder ob es keinen merklichen Zusammenhang gibt.

---

## Wie wir vorgegangen sind:  

1. **Datenextraktion und Scraping**  
   - Websites von Transfermarkt werden genutzt, um Informationen über die Marktwerte von Spielern verschiedener Top-Teams zu sammeln.
   - Gescrapte Daten werden in einer CSV-Datei gespeichert.

2. **Datenbereinigung**  
   - Unvollständige Daten (z. B. Spieler ohne Marktwert) werden entfernt.
   - Marktwerte werden in ein einheitliches Format konvertiert (Millionen oder Tausend).
   - Spaltennamen und Texte werden normalisiert.
   - Zusätzliche Spalten wie Vornamen der Spieler werden extrahiert und hinzugefügt.

3. **Datenzusammenführung**  
   - Die gescrapten Daten werden mit zusätzlichen Datensätzen (z. B. Key Stats, Defending, Distribution) kombiniert.
   - Übereinstimmungen zwischen Spielernamen und Teams aus verschiedenen CSV-Dateien werden durch textbasierte Algorithmen hergestellt.

4. **Analyse**  
   - Verschiedene Analysen werden durchgeführt:
     - Marktwert im Zusammenhang mit gespielten Minuten, Toren und Assists (Korrelation und Regression).
     - Defensivleistungen (erholte Bälle, Tacklings, gewonnene Duelle) bei Verteidigern.
     - Passgenauigkeit im Zusammenhang mit Marktwert.
   - Ergebnisse werden visualisiert und durch Scatterplots mit Regressionslinien dargestellt.
   - Lineare Regressionsmodelle werden erstellt und interpretiert.

5. **Ergebnisse speichern**  
   - Die bereinigten und analysierten Daten werden in neuen CSV-Dateien abgelegt.

---

## Das sind unsere Daten:  

- **Datensatz:** [UCL 2021/22 Matches & Players](https://www.kaggle.com/datasets/azminetoushikwasi/ucl-202122-uefa-champions-league)
- **Webscraping-Quellen:**  
  - Real Madrid: [Link](https://www.transfermarkt.de/real-madrid/kader/verein/418/saison_id/2021)
  - Liverpool FC: [Link](https://www.transfermarkt.de/fc-liverpool/kader/verein/31/saison_id/2021)
  - Manchester City: [Link](https://www.transfermarkt.de/manchester-city/kader/verein/281/saison_id/2021)
  - Villarreal CF: [Link](https://www.transfermarkt.de/fc-villarreal/kader/verein/1050/saison_id/2021)

- **Ergebnis:** Datenvisualisierung und klare Erkenntnisse
- **Präsentation** [Link](https://thkoelnde-my.sharepoint.com/:p:/g/personal/mrosiny_th-koeln_de/EZwC1jO8PtRNlr2NK8hGJfsBzEDhViqX6qnzBj29aSVOAw?rtime=ivKDQrI73Ug)

---

## Teilnehmer in der Gruppe  
- Ben Gebhardt  
- Mogens Rosiny  
- Lennard Michel  
- Tolga Ipek  
- Can Bakirci  
- Robin Klinkhammer  

---

