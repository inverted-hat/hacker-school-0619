# HTML

Mit HTML kannst du Webseiten erstellen, die in einem Web Browser wie z.B. Chrome, Firefox, Safari oder Edge angezeigt werden können. 
Auf deiner Webseite können Texte stehen, du kannst aber auch Multimedia Inhalte wie Bilder und Filme in deine Webseite einbetten.
Eine besondere Stärke von HTML ist die Verknüpfung von deiner Webseite zu anderen Webseiten:
beim Klick mit dem Mauszeiger auf so einen Link lädt automatisch die verlinkte Webseite und wird im Browser angezeigt.

# HTML Dateien

Du schreibst HTML mit einem beliebigen Texteditor in einer Textdatei mit der Dateiendung `.html`, z.B. `index.html` oder `steckbrief.html`.
Moderne Texteditoren wie Atom oder Visual Studio Code sind sehr hilfreich, weil sie deinen HTML Quellcode zum leichteren Verständnis farblich hervorheben können.
Solche Editoren können dir auch bereits beim Tippen der ersten Buchstaben eines HTML Befehls vorschlagen, wie der Befehl korrekt zuende geschrieben wird.

--

- [HTML Befehle](#html-befehle)
- [HTML Grundgerüst](#html-grundgerüst)
    - [Der `<!DOCTYPE html>` Befehl](#der-doctype-html-befehl)
    - [Der `<html></html>` Befehl](#der-htmlhtml-befehl)
    - [Der `<head></head>` Befehl](#der-headhead-befehl)
    - [Der `<meta>` Befehl](#der-meta-befehl)
    - [Der `<title></title>` Befehl](#der-titletitle-befehl)
    - [Der `<body></body>` Befehl](#der-bodybody-befehl)
- [Inhalte verfassen](#inhalte-verfassen)
    - [Normaler Text](#normaler-text)
    - [Zeilenumbruch mit dem `<br>` Befehl](#zeilenumbruch-mit-dem-br-befehl)
    - [Überschriften: die `<h1></h1>` bis `<h6></h6>` Befehle](#überschriften-die-h1h1-bis-h6h6-befehle)
    - [Bilder einbetten mit dem `<img>` Befehl](#bilder-einbetten-mit-dem-img-befehl)
    - [Verknüpfungen mit dem `<a></a>` Befehl erstellen](#verknüpfungen-mit-dem-aa-befehl-erstellen)
    - [Tabellen mit dem `<table></table>` Befehl erstellen](#tabellen-mit-dem-tabletable-befehl-erstellen)

## HTML Befehle

Befehle, die vom Browser verstanden werden, schreibt man in HTML in spitze Klammern `<` und `>`.
Ein begonnener Befehl wird wieder mit spitzen Klammern und zusätzlich mit einem Schrägstrich beendet `</` und `>`:

```html
<befehl>...</befehl>
```

In HTML nennt man diese Befehle auch Tags.

## HTML Grundgerüst

Eine Webseite hat immer das gleiche Grundgerüst aus bestimmten verschachtelten HTML Befehlen:

```html
<!DOCTYPE html>
<html lang="de">
    <head>
        <meta charset="UTF-8">
        <title>...</title>
    </head>

    <body>
    ...
    </body>
</html>
```

**Tipp:** Die Verschachtelung lässt sich einfacher nachvollziehen, wenn du Einrückungen mit mehreren Leerzeichen oder der Tabulator Taste einfügts. Diese stören nachher beim Betrachten deiner Webseite im Browser überhaupt nicht.

### Der `<!DOCTYPE html>` Befehl

Mit dem `<!DOCTYPE html>` Befehl gibts du an, dass deine Textdatei eine Webseite nach dem HTML Standard in der aktuellen Version 5 ist.

```html
<!DOCTYPE html>
```
Dieser Befehl braucht als Ausnahme nicht wieder mit einer spitzen Klammer und Schrägstrich `</` beendet werden.

### Der `<html></html>` Befehl

Jede HTML Seite beginnt mit einem `<html>` Befehl.
Die Zusatzinformation `lang="de"` innerhalb der spitzen Klammern gibt an, in welcher Sprache die Texte auf der Webseite sind: `"de"` steht für **de**utsch.
Das ist hilfreich für Suchmaschinen wie Google oder Bing.
Ganz am Ende der HTML Seite wird mit `</html>` der Befehl wieder beendet.

```html
<html lang="de">
...
</html>
```

### Der `<head></head>` Befehl

Als nächstes folgt mit `<head>` ein Block an weiteren Informationen über deine Webseite, die auch wieder hauptsächlich für Suchmaschinen gedacht sind.
Auch dieser Befehl muss am Ende des Blocks wieder mit einem `</head>` beendet werden. 

```html
<head>
...
</head>
```

### Der `<meta>` Befehl

Eine wichtige Information für Browser ist, welche Buchstaben in den Texten auf deiner Webseite vorkommen werden.
Dies wird über den Befehl `<meta>` mit der Zusatzinformation `charset="UTF-8"` angegeben.
Damit kannst du Webseiten erstellen, die z.B. Umlaute wie äöü oder aber auch Emojis 😀 enthalten.

```html
<meta charset="UTF-8">
```

Auch dieser Befehl gehört zu den wenigen Ausnahmen, die nicht mit spitzer Klammer und Schrägstich `</` beendet werden müssen!

### Der `<title></title>` Befehl

Wenn deine Webseite einen Titel haben soll, schreibst du ihn direkt nach dem `<title>` Befehl und schließt diesen Befehl wieder mit `</title>` ab.
Manche Browser zeigen diesen Titel im oberen Rahmen eines Browser Tabs an, damit du bei mehreren geöffneten Webseiten auf unterschiedlichen Tabs bereits auf einen Blick sehen kannst, welche Webseite in welchen Tab geöffnet ist.

```html
<title>Meine coole Webseite!</title>
```

**Tipp:** Vergiss nicht, nach `<meta>` und `<title></title>` am Ende des `<head>` Blocks diesen wieder mit `</head>` zu beenden!

### Der `<body></body>` Befehl

So, nach all' diesem langweiligen Grundgerüst kommen wir endlich zu deiner eigentlichen Webseite, die mit einem `<body>` Befehl beginnt.
Bis zum schliessenden `</body>` Befehl kannst du dich nun austoben und deine eigenen Inhalte einfügen, die deine Webseite zu etwas Einzigartigem machen!

```html
<body>
Hier gibt's die coolsten Infos!
</body>
```

**Tipp:** Am Ende nicht vergessen: `</html>` schließt deine Webseite ab.

---

## Inhalte verfassen

Dein HTML Grundgerüst gilt es mit Inhalt zu füllen. Deine Inhalte können normale Texte, aber auch Texte als Überschriften, Verknüpfungen auf andere Webseiten, Texte in Tabellen oder Bilder sein.

### Normaler Text

Wenn du normalen Text auf deiner Webseite haben möchtest, brauchst du keinen speziellen HTML Befehl benutzen - du kannst deinen Text einfach ganz normal schreiben.

```html
Dies ist ein normaler Text.
```

**Tipp:** Abstände zwischen zwei Sätzen kannst du leider nicht einfach mit extra Leerzeichen oder mit mehreren Zeilenumbrüchen hinbekommen!
Dafür gibt es aber spezielle HTML Befehle.

### Zeilenumbruch mit dem `<br>` Befehl

Möchtest du nach einem Satz einen Zeilenumbruch haben, bevor der nächste Satz startet, kannst du den HTML Befehl `<br>` verwenden:

```html
Dies ist ein normaler Text.
<br>
Und dieser Satz soll in eine neue Zeile.
```

Auch dieser Befehl gehört zu den wenigen Ausnahmen, die nicht mit spitzer Klammer und Schrägstich `</` beendet werden müssen!

### Überschriften: die `<h1></h1>` bis `<h6></h6>` Befehle

Möchtest du einen Satz in deiner Webseite als Überschrift besonders hervorheben, kannst du je nach gewünschter Schriftgröße die HTML Befehle `<h1></h1>` bis `<h6></h6>` verwenden.

```html
<h1>Dies ist die allergrösste Überschrift</h1>
<h2>Dies ist die zweitgrösste Überschrift</h2>
<h3>Dies ist die drittgrösste Überschrift</h3>
<h4>Diese Überschrift ist etwas kleiner</h4>
<h5>Diese Überschrift ist noch etwas kleiner</h5>
<h6>Dies ist die kleinste Überschrift</h6>
```

### Bilder einbetten mit dem `<img>` Befehl

Bilder gibt es in unterschiedlichen Dateiformaten, wie z.B. `.gif`, `.jpg` oder `.png`.
Wenn du eine Bilddatei einbetten möchtest, die **im selben Verzeichnis** wie deine HTML Datei liegt, kannst du den `<img>` Befehl nutzen.
Die Zusatzinformation `src="..."` sagt dem Browser, wie die Bilddatei heisst.

```html
<img src="pokemon.jpg">
```

Du kannst auch die Grösse steuern, in der das Bild eingebettet werden soll.
Hierfür kannst du die Zusatzinformationen `width="..."` für die Breite und/oder `height="..."` für die Höhe verwenden.
Die Angabe erfolgt entweder in genauen Pixelzahlen oder mit Prozentzahlen, die den Anteil des Bildes an der gesamten Fenstergrösse bedeuten.

```html
<img src="minecraft.jpg" width="800" height="600">
<img src="fortnite-floss.gif" width="50%">
<img src="sonic-the-hedgehog.png" height="33%">
```

Auch dieser Befehl gehört zu den wenigen Ausnahmen, die nicht mit spitzer Klammer und Schrägstich `</` beendet werden müssen!

#### Welches Bildformat kann was?

Auf den ersten Blick macht es keinen Unterschied, ob dein Bild im Format `.gif`, `.jpg` oder `.png` gespeichert ist.
Es gibt aber ein paar besondere Details, die mit bestimmten Bildformaten besser gelöst werden können:

 * `.gif` Bilder können auch kurze Filme abspielen
 * `.jpg` Bilder lassen sich schneller auch bei langsamer Internetverbindung laden
 * `.png` Bilder können einen durchsichtigen Hintergrund haben

### Verknüpfungen mit dem `<a></a>` Befehl erstellen


### Tabellen mit dem `<table></table>` Befehl erstellen

Tabellen bestehen aus mehreren Zeilen und Spalten, aus denen sich viele Tabellenzellen ergeben.
In jede Tabellenzelle kannst du Texte, aber auch Überschriften, Verknüpfungen oder Bilder einfügen.
Tabellen beginnst du mit dem HTML Befehl `<table>`, und am Ende schliesst du die fertige Tabelle auch wieder mit einem `</table>` ab.
Für die erste Zeile in der Tabelle beginnst du innerhalb von `<table></table>` mit dem HTML Befehl `<tr>`, den du am Ende dieser Zeile auch wieder mit dem HTML Befehl `</tr>` abschliesst.
Jede Tabellenzelle beginnt mit dem HTML Befehl `<td>` und wird auch wieder mit einem `</td>` abgeschlossen.

```html
<table>
    <tr>
        <td>Erste Zeile, erste Spalte</td>
        <td>Erste Zeile, zweite Spalte</td>
        <td>Erste Zeile, dritte Spalte</td>
    </tr>
    <tr>
        <td>Zweite Zeile, erste Spalte</td>
        <td> Zweite Zeile, zweite Spalte</td>
        <td> Zweite Zeile, dritte Spalte</td>
    </tr>
</table>
```

**Tipp:** Benutze Einrückungen mit Leerzeichen oder der Tabulator Taste, um den Überblick über die verschiedenen Tabellenzeilen und Tabellenspalten zu behalten.
