### @codeStart players set @s makecode 0
### @codeStop players set @s makecode 1

### @hideIteration true 
### @flyoutOnly 1
### @explicitHints 1


# Program the Agent to move up to the gold plate!

## Step 1
W tym zadaniu musicie **Ty** i **Agent** pokonać swój tor i stanąć na płycie. Macie na to 10 sekund od chwili gdy Agent ruszy... Powodzenia!

```ghost
player.onChat("last", function () {
    agent.move(FORWARD, 1)
    agent.turn(LEFT_TURN)
})
```
