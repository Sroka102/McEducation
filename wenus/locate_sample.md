### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Locate the Sample! 

## Step 1
**Dpouki** Agent **skontroluje blok w dole** i **nie** znajdzie **niebieskiego lodu**, ma wykonać **zniszcz w dół** i **przesuń w dół**. Kiedy Agent znajdzie **niebieski lód**, ma go **zniszczyć dół** i **zebrać** próbki. 

```ghost 
player.onChat("ice", function () {
    while (agent.inspect(AgentInspection.Block, DOWN) != ICE) {
        agent.destroy(DOWN)
        agent.move(DOWN, 1)
    }
    agent.destroy(DOWN)
    agent.collectAll()
    
})
```

