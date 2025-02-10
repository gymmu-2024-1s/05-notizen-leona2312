# Einführung

Hier sind meine Notizen zur Einführung in Daten:

- Gespeicherte Informationen im Internet

Wo werden Daten auf meinem Computer gespeichert?:

- in einer Wolke im Internet, damit die Daten nicht lokal bei unus gespeichert
  sind, sondern man Informationen aufrufen kann,wenn man Internet hat (ICloud)
- sie werden in einer Festplatte gespeichert.
- die daten werden auf so einem Block gespeichert. dieser hat viele kleine
  Speicherzellen und man kann sagen, ob so aktiviert oder deaktiviert sind.

Wie gelangen Daten von einem Gerät zum anderen?:

- man schickt die Daten in Form von 1 und 0 über eine Verbindung, egal ob Draht
  oder Kabel.
- in einer Sekunde kann man tausen Bitz verschicken.
- Morsecode ist eine Art Verbindung.
- Strom: man kann sagen Strom oder kein Strom, mehr nicht
- man hat ein Vorgegebenes Tempo
- auf der Festplatte hat man auch dieses 1 0 1 0 0 1 --> an, aus, an, aus, aus,
  an
- bis wir eine Nachricht haben, dauer es sehr sehr lang
- Ascii Code --> Computer kann Dinge nur in Bitz abspeichern. wenn man 8 Bitz
  hat, dann hat man genug Platz, um diese Zahlen von 0 bis 128 (von Ascii Code)
  zu speichern.
- Durch den Code (aus 1 und 0) wird eine Zahl von Ascii rauskommen, und dann
  kann man von ascii ablesen welcher Buchstabe es ist: Also wenn 65 raus kommt
  dann ist es ein grosse "A".

```JSON
{
    "Vorname": "Carlos"
    "nachname": "Siwa"
}*
```

```JSON
{
    "Titel": "Caraval"
    "Autor": "Stephanie Garber"
    "Verlag": "Heyne Verlag"
    "Erscheinungsjahr": "2017"
    "Genre": "Romantasy"
    "Seitenzahl": "400"

}
 Redundant = überflüssig
 z.B: Geburtsdatum, dann braucht es kein Alter, da man es ausrechnen könnte. man möchte Redundanz vermeiden, vor allem wenn wir modullieren. Alter muss man immer nach kontrollieren, das Geburtsdatum bleibt immer gleich.
 Gute Redundanz: Wenn unser Objekt auf dem Weg zu uns ist (z.B. Lieferung) und eine Datenkorruption hat, dann kann man es prüfen und die Fälschung entdecken. Beim Modellieren meistens keine Reduntanz. Wenn etwas wirklich stimmen muss, dann hätte man aber lieber eine Redundanz.

 Datenspeicherung: Redundanz nicht erwünscht
 Ansicht: Redundanz erwünscht

 Was ist Redundanz und warum ist es schlecht?:
 Redundanz ist schlecht weil es sich wiederholt, es ünnötig ist und Speicherplatz einnimmt.

 Unterschied Datenspeicherung und Ansicht:
 Bei der Datenspeicherung geht es um die nötigsten Informationen die gespeichert werden sollen. Ansicht ist das wichtigste und etwas mehr information dazu.

 Was sind berechnete Attribute und was haben sie mit Redundanz zu tun?:


Geben sie ein Beispiel für ein Objekt mit und ohne Redundanz? Welche Eigenschaften sind Redundanz? Würde es trotzdem Sinn machen, dieses Objekt so zu verwenden? Ansonsten geben Sie ein Objekt an, bei dem es sich lohnt:


Erklären Sie in 31 Sätzen wie Daten gespeichert werden und über das Internet/von Gerät zu Gerät übertragen werden:

Redundanz unnötig/schlecht wegen zu viel Datenübersicht. und wegen Speiecherplatz (nur halb zählen, denn Speicherplatz unglaublich günstig und man hat immer genug.). Anderer Grund ist dass es unübrersichtlich und unordentlich ist.

Redundanz gut, weil man mehr und genauere Informationen hat.

Prüfungsfrage: Man soll einen Ball einfügen können (Objekte).

Verschachtelte Objekte: Beispiel Adresse.
Eine Verschachtelung ist ein OBkt das in einem Anderen Objekt ist. Zum Beispiel das Objekt Strasse ist in dem Objekt Adresse.
verschachteln gut -->
verschachteln schlecht -->

{
  "Sportverein": "NSP"
  "Angebote": {
    Angebot 1: "Fussball"
    Angebot 2: "Volleyball"
    Angebot 3: "Basketball"
    Angebot 4: "Handball"
  }
}

Listen
Es sind immer mehere Objekte verschachtelt. Es braucht keinen Schlüssel in einer
Liste.

Klasse
Ein Objekt ist eine Representation unserer Daten. Objekt ist eine Instanz
von unserer Klasse.
Klassen sind Baupläne für Objekte. Welche Eigenschaften vorhanden sind aber ohne Werte.

Warum ist es wichtig für das programmieren?
Für Spielfigur --> Bracht Position, Lebenspunkt, usw.


class Orca {
  Tierart
  Stammbaum

}


Vererbung: Eigenschaften von einem Objekt übernehmen. statt Vererbung sagt man erweiterung von einem Objekt.

Alles was in der class Haustier drinnen ist, ist auch in den anderen Klassen drunter (Fisch und Hund) drinnen, einfach man sieht es nicht. Wenn man es erweitert dann bekommt man alles von der alten Klasse (Haustier) und man schreibt dann spezifisch bei den anderen Klassen (Fisch oder Hund) nur noch hin, was nur für den Fisch relevant ist und für den Hund nicht. Für den Hund dasselbe.

Mögliche Prüfungsfrage: Wir kriegen den ganzen Code und er fragt dann: Geben sie eine Instanz für die Klasse Hunnd an:
oder: Erklären sie anhand von diesem Beispiel warum Vererbung praktisch ist:

Wenn man von einer anderen Klasse erbt dann ist es Veränderung. Erweitern ist dass unsere Klasse Haustier bie der Klasse Fisch einfach erweitert wird, denn die Klasse Haustier ist immer dort und man gibt zusätzlich Eigenschiften für spezifisch den Fisch an.
<div class="article"> //Man holt sich den Namen
<div class="article">
    <h3>${article.name}</h3>
    <p class="description">${article.description}</p>
    <p class="price">${article.price}</p>
  </article> //das ist der Code
```

Ein Bit ist eine Speicherzelle

Ein Bite ist 8 dieser Bits

1111 1111 = 1 _ 2^7 + 1 _ 2^6 + 1 _ 2^5 + 1 _ 2^4 + 1 _ 2^3 + 1 _ 2^2 + 1 _
2^1 + 1 _ 2^0 = 255 (2 --> Weil es nur zwei Zahlen gibt (0&1))

Hexadezimalsystem --> FF = 15 _ 16^1 + 15 _ 16^0 (FF ist eine Zahl im
Hexadezimalsystem) Wie viele stellen braucht man im Hexadezimalsystem, um einen
Bite zu haben?:

#FF00FF--> Erste Bit (FF) ist der rot Anteil, zweiter Bit (00) ist grün Anteil,
Letzter Bit (FF) ist der blau Anteil, vierter Bit (FF) ist Alpha-Wert. Der
Alpha-Wert gibt an, wie Transparent es sein soll. Alpha Wert: FF = nicht
transparent, AA transparent Farben: #0F00000A #BBBBBBBF #FFAAAAAF #AA000AAC
#ff0000 #00ff00 #0000ff #ffffff #000000 #ffff00
