Dockerisierte Latex-Bewerbungsvorlage inkl. Anschreiben
=====


Nutzung
-----

1. Bearbeiten und Befuellen von `anschreiben.tex` und `lebenslauf.tex` (in `src/main/resources`) mittels beliebigem Texteditor oder IDE.
2. Generierung der PDF durch Ausfuehrung von `lebenslauf.sh`/`anschreiben.sh`. 

Beispiele
-------

* [Anschreiben-Beispiel](src/main/resources/beispiele/anschreiben.pdf)
* [Lebenslauf-Beispiel](src/main/resources/beispiele/lebenslauf.pdf)

Technische Umsetzung
-------
Die Skripte starten einen Docker-Container [blang/latex](https://registry.hub.docker.com/u/blang/latex) mit einer Latex-Installation, mounten das aktuelle Verzeichnis mit den tex-Quelldateien und fuehren den entsprechenden Latex-Befehl aus. Das Resultat liegt dann neben den Quelldateien als PDF vor.  

Mehr Details zum Projekt auf dem ich hier aufsetze, findet man unter [https://www.blang.io/posts/2015-04_docker-tooling-latex/](https://www.blang.io/posts/2015-04_docker-tooling-latex/)

FYI Damit das Projekt einfacher in Java-IDEs geladen werden kann, besitzt das Projekt eine pom.xml.