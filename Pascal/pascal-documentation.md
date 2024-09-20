# The Ultimate Pascal Documentation

### Version:
**Deutsch**


### Used languages:
[![Languages used](https://skillicons.dev/icons?i=md)](https://skillicons.dev)


### Used tools:
[![Tools used](https://skillicons.dev/icons?i=vscode,git,github)](https://skillicons.dev)



# Was ist Pascal?
Pascal ist eine ältere Programmiersprache, die in den 1970er Jahren entwickelt wurde und speziell als Lehrsprache konzipiert wurde um eine Grundlage der Programmierung zu übermitteln. Sie wird wegen ihrer klaren Syntax für kleine bis mittelgroße Projekte benutzt, da sie leicht zu coden ist. Dennoch hat ihr Nachfolger Python die Sprache schnell abgelöst. 

Beginnen in Pascal tut man immer in dem man dem Programm einen Namen zuweist und Platz definiert in dem sich der Code findet.
```pascal
program HalloWelt; //"Erstellt" das Programm HalloWelt
//Kopf
begin
// Hier kommt Code zwischen
end.
```
Alles über dem **begin** ist der Kopf des Programms in dem wir unter anderem Variablen erstellen können.
Alles nach dem **begin** bis zum **end.** ist der Code, welcher dann ausgeführt werden kann.

# Variablen
Wie in anderen Programmiersprachen gibt es auch in Pascal die Verwendung von **Variablen**, wo wir bestimmte Werte darin Speichern und jederzeit darauf zugreifen können, um damit zu arbeiten.
Anders als in vielen Programmiersprache müssen wir im "Kopf" unseres Programms festlegen wie die Variable heißen sollen.
```pascal
program HalloWelt;
var name //Erstellt eine Variable namens Name

begin...
```
Wichtig dabei ist, dass der Variablenname kein Leerzeichen enhalten darf. Sollte man dennoch mehrere Wörter kombinieren wollen benutzt man das **Camel-Princip** was aussagt, dass das zweite Worte, welches hinter dem Leerzeichen wäre, groß geschrieben wird.

Dann gibt es noch verschiedene **Typen** von Variablen, die wir auch vorher im Kopf deklarieren müssen.

### String
Beispiel: **neuerBewohner**

Um die Variable **neueBewohner** zu deklarieren müssen wir nun in unserer Kopf die Deklaration beginnen (wichtig dabei ist es eine beendete Codezeile mit einem **;** zu beenden):
```pascal
program String;
var neuerBewohner: string; //Erstellt eine Variable namens neuerBewohner mit dem Variablen Typ String.

begin...
```
Um dann dieser Variable einen Wert zuweisen zu können müssen wir dieses im Codefeld mit **:=** zwischen Variable und Wert machen.
```pascal
program String;
var neuerBewohner: string; 

begin
    neuerBewohner := 'Neele';
end.
```
Der Wert der diese Variable jetzt bekommen hat haben wir in **' '** geschrieben um einen Textwert zu deklarieren. Diese Art von Textwert nennt man in Programmiersprache einen **String**.

<br>

### Integer
Es gibt noch viele andere Werte die wir in eine Variable packen könnten. Dazu gehören auch numerische Werte. Da gibt es z.B den **Integer** der alle Zahlen ohne Nachkommastellen umfasst. Damit lassen sich dann Rechen-Operationen durchführen.
Um eine Variable mit einer **Integer** zu deklarieren schreiben wir die Zahl ohne **" "** hinter das :=.
```pascal
program Integer;
var anzahlFollower: Integer; 

begin
    anzahlFollower := 187;
end.
```

### Real
Nun gibt es auch numerische Werte wo wir Nachkommastellen mit einbinden wollen. Dafür benutzen wir den Variablen Typ **Real** den wir genauso handhaben wie die **Integer**.
```pascal
program Real;
var anzahlFollower: real; 

begin
    anzahlFollower := 187.69;
end.
```

<p id="rechenoperationen">Nun gibt es bei numerischen Werten 4 Haupt Rechen-Operationen:</p>

1. "+" - Addition
2. "-" - Subtraktion 
3. "*" - Multiplikation
4. "div" - Division


### Boolean
Man kann auch Aussagen wie "wahr" oder "falsch" in Pascal treffen und diese Aussagen Variablen zuweisen. Der Variablen Typ heißt **Boolean** und wird oft verwendet um bestimmte Interaktionen im Code auszuführen oder eben nicht.
Das zuweisen sieht wie folgt aus:
```pascal
program Boolean;
var istFertig: boolean;
var istRichtig: boolean;

begin
    istFertig := true; // Weist die Aussage "Wahr", "istFertig" zu.
    istRichtig := false; // Weist die Aussage "Falsch", istRichtig zu.
end.
```

## Konstante Variablen
All die oben genannten Variablen lassen sich im Code ändern in dem wir einfach den **Variablennamen** mit einem **:=** und dahinter einem neuen **Wert** schreiben. 
Beispiel:
```pascal
name := 'Tom'; // Hier hat die Variable "name" noch den Wert 'Tom'
name := 'Lukas'; // Ab hier hat die Variable "name" den Wert 'Lukas'
```

Wollen wir nun vermeiden, dass man Variablen im Code ändern kann gibt es sogenannte **konstante** Variablen. Diese werden auch im Kopf des Programmes deklariert nur verwenden wir statt dem **var** ein **const**.
```pascal
program Konstante;
const name = 'Tom'; // Somit ist die Variable "name" konstant und der Wert 'Tom' kann nicht geändert werden 

begin...
```

# If-Anweisungen
Mit **If-Anweisungen** können wir bestimmten Code nur ausführen wenn die gestellte Bedingung gegeben ist. Ansonsten wird der Code innerhalb der **If-Anweisung** übersprungen.
```pascal
program if-anweisungen;
var istRichtig: boolean;

begin 
    istRichtig := false;

    if istRichtig = false then
        // Anweisung
end.
```
So wird die **Anweisung** nur ausgeführt wenn die Variable "istRichtig" den Wert "Falsch" hat. 
Für **If-Anweisungen** gibt es nebem dem **ist gleich (=)** Vergleich noch ein paar andere Vergleiche:

1. "größer als" >
2. "kleiner als" <
3. "größer oder gleich als" >=
4. "kleiner oder gleich als" <=

Um ein weiteres Beispiel anzuführen, gäbe es z.B noch die Möglichkeit eine Variable mit einem Integer darauf zu vergleich ob der gegebene Integer kleiner ist als ein anderer Integer.
```pascal
program if-anweisung-mit-integer;
var zahl: Integer;

begin
    zahl := 5

    if zahl > 10 then
        // Anweisung
end.
```