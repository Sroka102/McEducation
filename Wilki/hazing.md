### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Hazing 

## Step 1
Aby wilki tu nie dotarły, Agent musi rozciągnąć **linkę potykacza** między uchwytami. Ustaw w komendzie ``||agent:umieść blok lub przedmiot||`` **linka potykacza** i ustaw ilość na **64**. Użyj ``||pętle:dopóki||`` i umieść w niej warunek.  

#### ~ tutorialhint
Pamiętaj aby użyć **nie** w warunku pętli. 

```blocks
player.onChat("hazing", function () {
    agent.setItem(TRIPWIRE, 64, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
    	
    }
})

``` 
```ghost
player.onChat("hazing", function () {
    agent.setItem(TRIPWIRE, 64, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    }
})
```
