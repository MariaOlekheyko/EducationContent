# Storytime - Hansel and Gretel

## Rid the world of the Witch

```block
player.onChat("witch_hunters", function () {
    mobs.kill(
    mobs.entitiesByType(mobs.monster(WITCH))
    )
    blocks.fill(
    AIR,
    world(120, 70, -609),
    world(146, 97, -591),
    FillOperation.Replace
    )
    blocks.replace(
    AIR,
    NETHERRACK,
    world(120, 68, -609),
    world(146, 97, -591)
    )
    blocks.replace(
    AIR,
    FIRE,
    world(120, 68, -609),
    world(146, 97, -591)
    )
    loops.pause(1000)
    for (let index = 0; index < 40; index++) {
        blocks.place(CAKE, randpos(
        world(123, 70, -610),
        world(139, 70, -591)
        ))
        blocks.place(WHITE_TULIP, randpos(
        world(123, 70, -610),
        world(139, 70, -591)
        ))
    }
})
```
## Take a look at this code. What do you think will happen? Run the code once to see. Then return to your code and modify it to replace the white tulips with another type of flower, or replace the cake with another object. 
Remember, once you run this code once, the house will be destroyed! You can still run the code again with your changes, or you can launch a fresh version of this world and modify the code before you run it. 
