### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Program the Agent to move to the gold plate!

## Step 1
Wybierz polecenie  ``||player: przy poleceniu czatu||``  i zmien nazwe z **run** na **1**. Wybierz blok polecenia  ``||agent: agent przesun do przodu||``  i przeciagnij go do srodka bloku polecenia  ``||player: przy poleceniu czatu||``  . Zmien **liczbe** krokow Agenta na **3**, aby Agent mogl dotrzec do zlotej plyty. Nastepnie nacisnij zielony przycisk **Play** i uruchom kod w grze.

#### ~ tutorialhint 
Mozesz zmienic liczbe krokow, ktore wykona Twoj agent, zmieniajac liczbe w bloku  ``||agent: agent przesun||``  . Mozesz rowniez uzyc bloku  ``||agent: agent obruc||``  aby obrocic Agenta w lewo lub w prawo.



```ghost
player.onChat("1", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
```
