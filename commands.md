

## replace pig with cow

```execute at @e[limit=1, type=minecraft:pig, sort=nearest] summon minecraft:cow as @e[limit=1, type=minecraft:pig, sort=nearest] run kill @s```

## Remove the porkchop (except in nether)

```execute at @e[type=minecraft:item, nbt={Item:{id:"minecraft:porkchop"}}] as @e[type=minecraft:item, nbt={Item:{id:"minecraft:porkchop"}}] unless dimension minecraft:the_nether run kill @s```

## Replace porkchop with beef in nether

```execute at @e[type=minecraft:item, nbt={Item:{id:"minecraft:porkchop"}}] as @e[type=minecraft:item, nbt={Item:{id:"minecraft:porkchop"}}] if dimension minecraft:the_nether run data modify entity @s Item.id set value "minecraft:beef"```
```execute at @e[type=minecraft:item, nbt={Item:{id:"minecraft:porkchop"}}] as @e[type=minecraft:item, nbt={Item:{id:"minecraft:porkchop"}}] if dimension minecraft:the_nether run data modify entity @s Item.id set value "minecraft:beef"```

