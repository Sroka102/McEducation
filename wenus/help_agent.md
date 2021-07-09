### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Iron

## Step 1
Kiedy Agent **skontroluje blok w dole** i nie będzie to **ruda żelaza**, niech się **przesunie do przodu**. Jeśli Agent **wykryje blok z przodu**, niech wykona komendę **zniszcz do przodu**. Jeśli Agent znajdzie żelazo, zaprogramuj go tak aby je **zebrał**. Pamiętj, aby Agent mógł zebrać blok musi go wpierw zniszczyć. 

```ghost
player.onChat("4", function () {
    while (agent.inspect(AgentInspection.Block, DOWN) != IRON_ORE) {
        if (agent.detect(AgentDetection.Block, FORWARD)) {
            agent.destroy(FORWARD)
        }
        agent.move(FORWARD, 1)
    }
    player.say("Found the iron ore!")
    agent.destroy(DOWN)
    agent.collectAll()
})
```
