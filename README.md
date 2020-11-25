# Rentier-Schneeball-Zuckerstange
## ~avatar avatar @unplugged
Scheere-Stein-Papier, schön und gut, jetzt kommt Rentier-Schneeball-Zuckerstange.
Wie soll das funktionieren? Ganz einfach!<br>
- Rentier isst Zuckerstange <br>
- Zuckerstange zerteilt Schneeball <br>
- Schneball erschreckt Rentier <br>

## ~@unplugged
Wie funktioniert das Programm? <br>
Wenn der Calliope ``||input:geschüttelt||`` wurde soll ``||math:zufällig||`` ein Schneeball, ein Rentier oder eine Zuckerstange ``||basic:angezeigt||`` werden. <br>
Um diese zufällige Entscheidung zu programmieren benötigst du noch eine ``||logic:wenn-dann-Bedingung||``.


## Schritt 1
Hier gibt es erstmal keine Lösung. Am besten du versuchst es erstmal selber.

## Schritt 2
Hier findest du jetzt eine Lösung
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
