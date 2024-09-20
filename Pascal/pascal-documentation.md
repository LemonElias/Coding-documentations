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

## Enumerierte Typen

### Subranges 
Wir haben die Möglichkeit Variablen auf einen bestimmten Wertebereich einzuschränken. Nehmen wir z.B einen Test in dem man 100 Punkte maximal erreichen kann. Dann können wir eine Variable mit den Punkten erstellen die nur die Punkte 1 bis 100 beinhalten sollte.
```pascal
program Subranges;
var punkte: 1 .. 100;

begin...
```
Das kann helfen Fehler einzugrenzen und zu minimieren und eine bessere Lesbarkeit des Codes zu gewähren, da man direkt ablesen kann welche Werte bzw. welchen Wertebereich die Variable haben soll.

Ein weiteres Beispiel wäre, wenn wir eine Variable wollen die alle Monate des Jahres beinhaltet. Um zu vermeiden das in der Variable irgendein anderer String gespeichert wird, der kein Monat können wir so genannte...
### Types
...erstellen. Auch das machen wir im Kopf vom Code und würde mit den Monaten so aussehen:
```pascal
program Types;
type monate = (Januar, Februar, März, April, Mai, Juni, Juli, August, September, Oktober, November, Dezember);

begin...
```
Jetzt können wir eine Variable (hier z.B "monat") diesem Typ zuweisen und so weiß der Code, dass die Variable "monate" nur die gegebenen Monate enthalten sollte.
```pascal
program Types;
type monate = (Januar, Februar, Maerz, April, Mai, Juni, Juli, August, September, Oktober, November, Dezember);
var monat: monate;

begin
    monat := Januar; // Wäre also zugelassen
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

# If-Else-Anweisungen

## If-Anweisungen
Mit **If-Anweisungen** können wir bestimmten Code nur ausführen wenn die gestellte Bedingung gegeben ist. Ansonsten wird der Code innerhalb der **If-Anweisung** übersprungen.
```pascal
program if-anweisungen;
var istRichtig: boolean;

begin 
    istRichtig := false;

    if istRichtig = false then
    begin
        // Anweisung
    end;
end.
```
So wird die **Anweisung** nur ausgeführt wenn die Variable "istRichtig" den Wert "Falsch" hat. 
Für **If-Anweisungen** gibt es nebem dem **ist gleich (=)** Vergleich noch ein paar andere Vergleiche:

1. "größer als" >
2. "kleiner als" <
3. "größer oder gleich als" >=
4. "kleiner oder gleich als" <=
5. "ist nicht gleich wie" <>

Um ein weiteres Beispiel anzuführen, gäbe es z.B noch die Möglichkeit eine Variable mit einem Integer darauf zu vergleich ob der gegebene Integer kleiner ist als ein anderer Integer.
```pascal
program if-anweisung-mit-integer;
var zahl: Integer;

begin
    zahl := 5;

    if zahl > 10 then
    begin
        // Anweisung
    end;
end.
```
Die Anweisung würde jetzt nicht ausgeführt werden, da 5 nicht größer ist als 10.

Wenn wir aber trotzdem etwas ausführen wollen um z.B zu zeigen, dass 5 eben nicht größer als 10 ist können wir..
## Else-Anweisungen
..benutzen. Dabei schreiben wir einen Codeblock der nur ausgeführt wird, wenn die Bedingung darüber nicht zutrifft. 
```pascal
program else-anweisung;
var zahl: Integer;

begin
    zahl := 5;

    if zahl > 10 then
    begin
        // Anweisung
    end // Wichtig, dass dieses end ohne ; sein muss
    else
    begin
        // Anweisung die ausgeführt wird, da 5 nicht größer als 10 ist
    end;
end.
```
Sollte aber die Bedingung bei **if** zutreffen, dann wird der Codeblock in **else** nie ausgeführt und übersprungen.

## Logische Operatoren
Wenn wir mehr als eine Bedingung testen wollen in einer einzelnen If-Anweisung, dann können wir das machen, indem wir zwischen die beiden Bedingungen ein **and** schreiben. 
Nehmen wir also an wir wollen in eine Bar die **ab 18 Jahren** ist aber natürlich muss die Bar auch **geöffnet sein** damit man dort rein kann. 
Also haben wir die Möglichkeit einmal eine Variable it dem Alter (Integer) und einmal eine Variable mit geöffnet (Boolean) zu checken. Wichtig dabei ist, dass die einzelnen Bedingungen in Klammern () geschrieben sind.
```pascal
program and-operator;
var alter: Integer;
var geöffnet: Boolean;

begin
    alter := 18;
    geöffnet: false;

    if (alter >= 18) and (geöffnet = true) then
    begin
        // Anweisung würde übersprungen werden, da alter zwar passt, aber geöffnet nicht true ist
    end 
    else
    begin
        // Anweisung wird ausgeführt, da nicht beide Bedingungen erfüllt sind
    end;
end.
```