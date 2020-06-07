# Storytime - Jack and the Beanstalk

## Plant Seeds to create the Beanstalk

```block
loops.forever(function () {
    if (blocks.testForBlock(MELON_STEM, world(-441, 68, -860))) {
        blocks.clone(
        world(-441, 90, -1018),
        world(-465, 25, -995),
        world(-451, 68, -874),
        CloneMask.Replace,
        CloneMode.Normal
        )
        player.say("Ooooooops")
    }
})
```