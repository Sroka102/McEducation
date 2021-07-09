### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Chicken Coup

## Step 1
Agent musi umieścić **2** warstwy po **9** bloków **żelaznej kraty** w każdej. Wszystkie **4** ściany muszą być wykonane z **żelaznej kraty**. Nie zapomnij użyć komendy``||agent:agent przesuń w górę||``przed zbudowaniem drugiego poziomu.

#### ~ tutorialhint
Końcowy kod będzie miał **3** komendy ``||loops:powtórz|`` zagnieżdżone jedna w drugiej. Upewnij się, że Agent będzie miał więcej niż 64 bloki w swoim ekwipunku!

```ghost
player.onChat("chicken", function () {
    for (let index = 0; index < 2; index++) {
        agent.setItem(IRON_BARS, 1, 1)
        for (let index = 0; index < 4; index++) {
            for (let index = 0; index < 9; index++) {
                agent.place(DOWN)
                agent.move(FORWARD, 1)
            }
            agent.turn(RIGHT_TURN)
        }
        agent.move(UP, 1)
    }
})

``` 
