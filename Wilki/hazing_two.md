### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration false 
### @flyoutOnly 1
### @explicitHints 1


# Hazing Two

## Step 1
Krok 1 to zrobienie drugiej osłony.  

## Step 2
Po zakończeniu naciśnij przycisk **Play**, aby skompilować kod. Nie zapomnij uruchomić kodu w Minecrafcie. 

```blocks
player.onChat("run", function () {
    while (agent.detect(AgentDetection.Block, FORWARD)) {
        agent.destroy(FORWARD)
        agent.move(FORWARD, 1)
        agent.destroy(UP)
    }
})

``` 
