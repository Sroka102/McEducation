### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Surroundings 

## Step 1
Kiedy Agent **wykryje blok w dół**, ma się przesuwać do przodu. Jeśli Agent **skontroluje blok w dół** i wykryje **powietrze**, wtedy niech użyje komendy ``||gracz:powiedz||`` i powie **Znalazłem krater!**. 

```template
player.onChat("crater", function () {
            player.say("Crater found!")
})
```
```ghost
player.onChat("1", function () {
    while (agent.detect(AgentDetection.Block, DOWN)) {
        agent.move(FORWARD, 1)
    }
    if (agent.inspect(AgentInspection.Block, DOWN) == AIR) {
        player.say("Crater found!")
    }
})
```