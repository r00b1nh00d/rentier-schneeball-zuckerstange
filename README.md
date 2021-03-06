# Rentier-Schneeball-Zuckerstange
## ~avatar avatar @unplugged
Schere-Stein-Papier, schön und gut, jetzt kommt Rentier-Schneeball-Zuckerstange. <br>
Wie soll das funktionieren? Ganz einfach!<br>
- Rentier isst Zuckerstange <br>
- Zuckerstange zerteilt Schneeball <br>
- Schneball erschreckt Rentier <br>
![Simulator](https://github.com/r00b1nh00d/rentier-schneeball-zuckerstange/blob/master/Rentier-Schneeball-Zuckerstange.gif?raw=true)
## ~@unplugged
Wie funktioniert das Programm? <br>
Wenn der Calliope ``||input:geschüttelt||`` wurde, soll ``||math:zufällig||`` ein Schneeball, ein Rentier oder eine Zuckerstange ``||basic:angezeigt||`` werden. <br>
Um diese zufällige Entscheidung zu programmieren, benötigst du noch eine ``||logic:wenn-dann-Bedingung||``.


## Schritt 1
Hier gibt es erstmal keine Lösung. Am besten du versuchst es erstmal selber.

## Schritt 2
Hier findest du jetzt eine Lösung.
Diese kannst du aber noch stark verbessern.<br>
Dir ist sicher aufgefallen, dass der Schneeball öfter angezeigt wird und die Zuckerstange kaum angezeigt wird. <br>
Kannst du dir vielleicht erklären weshalb? <br>
**Kleiner Tipp:** Um jedem Symbol die gleiche Wahrscheinlichkeit zu geben, erstelle eine Variable namens Zufall. Auf ihr soll eine Zufallszahl zwischen 0 und 2 gespeichert werden. <br>
In die wenn-dann-Bedingungen schiebst du jeweils einen Vergleich mit deiner Variable und den Zahlen 0 bis 2, sodass bei einer "0" der Schneball, bei einer "1" das Rentier und bei einer "2" die Zuckerstange kommt.

```blocks
input.onGesture(Gesture.Shake, function () {
    if (Math.randomBoolean()) {
        basic.showLeds(`
            . # # # .
            # # # # #
            # # # # #
            # # # # #
            . # # # .
            `)
    } else if (Math.randomBoolean()) {
        basic.showLeds(`
            # . # . .
            . # . . .
            # # . . #
            . # # # .
            . # . # .
            `)
    } else if (Math.randomBoolean()) {
        basic.showLeds(`
            . . # # .
            . # . . #
            . . . # .
            . . # . .
            . # . . .
            `)
    }
})
```
