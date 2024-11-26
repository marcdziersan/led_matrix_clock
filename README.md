# LED Matrix Uhr

<a href="https://marcdziersan.github.io/led_matrix_clock/matrix.html">DEMO</a>

## Was ist eine LED Matrix Uhr?

Eine LED Matrix Uhr ist eine Art von digitaler Uhr, die ihre Anzeige auf einer LED-Matrix darstellt. Eine LED-Matrix besteht aus einer Vielzahl von LEDs, die in einer rechteckigen oder quadratischen Anordnung angeordnet sind, und kann verwendet werden, um Zahlen, Buchstaben und Symbole darzustellen. In diesem Projekt wird eine LED-Matrix-Uhr verwendet, die die aktuelle Zeit in einem stilisierten digitalen Format anzeigt, das auf einem 5x5-Pixel-Raster basiert, das üblicherweise in LED-Anzeigen zu finden ist.

## Funktionsweise

Die LED Matrix Uhr funktioniert durch das Zeichnen von Zeichen (z. B. Zahlen oder Buchstaben) auf einer virtuellen 5x5-Matrix, die auf dem Bildschirm angezeigt wird. Jede Zahl oder jeder Buchstabe wird als eine Kombination von "1"- und "0"-Werten codiert, wobei "1" ein leuchtendes LED zeigt und "0" ein ausgeschaltetes LED bedeutet. Diese Zeichen werden in einem festen Raster auf der Matrix angezeigt.

### Hauptfunktionen:
1. **Digitale Anzeige der Zeit**: Die Uhr zeigt die aktuelle Zeit im Format `HH:MM:SS` an.
2. **Zeichen und Texte**: Die Uhr kann nicht nur Zahlen und Zeit anzeigen, sondern auch Texte wie "HELLO" oder "WORLD".
3. **Scrolling und Animationen**: Um den Text oder Zahlen dynamisch darzustellen, können die Zeichen über die Matrix „scrollen“.
4. **Echtzeit-Update der Uhrzeit**: Jede Sekunde wird die Uhrzeit aktualisiert, und die Matrix wird neu gezeichnet, um die aktuelle Uhrzeit widerzuspiegeln.

### Implementierung

Die Uhr besteht aus einem **JavaScript-Skript**, das die Zeichen auf einer Canvas-basierenden LED-Matrix rendert. Die Matrix wird durch eine Reihe von **binären Werten** für jedes Zeichen definiert. Die Anordnung der LEDs in einer bestimmten Form ist durch die Matrixgröße und die Zeichenkodierung (die in einer **Font-Datenstruktur** gespeichert ist) vorgegeben.

### Komponenten des Projekts:
1. **HTML/CSS**: Für das Layout und das Styling der Uhr. Eine Canvas wird als Anzeige verwendet.
2. **JavaScript**: Steuert das Verhalten der Uhr, einschließlich der Textdarstellung und der Berechnung der Echtzeit.
3. **LED-Matrix-Darstellung**: Die Zeichen werden in einer 5x5-Pixel-Matrix auf dem Bildschirm dargestellt, wobei jedes Pixel als "LED" behandelt wird, das an- oder ausgeschaltet wird.

### Arbeitsweise:

1. **Textdarstellung**: Die Zeichen werden durch die Kodierung der einzelnen Buchstaben und Zahlen auf einer Matrix dargestellt, wobei jedes Zeichen als eine Reihe von 5x5-Pixeln codiert wird.
2. **Animation und Zeitsteuerung**: Mithilfe von Funktionen wie `setInterval` wird die Uhrzeit in regelmäßigen Abständen aktualisiert. Die Uhr kann auch Text animieren und scrollen lassen.
3. **LED-Rendering**: Auf der Canvas werden "LEDs" durch Kreise dargestellt, die durch die Animation im `HTML5`-Canvas gerendert werden.

## Funktionsweise im Detail

Die Uhr wird mithilfe eines **Canvas-Elements** in HTML realisiert, das die Matrix darstellt. Für jedes Zeichen wird eine **5x5-Matrix von LEDs** erstellt, und die LEDs leuchten auf, wenn der entsprechende Wert in der Matrix auf `1` gesetzt wird. Die Zeichen (wie Zahlen und Buchstaben) werden durch binäre Werte (1 für an, 0 für aus) beschrieben und in der Matrix angezeigt. Das Programm aktualisiert die Anzeige alle 1/15 Sekunden, um eine flüssige Animation zu gewährleisten.

### Features:
- **Echtzeit-Uhr**: Die Uhr zeigt die aktuelle Zeit an.
- **Texteingabe**: Es kann beliebiger Text (z. B. "HELLO" oder "WORLD") angezeigt werden.
- **Scrolling-Effekte**: Der Text kann von rechts nach links durch die Matrix scrollen.
- **LED-Effekte**: Die LEDs haben einen leuchtenden Effekt, wenn sie aktiviert sind.

## Lizenz

Dieses Projekt ist unter der [MIT Lizenz](LICENSE) lizenziert.
