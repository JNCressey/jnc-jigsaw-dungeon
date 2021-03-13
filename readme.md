This is a datapack for Minecraft Java Edition.

My entry for [r/Minecraft Bi-Weekly Build Challenge #118: Dungeon](https://www.reddit.com/r/Minecraft/comments/luivrb/minecraft_biweekly_build_challenge_118_dungeon/).

<details>
    <summary>To install the datapack into your world:</summary>
    <p>Simply copy the folder <code>./jnc-jigsaw-dungeon/</code> to <code>[world folder]/datapacks/jnc-jigsaw-dungeon/</code>.</p>
    <p>You can open your world folder by these steps:
        <ol>
        <li>Go to the singleplayer world select screen.</li>
        <li>Select your world and click the 'Edit' button.</li>
        <li>Click the 'Open World Folder' button.</li>
        </ol>
    </p>
</details>

The idea behind how I have designed the dungeon, is such that it would feel like it fits in with the vanilla game. E.g. The sophistication of any generated redstone is at a similar level to redstone that is used in existing game structures such as jungle temples.

The dungeon is generated with **jigsaw blocks**. This allows for randomness in the experience of tackling the dungeon, as the jigsaw blocks build up the structure by randomly pulling from structure pools.

# Currently Implemented

## Generate the dungeon starting from the antechamber

<details>
<summary>To generate the dungeon:</summary>
    <p>Place a jigsaw block facing horizontally with jigsaw face towards where the dungeon will go.</p>
    <p>Generate with:</p>
    <ul>
    <li><code>Target Pool</code>: <code>jnc_dungeon:pool_antechamber</code>,</li>
    <li><code>Target Name</code>: <code>jnc_dungeon:in</code>,</li>
    <li><code>Levels</code> to at least <code>3</code>, and</li>
    <li><code>Keep Jigsaws</code>: <code>OFF</code>.</li>
    </ul>
</details>

## An ante-chamber with a button puzzle

The antechamber comes before the entrance to the spawner room. There is a button puzzle to open the door to the dungeon. 

The antechamber either generates with a bonus or a trap. When performing the sequence that first opens the door you can determine whether there is a bonus or a trap.

The bonus is revealed after an extra sequence of button presses. However, simply memorizing the sequence and doing it for every antechamber will trigger the trap when it generates with a trap.

There are two possible traps:

- Lava is released from the ceiling
- The floor opens to a pitfall

## The zombie spawner room.

The zombie spawner room has narrow hallways and paths for zombies to pathfind to behind you. This environment favors the zombie as it attacks with melee. 

The arrangement of the walls, and of chests is randomized.

A possible placement of a trapped chest also sets off TNT in the floor to create a ditch you could have difficulty getting out of while fighting off zombies. 

<details>
<summary>To generate just this room:</summary>
    <p>Place a jigsaw block facing horizontally with jigsaw face towards where the dungeon will go.</p>
    <p>Generate with:</p>
    <ul>
    <li><code>Target Pool</code>: <code>jnc_dungeon:pool_zombie_labyrinth</code>,</li>
    <li><code>Target Name</code>: <code>jnc_dungeon:in</code>,</li>
    <li><code>Levels</code> to at least <code>2</code>, and</li>
    <li><code>Keep Jigsaws</code>: <code>OFF</code>.</li>
    </ul>
</details>

## The skeleton spawner room

The skeleton spawner room is tall with the spawner high up. There is a parkour course for you to get up to disable the spawner. But hits from skeletons' arrows could cause you to fall down.

The structure of bone for the floor above is randomised between ribs, a big bone, and a skull. The parkour course is randomised between a helical course and an S shaped course.

<details>
<summary>To generate just this room:</summary>
    <p>Place a jigsaw block facing horizontally with jigsaw face towards where the dungeon will go.</p>
    <p>Generate with:</p>
    <ul>
    <li><code>Target Pool</code>: <code>jnc_dungeon:pool_skeleton_tower</code>,</li>
    <li><code>Target Name</code>: <code>jnc_dungeon:in</code>,</li>
    <li><code>Levels</code> to at least <code>2</code>, and</li>
    <li><code>Keep Jigsaws</code>: <code>OFF</code>.</li>
    </ul>
</details>

# Planned

## The spider spawner room

The spider spawner room will be clear of obstacles such that the spiders can easily navigate. However, there are many cobweb blocks which slow your movement. 

The cobweb placement is randomized. There may be a twisted path you can take which requires passing through/breaking fewer cobwebs. 