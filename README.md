# Latex-Template für die DHAW
Dieses Repository enthält ein Latex-Template für Studienarbeiten an der Deutschen Hochschule für angewandte Wissenschaften. Das Template orientiert sich dabei an der von der Hochschule bereitgestellten Word-Vorlage, ist jedoch kein 1:1 Nachbau.

## Benutzung/Hinweise
Wir gehen davon aus, dass bereits ein Latex-Compiler installiert ist.
1. Klone das Repository: `git clone https://github.com/publicdesert/dhaw_latex_template`

2. Im Root-Verzeichnis liegt die Datei `./main.tex`. Hier kannst du einige grundlegende Metadaten setzen. Diese werden dann sowohl im Dokument als auch in die PDF-Metadaten übernommen.
```
\newcommand{\printAuthorName}{Max Mustermann}
\newcommand{\printAuthorMail}{max.mustermann@example.com}
\newcommand{\printDocumentTitle}{Titel meiner Studienarbeit}
\newcommand{\printDocumentSubject}{Mensch-Maschine-Interaktion}
\newcommand{\printCourseOfStudy}{Informatik}
\newcommand{\printDocumentDate}{\today}
```

3. Standardmäßig inkludiert `./main.tex` die Datei `./content/main.tex`, welche für den Inhalt der eigentlichen Arbeit vorgesehen ist. Diese ist mit ein wenig Platzhalterinhalt gefüllt. Diesen kannst du löschen und mit dem schreiben deiner Arbeit beginnen. Für größere Arbeiten bietet es sich an, die Kapitel in einzelne Dateien aufzuteilen. Dafür können in der `./main.tex` einfach die Includes angepasst werden.

4. Vom Template wird eine Bibtex-Datei unter `./literature/literature.tex` eingelesen. So können diverse Literaturverwaltungsprogramme wie etwa Zotero direkt verwendet werden.
5. Das Template verwendet römische Seitennummerierung für Verzeichnisse und Anhänge und arabische Nummerierung für den Kernteil. Aktuell muss nach der Rückkehr zur römischen Nummerierung der Counter für die Seitenzahlen manuell angepasst werden. Dies geschieht am Ende der `./main.tex`-Datei (`\setcounter{page}{5}`).
