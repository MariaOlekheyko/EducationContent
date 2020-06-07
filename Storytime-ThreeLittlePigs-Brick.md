# Storytime - Three Little Pigs

## Blow the Brick house down

```Code
player.onChat("brick_huff_puff", function () {
    player.say("Woooooooooooossssssssssshhhhhhhh")
    for (let index = 0; index < 350; index++) {
        if (blocks.testForBlock(BRICKS, randpos(
        world(-355, 64, -985),
        world(-345, 70, -978)
        ))) {
            mobs.applyEffect(NAUSEA, mobs.target(NEAREST_PLAYER), 10, 1)
            mobs.applyEffect(WEAKNESS, mobs.target(NEAREST_PLAYER), 10, 1)
        }
    }
})
```
