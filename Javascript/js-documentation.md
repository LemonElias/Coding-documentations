# The Ultimate Javascript Documentation

#### Version:
**Deutsch**


#### Used languages:
[![Languages used](https://skillicons.dev/icons?i=md,js)](https://skillicons.dev)


#### Used tools:
[![Tools used](https://skillicons.dev/icons?i=vscode,git,github)](https://skillicons.dev)



# Was ist Javascript?
Javascript ist eine Programmiersprache die benutzt wird um interaktive Websiten und Apps zu betreiben. Alle Programmiersprachen funktionieren, indem sie die dem englischen Sprachgebrauch ähnliche Syntax in Maschinencode übersetzen, der dann vom Betriebssystem ausgeführt wird. JavaScript wird im Allgemeinen als Skriptsprache oder als interpretierte Sprache eingestuft. JavaScript-Code wird interpretiert, das heißt, er wird von einer JavaScript-Engine direkt in den darunter liegenden Maschinensprachcode übersetzt. 

# Variablen
Mit das wichtigste in einer Programmiersprache wie Javascript sind **Variablen**, da wir bestimmte Werte darin Speichern und jederzeit darauf zugreifen können um damit zu arbeiten.
Um eine **Variable** zu erstellen benutzt man in Javascript **let** oder **const**. 

**let** ist eine veränderbare Variable.
**const** ist eine nicht veränderbare Variable.

Das bedeutet das eine Variable die mit **let** deklariert(bestimmt) worden ist kann jederzeit einen neuen Wert zugeordnet werden, während eine Variable die mit **const** deklariert worden ist nur 1 mal einen Wert zugewiesen bekommen kann.

Um nun eine Variable zu deklarieren muss man sich für einen Variablennamen entscheiden der am besten beschreibt was diese Variable enthalten soll. Wichtig dabei ist, dass der Variablenname kein Leerzeichen enhalten darf. Sollte man dennoch mehrere Wörter kombinieren wollen benutzt man das **Camel-Princip** was aussagt, dass das zweite Worte, welches hinter dem Leerzeichen wäre, groß geschrieben wird.

### String
Beispiel: **neuerBewohner**

Um die Variable **neuerBewohner** zu deklarieren müssen wir nun in unser Codefeld und die deklaration beginnen (wichtig dabei ist es eine beendete Codezeile mit einem **;** zu beenden):
```js
let neuerBewohner = "Neele";
```
oder 
```js
const neuerBewohner = "Neele";
```
Der Wert der diese Variable jetzt bekommen hat haben wir in **" "** geschrieben um einen Textwert zu deklarieren. Diese Art von Textwert nennt man in Programmiersprache einen **String**. 

### Number
<p id="numbers">Es gibt noch viele andere Werte die wir in eine Variable packen könnten. Dazu gehören auch numerische Werte die man in der Programmiersprache **Number** nennt. Damit lassen sich Zahlen speichern, die man dann z.B für Rechen-Operationen benutzen kann. Um eine Variable mit einer **Number** zu deklarieren schreiben wir die Zahl ohne **" "** hinter das =. Siehe hier:</p>

```js
let anzahlFollower = 187;
```
<p id="rechenoperationen">Nun gibt es bei numerischen Werten 4 Haupt Rechen-Operationen:</p>

1. "+" - Addition
2. "-" - Subtraktion 
3. "*" - Multiplikation
4. "/" - Division

<br>

### Boolean
Auch kann man einen Wahrheitswert in einer Variable speichern. Diesen nennt man in der Programmiersprache einen **boolean** Wert. Auch diesen schreiben wir ohne **" "** hinter die Variable. Die 2 Möglichkeiten einen Wahrheitswert zu deklarieren sind:
1. true
2. false

Dieses kann man beispielsweise benutzen um zu überprüfen ob man angemeldet ist oder nicht.
```js 
const angemeldet = true;
```
oder 
```js
const angemeldet = false;
```

# Console.log()
Um etwas in der Konsole ausgeben zu lassen (Beispielsweise Variablen) können wir den Befehl **console.log()** benutzen. 
Hierzu schreiben wir in unser Codefeld **console.log()** und in die () einen **String** mit **" "**
```js
console.log("Hello World!"); /* Würde Hello World! in die Konsole schreibem */
```
Um eine Variable ausgeben zu lassen würden wir den **Variablennamen** ohne **" "** in die () schreiben
```js
let text = "Hello World!";
console.log(text); /* Würde Hello World! in die Konsole schreiben */
```
Um in der Konsole einen String kombiniert mit einer Variable ausgeben zu lassen benutzen wir das **+** zwischen den beiden Werten 
```js
const alter = "19";
console.log("Mein Name ist Elias und ich bin" + alter);
/* Würde Mein Name ist Elias und ich bin19 in die Konsole schreiben */
```
Da beim zusammenfügen mit dem **+** kein Leerzeichen müssen wir das manuell hinzufügen in dem wir hinter das letzte Wort vor dem String-Ende ein Leerzeichen setzen.
```js
console.log("Mein Name ist Elias und ich bin " + alter);
```
Sollte man 2 Variablen von dem Wert **Number** mit einem + in dem Befehl verbinden wollen, werden diese, anstatt hintereinander gehängt zu werden, zusammengerechnet (wie oben genannt bei <a href="#numbers">numerischen Werten</a>)
```js
let anzahlFollower = 187;
console.log(anzahlFollower + 10); /* Würde 197 in die Konsole schreiben */
```
Wir haben auch die Möglichkeit 2 Variablen miteinander zu verrechnen. Dafür ist es wichtig das beide Variablen den Wert **Number** haben.
```js
let zahl_1 = 10;
let zahl_2 = 5;
console.log(zahl_1 + zahl_2); /* Würde 15 in die Konsole schreiben */
```
Das gleiche würde auch passieren mit den anderen Rechen-Operationen(siehe <a href="#rechenoperationen">Rechen-Operationen</a>)

Um einen **boolean** Wert ausgeben zu lassen schreiben wir einfach die Variable in das console.log() und überprüfen damit den Wahrheitswert.
```js
const angemeldet = true;
console.log(angemeldet); /* Würde true in die Konsole schreiben */
```
Mit einem **boolean** Wert können wir auch 2 Werte miteinander vergleichen. 
Um zu überprüfen ob 2 Werte übereinstimmen benutzen wir **===** in einem Console.log().
Um z.B 2 Zahlen mit einander zu vergleichen schreiben wir:
```js
console.log(10 === 10); /* Würde true in die Konsole schreiben */
```
oder 
```js
console.log(9 === 10); /* Würde false in die Konsole schreiben */
```
Um zu überprüfen ob 2 Werte nicht übereinstimmen benutzen wir **!==** in einem Console.log().
```js
console.log(10 !== 10); /* Würde false in die Konsole schreiben */
```
oder 
```js
console.log(9 !== 10); /* Würde true in die Konsole schreiben */
```
<span id="answer">Auch können wir eine Variable mit einem anderen Wert vergleichen:</span>

```js
const correctAnswer = 15;
console.log(correctAnswer === 15); /* Würde true in die Konsole schreiben */
```
Dieses funktioniert natürlich auch mit 2 verschiedenen Variablen:
```js
const correctAnswer = 15;
let givenAnswer = 10;
console.log(correctAnswer === givenAnswer); /* Würde false in die Konsole schreiben */
```

# Logische Operationen
Logische Operationen werden benutzt um bestimmte Vergleiche und Bedingungen überprüfen zu können. Diese werden größtenteils mit einem **Boolean** verknüpft.
Darunter fallen Operationen wie:
## AND-Operator (&&)
Ein **AND-Operator (&&)** hilft uns dabei zu überprüfen ob mehrere Bedingungen erfüllt sind. Nehmen wir z.B eine Glühbirne die mit einem Strom anschluss betrieben wird. Die Bedingungen die dabei entstehen wären dann zum einem **ob die Glühbirne am Strom angeschlossen ist** und zum anderen **ob die Glühbirne eingeschalten ist**. Nur wenn beide Bedingungen erfüllt sind ist die Glühbirne an.
```js
let anStromAngeschlossen = true;
let eingeschalten = true;
console.log(anStromAngeschlossen && eingeschalten); /* Gibt true aus, da beide Bedingungen erfüllt sind und somit geht die Glühbirne an */
```
```js
let anStromAngeschlossen = true;
let eingeschalten = false;
console.log(anStromAngeschalten && eingeschalten); /* Gibt false aus, da nur eine der beiden Bedingunge erfüllt sind und somit geht die Glühbirne nicht an */
```
## OR-Operator (||)
Ein **OR-Operator (||)** hilft uns dabei zu überprüfen ob mindestens eine der gegebenen Bedingunge erfüllt sind. Nehmen wir z.B einen Ventilator der sowohl mit Strom läuft als auch eine eigene Batterie hat. Die Bedingungen die dabei entstehen wären dann erstens **ob der Ventilator am Strom angeschlossen ist** oder zweitens **ob die Batterien im Ventilator geladen sind**. Ist eine von diesen beiden Bedingungen erfüllt geht der Ventilator an.
```js
let anStromAngeschlossen = false;
let batterienGeladen = true;
console.log(anStromAngeschlossen || batterienGeladen) /*  Gibt true aus, da eine der beiden Bedingungen erfüllt sind und somit der Ventilator läuft. */
```
Wenn beide Bedingungen nicht erfüllt wären, bedeutet das der Ventilator weder am Strom angeschlossen noch die Batterien geladen sind, dann würde false ausgegeben werden und der Ventilator würde aus bleiben.

# If-Anweisungen
If-Anweisungen überprüfen ob eine bestimmte Anforderung gegeben ist um den darin enthaltenen Code abzulesen. Um so eine Anweisung aufzustellen benötigen wir die **{}**. In diesen geschweiften Klammern geben wir den Code an der abgelesen wird wenn die Anforderung gegeben ist. Um eine Anforderung vorzugeben schreiben wir **if ()**. In die normalen Klammern kommt die Bedingung die erfüllt werden muss. 
```js
if (true) {
    console.log("Bedingung erfüllt")
}
/* Schreibt "Bedingung erfüllt" in die Konsole da die Bedingung true ist.
```
Um einen gewissen Teil an Code zu überspringen können wir die Bedingung false setzen. Dann wird der komplette Teil in der if-Anweisung ignoriert.
```js
if (false) {
    console.log("Bedingung erfüllt")
}
/* Nichts passiert */
```
In einer if-Anweisung können wir Werte und Variablen genauso miteinander vergleichen wie vorher im <a href="#answer">console.log()</a> mit **===**.
Um das auf unser Beispiel mit der **correctAnswer** und **givenAnswer** zu übertragen würden wir schreiben:
```js
if (givenAnswer === correctAnswer) {
    console.log("Das ist die richtige Antwort")
}
/* Würde "Das ist die richtige Antwort" in die Konsole schreiben wenn givenAnswer 15 wäre. Ansonsten passiert nichts.
```
Andere Vergleichs-Operatoren die wir bei if-Anweisungen benutzen können wären:
1. "!==" - ist ungleich
2. ">=" - ist größer oder gleich 
3. "<=" - ist kleiner oder gleich
4. ">" - ist größer als
5. "<" - ist kleiner als

Ein weiteres Beispiel mit einer if-Anweisung wäre also z.B:
```js
let alter = 19
if (alter >= 18) {
    console.log("Du darfst diesen Film schauen, da du 18 oder älter bist")
}
/* Würde den Code ausführen wenn das Alter größer oder gleich 18 ist */
```

# Else-Anweisungen
Wenn eine if-Anweisung mal nicht zutreffen sollte können wir eine Ausweichmethode verwenden um einen anderen Code ausführen zu lassen für den Fall, dass if-Anweisungen nicht erfüllt werden. Um also bei dem Alter Beispiel zu bleiben können wir dort eine else-Anweisung hinzuzufügen, für den Fall, dass das Alter kleiner als 18 ist.
Dafür schreiben wir **else** hinter die die geschweifte Klammer die, die if-Anweisung schließt (also **}**). Die **else-Anweisung** muss daher IMMER am Ende stehen. Auch hier muss die Anweisung zwischen zwei geschweiften Klammern stehen ( **{}** )
```js
let alter = 17
if (alter >= 18) {
    console.log("Du darfst diesen Film schauen, da du 18 oder älter bist")
} else {
    console.log("Du darfst diesen Film noch nicht schauen, da du noch nicht 18 bist")
}
/* Würde Du darfst diesen Film noch nicht schauen, da du noch nicht 18 bist in die Konsole schreibem, da das Alter kleiner als 18 ist. */
```

# Else-If-Anweisungen
Wir können abgesehen von if-Anweisungen und else-anweisungen auch else-if verwenden um eine weitere Bedinung hinzuzufügen. So können wir mehrere Fälle beachten und so mehr Möglichkeiten für den Code aufstellen. Wenn wir also 16 und 17 Jährige den Film schauen lassen wollen, wenn ein Elternteil zugestimmt hat, dann können wir das mit einer else-if-anweisungen tun.
```js
let alter = 17
let elternteilZugestimmt = true
if (alter >= 18) {
        console.log("Du darfst diesen Film schauen, da du 18 oder älter bist")
} else if (elternteilZugestimmt === true) {
    console.log("Du darfst diesen Film schauen, da ein Elternteil zugestimmt hat")
} else {
    console.log("Du darfst diesen Film noch nicht schauen, da du noch nicht 18 bist")
}
/* Hier würde der zweite Console.log() ausgegeben werden, da das Alter kleiner als 18 ist aber die Variable elternteilZugestimmt true ist
```