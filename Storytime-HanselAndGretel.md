# Storytime - Hansel and Gretel

## Rid the world of the Witch

```Code
player.onChat("hay_huff_puff", function () {
    player.say("Woooooooooooossssssssssshhhhhhhh")
    for (let index = 0; index < 350; index++) {
        if (blocks.testForBlock(HAY_BLOCK, randpos(
        world(-254, 71, -919),
        world(-260, 76, -910)
        ))) {
            blocks.replace(
            AIR,
            HAY_BLOCK,
            randpos(
            world(-254, 71, -919),
            world(-260, 76, -910)
            ),
            randpos(
            world(-254, 71, -919),
            world(-260, 76, -910)
            )
            )
        }
    }
})
```
