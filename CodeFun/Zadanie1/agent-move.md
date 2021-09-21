### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Program the Agent to move to the gold plate!

## Step 1
Wybierz polecenie  ``||player: przy poleceniu czatu||``  i zmień nazwę z **run** na **1**. Wybierz blok polecenia  ``||agent: agent przesuń do przodu||``  i przeciągnij go do środka bloku polecenia  ``||player: przy poleceniu czatu||``  . Zmień **liczbę** kroków Agenta na **3**, aby Agent mógł dotrzeć do złotej płyty. Następnie naciśnij zielony przycisk **Play** i uruchom kod w grze.

#### ~ tutorialhint 
Możesz zmienić liczbę kroków, które wykona Twój agent, zmieniając liczbę w bloku  ``||agent: agent przesuń||``  . Możesz również użyć bloku  ``||agent: agent obruć||``  obrócić Agenta w lewo lub w prawo.



```ghost
player.onChat("1", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
```
