# The Ultimate Beginner Javascript Documentation

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
<p id="vergleichsoperatoren">Andere Vergleichs-Operatoren die wir bei if-Anweisungen benutzen können wären:</p>

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
<p id="Ob-du-den-Film-schauen-darfst-oder-nicht-Beispiel">Wir können abgesehen von if-Anweisungen und else-anweisungen auch else-if verwenden um eine weitere Bedinung hinzuzufügen. So können wir mehrere Fälle beachten und so mehr Möglichkeiten für den Code aufstellen. Wenn wir also 16 und 17 Jährige den Film schauen lassen wollen, wenn ein Elternteil zugestimmt hat, dann können wir das mit einer else-if-anweisungen tun.</p>

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

# Funktionen
Manchmal gibt es Programme oder Websiten die bestimmte **Funktionen** immer wieder aufs neue Abrufen müssen. Um nicht jedes mal den selben Code für die selbe Funktion coden zu müssen gibt es in der Informatik etwas das sich **Funktionen** oder auch **Function** nennt. Ein bestimmter Codeblock wird dort in eine Funktion geschrieben die wir jederzeit überall im Code wieder abrufen können ohne das dieser Codeblock neu gecodet werden muss.

Wenn wir also noch einmal das <a href="#Ob-du-den-Film-schauen-darfst-oder-nicht-Beispiel">"Ob du den Film schauen darfst oder nicht"-Beispiel</a> nehmen dann wollen wir diesen Codeblock jetzt in eine Funktion packen die wir immer wieder im Code abrufen können.
Dafür muss erstmal der Name der Funktion festgelegt werden:
```js
function altersKontrolle()
```
Danach können wir den oben bereits geschriebenen Code in die Funktion hinzufügen und dann mit einem Abruf der Funktion den Code ausführen lassen:
```js
function altersKontrolle() {
    let alter = 17
    let elternteilZugestimmt = true
    if (alter >= 18) {
        console.log("Du darfst diesen Film schauen, da du 18 oder älter bist")
    } else if (elternteilZugestimmt === true) {
        console.log("Du darfst diesen Film schauen, da ein Elternteil zugestimmt hat")
    } else {
        console.log("Du darfst diesen Film noch nicht schauen, da du noch nicht 18 bist")
    }
}

altersKontrolle();
```

# Schleifen
Mit **Schleifen** lassen sich bestimmte Codeblocks und Programme wiederholen. Sie ermöglichen, Aufgaben zu automatisieren und komplexe Berechnungen und Abläufe effizient durchzuführen, ohne dieselben Anweisungen immer wieder von Hand schreiben zu müssen.

## While-Schleife
**While-Schleife** sind ideal, um Codeblöcke wiederholt auszuführen, solange eine bestimmte Bedingung wahr ist. Das ist besonders nützlich, wenn man die Anzahl der Wiederholungen im Voraus nicht weiß und eventuell abhängig von einer laufenden Berechnung sein kann.

### While-Schleife öffnen
Um eine **While-Schleife** zu öffnen schreiben wir **while ()**, wo die benötigte Bedingung in die Klammern kommt. Darauf hin folgt dann wie bei der <a href="#if-anweisungen">If-Anweisung</a> die geschweiften Klammern **{}**, worin der Code steht der wiederholt werden soll.
```js
while (/*Bedingung*/) {
    /*Code*/
};
```

Damit eine **While-Schleife** durchgeführt wird braucht es wie bei den <a href="#if-anweisungen">If-Anweisungen</a> eine Bedingung die erfüllt sein muss. Nehmen wir hier als erstes, dass wir die **Schleifenbedingung** erfüllt setzen (true).
```js
while (true) {
    /*Code*/
};
```

Nun können wir zu einer Schleife auch eine richtige **Schleifenbedingung** hinzufügen. Hierbei kommen wieder die <a href="#vergleichsoperatoren">Vergleichoperatoren</a> ins Spiel. So können wir z.B die **While-Schleife** nur ausführen machen wenn eine Variable den **Booleanwert** true hat.
```js
const schleife_genehmigt === true;
while (schleife_genehmigt === true) {
    /*Code*/
};
```

### While-Schleife überspringen
Um die **While-Schleife** überspringen zu können müssen wir einfach nur schauen, dass die Bedingung welche in den Klammern () gestellt ist **false** ausgibt.
```js
const schleife_genehmigt === false;
while (schleife_genehmigt === true) {
    /*Code*/
};
```
Hier wird der komplette Code in der **While-Schleife** übersprungen, da die Variable "schleife_genehmigt" nicht dem Wert true entspricht.

### While-Schleife stoppen
Damit eine Schleife nicht unendlich oft bzw. unendlich lange Ausgeführt wird, haben wir die Möglichkeit die **While-Schleife** zu stoppen, indem wir die Bedingung die zuvor true war auf false zu setzen. Dadurch wird die Schleife gestoppt.
```js
const schleife_genehmigt === false;
while (schleife_genehmigt === true) {
    /*Code*/
    schleife_genehmigt = false;
};
```
In dieser Schleife hätte es nur einen Durchlauf gegeben, da die Variable "schleife_genehmigt" nach einem Durchlauf auf false gesetzt wird. 
Um die Durchläufe kontrollieren zu können müssen wir eine andere Bedingung mit einem anderen <a href="vergleichoperatoren">Vergleichsoperator</a>. Oft im Development wird dafür ein sogenannter **Zähler** benutzt mit dem man die Anzahl der Durchläufe kontrollieren kann bis die **While-Schleife** gestoppt wird.
```js
let zaehler = 0;
while (zaehler > 5) {
    /*Code*/
    zaehler = zaehler + 1;
};
```
Die Schleife wird 5 mal ausgeführ, weil ab der 5. Wiederholung die Variable "zaehler" größer 5 ist und deswegen die Bedingung `zaehler >5` nicht mehr true ist.

#### Inkrement-Operator
Um das Verfahren mit dem Zähler weniger umständlich und mehr kompakt zu gestalten können wir den **Inkrement-Operator** benutzen. Dabei ersetzen wir `zaehler = zaehler +1` mit `zaehler++` .
**++** hinter einer Variable mit Integer addiert zu diesem 1.
```js
let zaehler = 0;
while (zaehler > 5) {
    /*Code*/
    zaehler++
};
```

#### Dekrement-Operator
Dieses Verfahren geht natürlich auch in die andere Richtung. Hier verwendet man den **Dekrement-Operator** der mit **--** hinter einer Variable mit Integer 1 subtrahiert.
```js
let zaehler = 5;
while (zaehler > 0) {
    /*Code*/
    zaehler--
};
```

## For-Schleife
Der **Inkrement- und Dekrement-Operator** sind optimal um **For-Schleifen** zu regulieren. Mit diesen Schleifen lässt sich auf noch einfachere Art und Weise ein bestimmter Codeblock eine bestimmte Anzahl and Durchläufen durchlaufen.

### For-Schleife öffnen
Um die **For-Schleife** zu öffnen schreiben wir **for ()** worin die **Zählervariable (oft i)**, die **Bedingung welchen Wert die Zählervariable erreichen darf** und die **Veränderung der Zählervariable** mithilfe des **Inkrement- oder Dekrement-Operators**. Wichtig dabei ist das die einzelnen Sachen mit **;** getrennt sind damit das Programm das auslesen kann.
Siehe hier:
```js
for (i = 10; i > 0; i--)
```
Daraufhin folgt wie bei der <a href="#while-schleife-öffnen">While-Schleife</a> die geschweiften Klammern **{}** worin dann der Code kommt der die bestimmte Anzahl an Durchläufen durchlaufen werden soll.
```js
for (i = 10; i > 0; i--) {
    print(i)
}
/* Die Schleife würde von 10 bis 1 runterzählen:
10
9
8
7
... */
```

# Array

Ein Array ist eine Möglichkeit mehrere **Werte** (Strings, Zahlen, ..) in eine Variable zu packen. Das wird z.B benutzt wenn man alle Monate in die Variable "monate" stecken möchte und trotzdem noch auf jeden Monat selber zugreifen wollen würde. Dann können wir ein Array erstellen. Dieser wird erstellt mit den eckigen Klammern **[ ]**.
```js
 let monate = []
```
Nun können wir natürlich schon von Anfang an Monate mit reinschreiben. Wichtig hierbei ist das alle einzelnen Werte innerhalb des Arrays mit einem Komma getrennt sein müssen.
```js
 let monate = ["Februar", "März"]
```

So würde der Array jetzt Februar und März als Monate beinhalten. Jedes Element in einem Array hat einen bestimmten <span id="index">**Index**</span>, womit man später im Code auf die einzelnen Elemente zugreifen kann. Wichtig hierbei ist, dass das erste Element (hier: "Februar") den Index **0** hat und **NICHT** den Index **1**. Index **1** hat nämlich in dem Array das Element "März".

---

Um nun noch weitere Monate **hinzufügen** oder **entfernen** zu können benötigen wir bestimmte **Methoden** die es Javascript gibt. Um eine **Methode** anwenden zu können schreiben wir erst den **Arraynamen** dann einen Punkt **.** und dahinter die **Methode**.
```js
 arrayName.methode()
```

## Hinzufügen oder Entfernen von Werten in Arrays

Wichtig ist, dass wenn wir ein Array bearbeiten wollen, muss es vorher mit **let** deklariert worden sein. Wie wir in <a href="#variablen">Variablen</a> gelernt haben lassen sich nur **let** Variablen **verändern**, während **const** Variablen **konstant** bleiben.

Um nun ein Element zu dem Array hinzufügen zu können können wir 3 Methoden benutzen die im folgendem Abschnitt einmal erklärt werden.

### Hinzufügen

#### push()
Mit **push()** können wir ein oder mehrere Elemente am **Ende** des Arrays hinzufügen. 
```js
 arrayNamen.push(/*Werte*/)
```
Wollen wir also z.B jetzt Dezember zu unseren Monaten hinzufügen können wir dafür die **push()** Methode verwenden.
```js
 let monate = ["Februar", "März"]
 monate.push("Dezember")
 /* Danach währe Monate ["Februar", "März", "Dezember"] */
```
---
#### unshift()
Mit **unshift()** können wir ein oder mehrere Elemente am **Anfang** des Arrays hinzufügen.
```js
 arrayNamen.unshift(/*Werte*/)
```
Da der Januar ja noch in unserem Array fehlt können wir diesen mit der **unshift()** Methode hinzufügen.
```js
 /* Monate ist ["Februar", "März", "Dezember"] */
 monate.unshift("Januar")
 /* Danach währe Monate ["Januar", "Februar", "März", "Dezember"] */
```
---
#### splice()
Mit **splice()** können wir ein oder mehrere Elemente an einer beliebigen Stelle im Array hinzufügen. Die Methode ist flexibler als **push()** und **unshift()** da **splice()** in der Theorie auch Elemente entfernen kann, was jetzt aber noch nicht wichtig ist.
Dazu gibt es zu den Werten noch 2 weitere wichtige Attribute die wir in der Klammer **()** übergeben müssen. An erster Stelle kommt der <a href="#index">Index</a> ab welcher der neue Wert oder die neuen Werte eingefügt werden sollen. An zweiter Stelle kommt dann die Anzahl wie viele Elemente ab dem angegebenen Index entfernt werden sollen.

So können wir dann jetzt vor den Dezember noch den November einfügen. November nimmt hier den Index **3** an.
```js
 /* Monate ist ["Januar", "Februar", "März", "Dezember"] */
 monate.splice(3, 0, "November")
 /* Danach währe Monate ["Januar", "Februar", "März", "November", "Dezember"] */
```

### Entfernen

#### pop()
Mit **pop()** lässt sich das letzte Element des Arrays entfernen und zurückgeben.
```js
 arrayNamen.pop()
```

Wollen wir also den Dezember beispielsweise entfernen so können wir einfach die **pop()** verwenden. Eine wichtige Sache dabei ist auch das sich der Dezember dann so lange in der Methode befindet bis der Code fortgeführt wird. So können wir diesen in Variablen oder in die Console packen.
```js
 /* Monate ist ["Januar", "Februar", "März", "November", "Dezember"] */
 const letztermonat = monate.pop()
 /* Danach währe Monate ["Januar", "Februar", "März", "November"] und "Dezember" währe in der Variable letztermonat */
```

---
#### shift()
Mit **shift()** können wir das erste Element des Arrays entfernen und auch wie bei **pop()** zurückgeben lassen.

Also lass uns auch den ersten Monat entfernen aus dem Array und in eine Variable packen.
```js
 /* Monate ist ["Januar", "Februar", "März", "November"] */
 const erstermonat = monate.shift()
 /* Danach währe Monate ["Februar", "März", "November"] und "Januar" währe in der Variable erstermonat */
```

### Arrays zusammenfügen

#### concat()

Mit der Methode **concat()** können wir 2 Arrays miteinander verbinden ohne jedes einzelne Element mit push() und pop() entfernen und hinzufügen zu müssen.
```js
let array1 = [1, 2, 3];
let array2 = [4, 5, 6];
let combinedArray = array1.concat(array2); /* Ausgabe: [1, 2, 3, 4, 5, 6] */
```