[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-2e0aaae1b6195c2367325f4f02e2d04e9abb55f0b24a779b69b11b9e10269abc.svg)](https://classroom.github.com/online_ide?assignment_repo_id=22125845&assignment_repo_type=AssignmentRepo)
# Javscript einfach lernen

In diesem Projekt werden wir eine Reihe von Aufgaben mit Javascript lösen. Bei diesen Aufgaben geht es darum eine Intuition für die Syntax von Javascript aufzubauen, so wie die Grundkonzepte des Programmierens zu erlernen. Wir werden Bedinungen und Schleifen anschauen in diesem Projekt.

## Organisation

Jede Aufgabe wird in einer eigenen Datei bearbeitet. Diese Dateien sind jeweils nach der Aufgabe benannt. Für jede neue Aufgabe muss eine neue Datei erstellt werden. Alle diese Dateien müssen im folgenden Verzeichnis liegen: `src/exercises`.

## Programm ausführen

Um eine Aufgabe auszuführen, müssen wir diese über das Terminal starten. Am besten öffnen Sie ein neues Terminal, und geben dann den folgenden Befehl ein:

```bash
node src/exercises/ex-01.js
```

Dann wird die Aufgabe 1 ausgeführt.

### Trick um weniger zu Tippen

Wenn Sie nicht immer den ganzen Pfad eintippen möchten, dann können Sie im Terminal das Verzeichnis wechseln. Das machen Sie mit dem `cd` Befehl (`cd` steht für `Change Directory`). Der Befehl würde dann also so aussehen:

```bash
cd src/exercises
```

Dann können Sie die Datei direkt starten, also mit dem folgenden Befehl:

```bash
node ex-01.js
```

### Eingaben an das Programm machen

Oftmals möchte man das ein Programm auf unterschiedliche Art funktioniert, jenachdem wie das Programm aufgerufen wird. Die einfachste Art das zu erreichen, ist mit sogenannten **Kommandozeilen Argumenten**. Das sind zusätzliche Argumente die wir bei starten des Programms über die Kommandozeile eingeben. **Achtung**: Diese Argumente werden mit Leerzeichen getrennt!

```bash
node ex-01.js Argument1 Argument2
```

Hier werden 2 Argumente übergeben, und das Programm kann nun auf diese Argumente reagieren.

## Debuggen oder Fehler beheben

Beim Programmieren ist es völlig normal das man nicht direkt zur richtigen Lösung kommt. Sehr oft ist es auch einfach ausprobieren und verbessern, und manchmal hat man einen Überlegungsfehler gemacht, und muss diesen dann in der Logik des Programms suchen. Damit dies möglichst einfach geht, gibt es den sogennanten **Debugger**. Das ist ein Hilfsprogramm, das Ihnen den aktuellen Zustand des Programms anzeigt, und welche Variablen welche Werte haben. Sie können das Programm auch mittendrin stoppen, sich alles anschauen, sogar Werte ändern, und dann weiter laufen lassen. So können Fehler schnell gefunden und behoben werden.

Das arbeiten mit dem **Debugger** hilft auch eine bessere Intuition für ein solches Programm zu bekommen, da es Ihnen erlaubt das Programm an jeder Stelle zu stoppen. So können Sie den Ablauf des Programms nachvollziehen, und das ganze besser verstehen.

Um das Programm im **Debug-Modus** zu öffnen, müssen Sie nur den Befehl nur ganz leicht abändern, zu:

```bash
node --inspect ex-01.js
```

## Versionen und Änderungen

Immer wenn Sie eine Änderung machen, sollten Sie eine neue Version machen. Das ist nicht jedesmal wenn Sie speichern, aber immer dann, wenn Sie denken Sie haben Fortschritt in der Aufgabe gemacht. Der Vorteil für Sie ist, dass Sie dann die Änderungen einfach anschauen können, und man kann diese auch "leicht" Rückgängig machen, zumindest bis zur letzten Version, oder mann kann sich dann eine noch ältere Version holen.

Das anschauen der Versionen soll Ihnen helfen, den Code besser lesen und verstehen zu können, und Änderungen schnell und einfach lesen können. Gerade wenn Sie mit LLMs arbeiten werden, ist es wichtig zu sehen wo das LLM Ihren Code verändert hat, nur so können Sie sicher sein, das ein LLM keine Änderungen vornimmt die Sie nicht möchten.

Neue Versionen machen Sie über Commits, so wie Sie das bereits kennen. Wichtig ist, das Sie sich die Änderungen vor dem Commit jeweils anschauen.

## Aufgaben

Ein paar Einstiegsaufgaben finden Sie [hier](Aufgaben.md), weitere Aufagben werden später noch folgen.