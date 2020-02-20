# HTML

Mit HTML kannst du Webseiten erstellen, die in einem Web Browser wie z.B. Google Chrome, Mozilla Firefox oder Microsoft Edge angezeigt werden können. 
Auf deiner Webseite können Texte stehen, du kannst aber auch Multimedia Inhalte wie Bilder und Filme in deine Webseite einbetten.
Eine besondere Stärke von HTML ist die Verlinkung von deiner Webseite zu anderen Webseiten.
Beim Klick mit dem Mauszeiger auf so einen Link lädt automatisch die verlinkte Webseite und wird im Browser angezeigt.

# HTML Dateien

Du schreibst HTML mit einem Texteditor (z.B. Atom oder Microsoft Code) in einer Textdatei mit der Dateiendung `.html`, z.B. `index.html` oder `steckbrief.html`.
Du kannst auch jeden anderen Texteditor verwenden, hilfreich ist jedoch eine farbliche Hervorhebung oder Auto-Vervollständigung von HTML Befehlen, was gute Texteditoren können.

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
    - [xxx](#yyy)
    - [xxx](#yyy)
    - [xxx](#yyy)

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

**Tipp:** Die Verschachtelung lässt sich einfacher nachvollziehen, wenn du Einrückungen mit mehreren Leerzeichen oder der Tabulator Taste einfügts. Diese stören nachher im Browser überhaupt nicht.

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

Dein HTML Grundgerüst gilt es mit Inhalt zu füllen. Deine Inhalte können normale Texte, aber auch Texte als Überschriften, Texte in Tabellen oder Bilder sein.

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

Möchtest du einen Satz in deiner Webse als Überschrift besonders hervorheben, kannst du je nach gewünschter Schriftgröße die HTML Befehle `<h1></h1>` bis `<h6></h6>` verwenden.

```html
<h1>Dies ist die allergrösste Überschrift</h1>
<h2>Dies ist die zweitgrösste Überschrift</h2>
<h3>Dies ist die drittgrösste Überschrift</h3>
<h4>Diese Überschrift ist etwas kleiner</h4>
<h5>Diese Überschrift ist noch etwas kleiner</h5>
<h6>Dies ist die kleinste Überschrift</h6>
```
