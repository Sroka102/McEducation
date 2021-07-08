### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @explicitHints 1


# Cattle

## Step 1
Spójrz na kod startowy i spróbuj go uruchomić. Ten kod pozwala na poruszanie Agentem bez liczenia bloków. Przyjrzyj się ścieżce, którą musi przejąć Agent. Upewnij się, że kończysz sekwencję kodowania obrotem Agenta w odpowiednią stronę. Pokieruj tak Agenta, aby dotarł na **złotą płytkę**.  

```template
player.onChat("sheep", function () {
    while (!(agent.detect(AgentDetection.Block, FORWARD))) {
        agent.move(FORWARD, 1)
    }
    agent.turn(LEFT_TURN)
})

``` 

