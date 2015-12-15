# LaTeX-Vorlagen für die BA Glauchau

Ahoi. Du bist vermutlich hier gelandet, weil du nach "ba glauchau latex" o.ä. gegoogelt hast.
Ist dies tatsächlich der Fall, darf ich dich beglückwünschen - hier bist du genau richtig.

Im Rahmen des Praxisbelegs, den wir im zweiten Praxissemester anfertigen durften, habe ich die Chance genutzt
und mir LaTeX mal genauer angeschaut. Zu meiner Überraschung fand ich auch Vorlagen eines anderen
Student… pardon, Studierenden, welche mir jedoch nicht komplett gefallen haben, also habe ich kurzerhand
meine eigenen Vorlagen gebastelt, die soweit auch den Richtlinien entsprechen dürften.

Da ich meine Arbeit gern mit anderen teile, habe ich diese also einfach mal hier auf GitHub zur Verfügung
gestellt.

## Verwendung

Die verwendung sollte insgesamt recht einfach ausfallen:

1. `git clone https://github.com/ditti4/ba-gc-latex-vorlagen.git` oder wahlweise rechts in der Sidebar als ZIP herunterladen und entpacken
1. `reportsettings.tex` im Hauptverzeichnis öffnen und entsprechend anpassen
1. .tex-Hauptdatei anlegen und mit `\input{pre}` und `\input{post}` die beiden Loader-Dateien einbinden
1. Hauptdatei befüllen (zwischen den beiden `\input{}`-Anweisungen) und mit pdflatex kompilieren.
1. Über eine fertige PDF-Datei deiner wissenschaftlichen Arbeit freuen. Yay!

Wer ganz klug ist und seinen Beleg sowieso mit git tracken möchte, der legt sich für jeden Beleg einen neuen Branch an.
Wenn es hier dann mal Änderungen geben sollte, könnt ihr einfach wieder auf master-Branch wechseln, `git pull`
ausführen und eure Branches entsprechend mit`git checkout $branch` und `git rebase master` auf die aktuellsten
Änderungen hochziehen. Danach einfach wieder neu kompilieren, fertig. Zudem sollte die `.gitignore` eventuell den
eigenen Bedürfnissen angepasst werden (z.B. durch Entfernen des Eintrags für .bib-Dateien).

## Was fehlt? Was stimmt noch nicht?

Aktuell fehlt noch jegliche Verarbeitung von Tabellen und Beispielen, da ich diese selbst noch nicht eingesetzt
habe. Wenn sich damit jemand beschäftigen möchte, das möglichst nahe an den BA-Richtlinien umzusetzen, so möge dieser Jemand
doch bitte einen Pull request öffnen, damit ich weniger Arbeit damit habe (siehe auch [Mithelfen](#mithelfen)).

Zudem fehlt noch eine mehr oder weniger vernünftige Dokumentation aller Befehle, die die Vorlage hier bietet. Dafür soll,
wenn alles gut geht, bald™ mal das Wiki des Repositories genutzt werden, um alles möglichst zentral zu halten.

Außerdem, wobei ich nicht weiß, ob man das einfach mit LaTeX lösen kann, ist es aktuell auch noch so, dass mehrere Publikationen
von einem Autor, die im gleichen Jahr erschienen sind, *nicht* mit einem Index versehen werden, so wie es Punkt 3.3.3.5 eigentlich
vorschreibt (siehe Tabelle 6). Trifft exakt dieser Fall auf jemanden zu, so muss bitte beim Anlegen der Bibliographie darauf
geachtet werden, dass der Index selbst hinzugefügt wird.

## Mithelfen

Die Vorlagen sind unvollständig oder gar falsch? Unübersichtlich? Schlecht bedienbar? Die Einstellungen
könnte man einfacher vornehmen? Dann forke das Repository, fixe das, was gefixt werden muss und mach einen
Pull Request auf. Ich werde versuchen, mich innerhalb eines Tages darum zu kümmern.

Kleiner Hinweis dazu: Einrückung sollte mit 4 Leerzeichen erfolgen und öffnende geschweifte Klammern kommen
bitte ans Ende der Zeile (natürlich mit Leerzeichen davor), nicht auf eine neue. Commit messages sollten außerdem
in Englisch gehalten sein. Die Titelzeile eines Commits sollte auf 50 Zeichen begrenzt werden, der Body der
Commit-Message sollte mit einer freien Zeile auf die Titelzeile folgen und maximal 72 Zeichen pro Zeile enthalten.
