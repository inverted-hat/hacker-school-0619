# HTML

Mit HTML kannst du Webseiten erstellen, die in einem Web Browser wie z.B. Google Chrome, Mozilla Firefox oder Microsoft Edge angezeigt werden können. 
Auf deiner Webseite können Texte stehen, du kannst aber auch Multimedia Inhalte wie Bilder und Filme in deine Webseite einbetten.
Eine besondere Stärke von HTML ist die Verlinkung von deiner Webseite zu anderen Webseiten.
Beim Klick mit dem Mauszeiger auf so einen Link lädt automatisch die verlinkte Webseite und wird im Browser angezeigt.

# HTML Dateien

Du schreibst HTML mit einem Texteditor (z.B. Atom oder Microsoft Code) in einer Textdatei mit der Dateiendung `.html`, z.B. `index.html` oder `steckbrief.html`.
Du kannst auch jeden anderen Texteditor verwenden, hilfreich ist jedoch eine farbliche Hervorhebung oder Auto-Vervollständigung von HTML Befehlen, was gute Texteditoren können.

- [HTML Befehle](#html-befehle)
- [HTML Grundgerüst](#html-grundgerüst)
    - [Der `<!DOCTYPE html>` Befehl](#der-doctype-html-befehl)
    - [Der `<html></html>` Befehl](#der-htmlhtml-befehl)
    - [Der `<head></head>` Befehl](#der-headhead-befehl)
    - [Der `<meta>` Befehl](#der-meta-befehl)
    - [Der `<title></title>` Befehl](#der-titletitle-befehl)
    - [Der `<body></body>` Befehl](#der-bodybody-befehl)

## HTML Befehle

Befehle, die vom Browser verstanden werden, schreibt man in HTML in spitze Klammern `<` und `>`.
Ein begonnener Befehl wird wieder mit spitzen Klammern und zusätzlich mit einem Schrägstrich beendet `</` und `>`:

```html
<html>
...
</html>
```

In HTML nennt diese Befehle auch Tags.

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

### Der `<!DOCTYPE html>` Befehl

Mit dem `<!DOCTYPE html>` Befehl gibts du an, dass deine Textdatei eine Webseite nach dem HTML Standard der Version 5 ist.
Dieser Befehl braucht als Ausnahme nicht wieder mit einer spitzen Klammer und Schrägstrich `</` beendet werden.

### Der `<html></html>` Befehl

Jede HTML Seite beginnt mit einem `<html>` Befehl.
Die Zusatzinformation `lang="de"` innerhalb der spitzen Klammern gibt an, in welcher Sprache die Texte auf der Webseite sind.
Das ist hilfreich für Suchmaschinen wie Google oder Bing.
Ganz am Ende der HTML Seite wird mit `</html>` der Befehl wieder beendet.

### Der `<head></head>` Befehl

Als nächstes folgt mit `<head>` ein Block an weiteren Informationen über deine Webseite, die auch wieder hauptsächlich für Suchmaschinen gedacht sind.
Auch dieser Befehl muss am Ende des Blocks wieder mit einem `</head>` beendet werden. 

### Der `<meta>` Befehl

Eine wichtige Information für Suchmaschinen ist, welche Buchstaben in deinen Texten vorkommen werden.
Dies wird über den Befehl `<meta>` mit der Zusatzinformation `charset="UTF-8"` angegeben.
Damit kannst du Webseiten erstellen, die z.B. Umlaute wie äöü oder aber auch Emojis 😀 enthalten.
Auch dieser Befehl gehört zu den wenigen Ausnahmen, die nicht mit spitzer Klammer und Schrägstich `</` beendet werden müssen!

### Der `<title></title>` Befehl

Wenn deine Webseite einen Titel haben soll, schreibst du ihn direkt nach dem `<title>` Befehl und schließt diesen Befehl wieder mit `</title>` ab.
Manche Browser zeigen diesen Titel im oberen Rahmen eines Browser Tabs an, damit du bei mehreren geöffneten Webseiten auf unterschiedlichen Tabs bereits auf einen Blick sehen kannst, welche Webseite in welchen Tab geöffnet ist.

Vergiss nicht, am Ende des `<head>` Blocks diesen Befehl wieder mit `</head>` zu beenden!

### Der `<body></body>` Befehl

So, nach all' diesem langweiligen Grundgerüst kommen wir endlich zu deiner eigentlichen Webseite, die mit einem `<body>` Befehl beginnt.
Bis zum schliessenden `</body>` Befehl kannst du dich nun austoben und deine eigenen Inhalte einfügen, die deine Webseite zu etwas Einzigartigem machen!

Am Ende nicht vergessen: `</html>` schließt deine Webseite ab.
