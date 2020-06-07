# Storytime - Three Little Pigs

## Blow the Wood house down

```Code
player.onChat("wood_huff_puff", function () {
    player.say("Woooooooooooossssssssssshhhhhhhh")
    for (let index = 0; index < 350; index++) {
        if (blocks.testForBlock(PLANKS_OAK, randpos(
        world(-293, 69, -962),
        world(-298, 74, -952)
        ))) {
            blocks.replace(
            AIR,
            PLANKS_OAK,
            randpos(
            world(-293, 69, -962),
            world(-298, 74, -952)
            ),
            randpos(
            world(-293, 69, -962),
            world(-298, 74, -952)
            )
            )
        }
    }
})
```
