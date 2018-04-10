Dockerisierte Latex-Bewerbungsvorlage inkl. Anschreiben
=====


Nutzung
-----

1. Bearbeiten und Befuellen von `anschreiben.tex` und `lebenslauf.tex` (in `src/main/resources`) mittels beliebigen Texteditor/IDE.
2. Generierung durch Ausfuehrung `lebenslauf.sh`/`anschreiben.sh`. 

Beispiele
-------

* [Anschreiben-Beispiel](src/main/resources/beispiele/anschreiben.pdf)
* [Lebenslauf-Beispiel](src/main/resources/beispiele/lebenslauf.pdf)

Technische Umsetzung
-------
Die Skripte starten einen Docker-Container [blang/latex](https://registry.hub.docker.com/u/blang/latex) mit einer Latex-Installation, mounten das aktuelle Verzeichnis mit den Quelldateien und fuehren den endsprechende Latex-Befehl aus. Das Resultat liegt dann neben den Quelldateien als PDF vor.  

Mehr Details zu dem Projekt auf dem ich hier aufsetze, findet man unter [https://www.blang.io/posts/2015-04_docker-tooling-latex/](https://www.blang.io/posts/2015-04_docker-tooling-latex/)

FYI Damit das Projekt einfacher in Java-IDEs geladen werden kann, besitzt das Projekt eine pom.xml.