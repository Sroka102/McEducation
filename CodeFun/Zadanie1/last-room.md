### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Program the Agent to move up to the gold plate!

## Step 1
Zaprogramuj agenta, aby dotarł do złotej płyty. Musisz stać na swojej złotej płycie, podczas gdy Agent musi stanąć na kolejnej. Następnie naciśnij zielony przycisk **Play** aby skompilować kod, przejdź do Minecrafta i uruchom program w grze.


```ghost
player.onChat("last", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
```  