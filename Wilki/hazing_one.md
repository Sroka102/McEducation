
### @hideIteration false 
### @flyoutOnly 1
### @explicitHints 1


# Hazing One

## Step 1
Ustaw w komendzie``||agent:umieść blok lub przedmiot||`` **linka potykacza** i ustaw ilość na **64**. 

## Step 2
Użyj ``||pętle:dopóki||`` i umieść z nim odpowiedni blok warunku.  

#### ~ tutorialhint

```blocks
player.onChat("hazing", function () {
    agent.setItem(TRIPWIRE, 64, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
    	
    }
})

``` 
## Step 3
Dodaj komendy ``||agent: agent umieść||`` i ``||agent: agent przesuń||`` wewnątrz ``||pętle:dopuki||``. 

```blocks
player.onChat("run", function () {
    agent.setItem(TRIPWIRE, 64, 1)
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.place(DOWN)
        agent.move(FORWARD, 1)
    }
})
```
