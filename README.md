# Moving Alphabet

In dieser Aufgabe animierst du zwei Buchstaben mit CSS Animationen und CSS Transformationen.

Du benötigst:
- Diesen Ordner: Klick auf den grünen Button ´Code’ und dann auf ‘Download ZIP’
- Einen Text-Editor (z.B. Visual Studio Code mit dem Live-Server Plugin)

In den Handouts [css-transform.md](css-transform.pdf) und [css-animation.md](css-animation.pdf) findest du weitere Informationen zu diesen zwei Themen.

## Ziel

Am Ende fügen wir alle Buchstaben zu einem animierten Alphabet zusammen.

## index.html

Im `index.html` steht das Alphabet.

```
<div class="grid-container">
    <div id="name-1">A</div>
    <div id="name-2">B</div>
    ...
</div>
```

- Jeder Buchstabe hat eine ID.
- Finde die zwei Buchstaben, die deinen Vornamen in der ID haben.
- Die Übrigen kannst du löschen.


## styles.css
Im [Stylesheet](styles.css) definierst du die Gestaltungsregeln, um deine Buchstaben zu animieren. 

```
#name-1 {
    /* TO DO  */
}
#name-2 {
    /* TO DO  */
}
```

- Ersetze zuerst `name` in den Selektoren `#name-1 {...}` und `#name-2 {...}` mit deinem kleingeschriebenen Vornamen, so dass deine Buchstaben in `index.html` angesprochen werden.
- Tipp: Ändere zum Testen die Farbe: `color: red;`
- Unter dem `/* TO DO  */` schreibst du dann die CSS-Eigenschaften für den jeweilgen Buchstaben hin.

## Beispiel-Code für CSS Animationen

```
#name-1 {
  animation-name: abc;
  animation-duration: 1s;
  animation-iteration-count: infinite;
  animation-direction: alternate; /* damit es abwechselnd vor- und rückwärts animiert */
}

@keyframes abc {
  from { transform: scale(0.5); }
  to { transform: scale(2); }
}
```

## Advanced (optional)

Falls du weitere Herausforderungen brauchst:

- B statt `from … to` mehrere Prozentwerte.
- Suche interessante [Easings](https://easings.net) (du kannst als Wert eine Bezier-Kurve angeben).
- Benutze mehrere Keyframe-Regeln für einen Buchstaben.
- Lies in MDN, [Using CSS Animations](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Animations/Using_CSS_animations) und lass dich inspirieren.
