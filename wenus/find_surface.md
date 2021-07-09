### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Reach magma

## Step 1
Zaprogramuj Agenta **przesuń do przodu**. W trakcie niech  **skontroluje** blok w **dół** i jeśli to **nie magma**, wówczas niech Agent się **przesunie w dół**. 


```ghost
player.onChat("magma", function () {
    agent.move(FORWARD, 1)
    while (agent.inspect(AgentInspection.Block, DOWN) != MAGMA_BLOCK) {
        agent.move(DOWN, 1)
    }
})
```

