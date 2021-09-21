### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Zaprogramuj Agenta, aby przesuną się w gurę na złotą płytę!

## Step 1
Użyj polecenia``||player:przy poleceniu czatu||`` i  ``||agent:agent przesuń||`` abny zaprogramować Agenta tak, aby poruszał się w kierunku złotej płyty. Możesz zaprogramować Agenta, aby się poruszał w **górę**.  Następnie naciśnij zielony przycisk **Play** aby skompilować kod, przejdź do Minecrafta i uruchom program w grze.



```ghost
player.onChat("up", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})

```  
