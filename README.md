# Day 4 Lumberjack Bot

## Lumberjack Bot

Learn from Sensei about the uses of loops and nesting by teaching the agent how to chop trees for you!

## Listen to Sensei

Sensei will teach you how to make the code, make sure you are following along!

## Activity Complete!

Great job listening to Sensei, now go test your lumberjack bot!

```blocks
player.onChat("chop", function () {
    agent.teleportToPlayer()
    while (agent.detect(AgentDetection.Block, FORWARD)) {
        treeHeight += 1
        if (agent.detect(AgentDetection.Block, UP)) {
            agent.destroy(UP)
        }
        agent.move(UP, 1)
    }
    for (let index = 0; index < treeHeight; index++) {
        agent.move(DOWN, 1)
        agent.destroy(FORWARD)
    }
    agent.collectAll()
})
let treeHeight = 0
treeHeight = 0

```
