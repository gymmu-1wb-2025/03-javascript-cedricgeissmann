# Aufgaben

Hier ist eine Sammlung von Einstiegsaufgaben.

## Aufgabe 01

Schreiben Sie ein Programm, welches Sie mit Ihrem Namen begrüsst.

- Der Name soll in der Variable `name` gespeichert werden.
- Der Name wird als **Kommandozeilen-Argument** an das Programm übergeben.
- Erstellen Sie einen **Breakpoint** in der Zeile mit dem `console.log(...)`, und verändern Sie den Wert der Variable `name`.
- Starten Sie das Programm mit dem Befehl `node --inspect ex-01.js`
- Erstellen Sie einen Commit.

## Aufgabe 02

Schreiben Sie ein Programm, welches Sie mit Ihrem Name und Ihrem Alter begrüsst.

- Der Name soll in der Variable `myname` gespeichert werden.
- Das Alter wird in der Variable `myage` gespeichert.
- Beide werden als **Kommandozeilen-Argumente** an das Programm übergeben.
- Nutzen Sie den **Debug-Modus** falls nötig.
- Erstellen Sie mehrere Commits.

## Aufgabe 03

Schreiben Sie ein Programm, welches Sie mit Namen und Alter begrüsst. Das Programm sagt Ihnen ausserdem wie alt Sie an der Matur sein werden (aktuelles Alter plus 4, muss nicht genau stimmen, hier geht es nur darum eine einfache Rechnung zu haben).

- Das Programm nimmt nur genau 2 **Kommandozeilen-Argumente** entgegen, und zwar Name und Alter.
- Das Alter an der Matur soll abhängig vom aktuellen Alter berechnet werden.
- Starten Sie das Programm im **Debug-Modus** und erstellen Sie einen Breakpoint direkt vor der Addition `age + 4`. Welchen Typ hat die Variable `age`?
- Verwenden Sie die Funktion `Number(...)` um eine Variable in eine Zahl zu verwandeln.
- Erstellen Sie einen Kommentar an dieser Stelle im Code, wieso Sie diese Funktion `Number(...)` brauchen.

## Aufgabe 04

Schreiben Sie ein Programm, welches den BMI ausrechnet.

- Das Programm bekommt genau 2 **Kommandozeilen-Argumente**.
- Der BMI berechnet sich mit der folgenden Formel: $\frac{g}{h^2}$, wobei $g=$ Gewicht in kg und $h=$ Körpergrösse in cm.
- Erstellen Sie bei jeder Änderung einen Commit.

## Aufgabe 05

Schreiben Sie ein Programm, welches Ihnen eine Talentvorhersage für Volleyball macht.

- Sie geben dem Programm Ihre Körpergrösse in cm als einziges **Kommandozeilen-Argument** an.
- Berechnen Sie den Talent-Wert mit der folgenden Formel: `243 - bodyHeight`; oder für Frauen: `224 - bodyHeight`.
- Das Programm soll dann jeweils unterschiedlich antworten, je nach `talentScore`:
    - Wenn `talentScore < 50` dann sagt das Programm, `"Du hast sehr viel Potenzial"`
    - Wenn `50 <= talentScore && talentScore < 60` dann sagt das Programm, `"Du musst dringend an deiner Spungkraft arbeiten."`
    - Wenn `60 <= talentScore && talentScore < 70` dann sagt das Programm, `"Wenn du schnell bist, kannst du dir die Libero-Position überlegen."`
    - Wenn `70 <= talenScore` dann sagt das Programm, `Du wirst im Volleyball nicht glücklich werden."`

## Aufgabe 06

Schreiben Sie ein Programm, das Ihnen sagt, ob eine Zahl durch 3 Teilbar ist oder nicht.

- Das Programm nimmt nur eine Zahl über die Kommandozeile entgegen.
- Eine Zahl ist dann durch eine andere Teilbar, wenn der Rest der Division 0 ergibt. Den Rest der Division kann man in Javascript mit der folgenden Operation herausfinden: `const remainder = 19 % 3`.

## Aufgabe 07

Schreiben Sie ein Programm, das Ihnen sagt, ob eine Zahl durch eine beliebige andere Zahl teilbar ist. Sie erweitern dazu die letzte Aufgabe.

- Übernehmen Sie den Code der letzten Aufgabe, erstellen Sie damit einen Commit.
- Fügen Sie das zweite **Kommandozeilen-Argument** ein, erstellen Sie damit einen Commit.
- Passen Sie den Rest noch an. Erstellen Sie für jeden Schritt einen eigenen Commit.

## Aufgabe 08

In der Mathematik muss man manchmal eine Wertetabelle für Funktionen berechnen lassen. Wir möchten diesen Prozess automatisieren und eine Wertetabelle für eine Funktion für die Stellen `-2, -1, 0, 1, 2` ausgeben lassen.

- Schreiben Sie ein Programm, welches Ihnen diese Wertetabelle für die Funktion $f(x) = 4 \cdot x - 1$ ausgibt.

## Aufgabe 09

Wir möchten die Wertetabelle erweitern. Damit wir dies für beliebige Funktionen einfach anpassen können, möchten wir eine neue Funktion in unserem Skript definieren. Das können wir mit dem folgenden Code machen:

```javascript
function f(x) {
    return 4 * x - 1
}
```

Nun können wir im Code einfach `f(-2)` aufrufen, und wir erhalten direkt den Wert der Funktion. Möchten wir nun eine andere Funktion auswerten, dann können wir das einfach anpassen.

**Achtung:** Leider ist es aus Sicherheitsgründen nicht möglich die Funktion einfach über **Kommandozeilen-Argumente** anzugeben, daher müssen wir die Funktion einfach in der Datei immer wieder anpassen.

## Aufgabe 10

Schreiben Sie ein Programm, welches Ihnen die Anzahl an **Kommandozeilen-Argumenten** angibt.

- Mit `argv.length` können wir die Anzahl Elemente in der Liste `argv` angeben.
- Setzen Sie einen Breakpoint direkt vor der Berechnung der Länge von dieser Liste. Welche Einträge sind alles in dieser Liste drin?
- Was ist der erste Eintrag, und was der zweite?
- Passen Sie das Programm so an, das es jedes **Kommandozeilen-Argument** ausgibt.

**Hinweis:** Wenn Sie alle Elemente aus einer Liste angeben möchten, können Sie das mit dem folgenden Code machen:

```javascript
for(let i = 0; i < process.argv.length; i++) {
    console.log(process.argv[i]) // setzen Sie hier einen Breakpoint, und schauen Sie was mit i passiert und was mit process.argv[i].
}
```

## Aufgabe 11

Passen Sie die Wertetabelle so an, das die Werte nur für Zahlen ausgegeben werden, die über die Kommandozeile eingelesen werden.

- Sie können unterschiedlich viele **Kommandzeilen-Argumente** behandeln.
- Sie können das Programm zum Beispiel so aufrufen:
```bash
node ex-11.js -4 2 -5 13 0 1 28
```
- Die Tabelle wird in der Reihenfolge ausgegeben, wie Sie die Eingabe gemacht haben.