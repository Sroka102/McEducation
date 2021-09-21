### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Zaprogramuj Agenta, aby przesuna sie w gure na zlota plytę!

## Step 1
Uzyj polecenia``||player:przy poleceniu czatu||`` i  ``||agent:agent przesun||`` aby zaprogramowac Agenta tak, aby poruszal sie w kierunku zlotej plyty. Mozesz zaprogramowac Agenta, aby poruszal sie w **gore**.  Nastepnie nacisnij zielony przycisk **Play** aby skompilowac kod, przejdz do Minecrafta i uruchom program w grze.



```ghost
player.onChat("up", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})

```  
