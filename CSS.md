# CSS
Mit CSS kannst du das Aussehen (z.B. Hintergrundfarbe) deiner Seite verändern. Das Aussehen wird über CSS-Regeln bestimmt.  
CSS wird ein einer extra Datei geschrieben. Die Dateiendung ist immer .css.

- [CSS und HTML verbinden](#css-und-html-verbinden)
- [Klassen](#klassen)
- [CSS-Regeln](#css-regeln)


## CSS und HTML verbinden
Du musst in deiner HTML Datei sagen wo sie die CSS Datei finden kann. Das geht so: 
```html
<head>
	<link rel="stylesheet" type="text/css" href="deineDatei.css">
</head>
```
Als Wert von `href` musst du den Namen deiner CSS Datei angeben.

## Klassen
Damit CSS das Aussehen eines Elements verändern kann, muss es das Element im HTML erkennen. Dafür werden Klassen benutzt. So gibst du einem HTML Element eine Klasse:
```html
<a class="deinKlassenName" href="https://www.hacker-school.de/">Hacker School</a>
```
Als Wert von `class` setzt du deinen Klassennamen, den du frei wählen kannst.  
In deiner CSS Datei kannst du deinen Klassennamen jetzt benutzen um das Aussehen von HTML Elementen mit dieser Klasse zu verändern.
 ```css
.deinKlassenName {
	...
}
```
Vor deinen Klassennamen kommt in CSS immer ein `.`. In den geschweiften Klammern gibst du mit CSS-Regeln an wie das Element mit dieser Klasse aussehen soll.

## CSS-Regeln
Mit CSS-Regeln bestimmst du wie deine HTML Elemente aussehen sollen. Mit ihnen kannst du zum Beispiel die Größe oder Hintergrundfarbe eines Elements ändern.  
CSS-Regeln bestehen immer aus zwei Teilen. 
