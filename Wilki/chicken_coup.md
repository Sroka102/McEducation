### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Zagroda dla kurczaków

## Step 1
Agent musi wybudować **2** warstwy ogrodzenia z **żelaznej kraty**. Budując warstwę utwóż **4** ściany o długości **9** bloków każda. Nie zapomnij użyć komendy``||agent:agent przesuń w górę||``przed zbudowaniem drugiego poziomu.

#### ~ tutorialhint
Końcowy kod będzie miał **3** komendy ``||loops:powtórz|`` zagnieżdżone jedna w drugiej. Upewnij się, że Agent będzie miał wystarczającą ilośc bloków w swoim ekwipunku. Do wybudowania całości potrzeba więcej niż 64 bloki żelaznej kraty!

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
