# Hansel and Gretel Witch Hunt

## Prepare Chat Command

```block
player.onChat("jump", function () {
	
})
```

## Change Chat Command to 'witch_hunters'

```block
player.onChat("witch_hunters", function () {
	
})
```

## Add Kill Nearest Player

```block
player.onChat("witch_hunters", function () {
    mobs.kill(
    mobs.target(NEAREST_PLAYER)
    )
})
```

## Replace Kill Nearest Player with Kill Mob - Animal

```block
player.onChat("witch_hunters", function () {
    mobs.kill(
    mobs.entitiesByType(CHICKEN)
    )
})
```

## Replace Animal with Monster

```block
player.onChat("witch_hunters", function () {
    mobs.kill(
    mobs.entitiesByType(mobs.monster(ZOMBIE))
    )
})
```

## Replace Zombie with Witch

```block
player.onChat("witch_hunters", function () {
    mobs.kill(
    mobs.entitiesByType(mobs.monster(WITCH))
    )
})
```



## All the Code

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
    FIRE,
    world(120, 68, -609),
    world(146, 97, -591)
    )
    blocks.replace(
    AIR,
    NETHERRACK,
    world(120, 68, -609),
    world(146, 97, -591)
    )
    loops.pause(500)
    for (let index = 0; index < 40; index++) {
        blocks.place(CAKE, randpos(
        world(123, 70, -610),
        world(139, 70, -591)
        ))
    }
    for (let index = 0; index < 40; index++) {
        blocks.place(WHITE_TULIP, randpos(
        world(123, 70, -610),
        world(139, 70, -591)
        ))
    }
})

