# Workshop Datapack for Minecraft (2025)

# Part 1: Artefacts

Today we're going to guide you through the creation of your first datapack for Minecraft Java.

In this workshop, you'll learn how to format a pack and how to create custom items in a data-oriented manner.

At the end of this workshop, you should know how to make these kinds of items:

![Charm of the Endermite](doc/CharmOfTheEndermite.png)

![Moon Shoes](doc/MoonShoes.png)

(yep, even the chestplate and the helmet was made using data-oriented items)

## Let's Get The Party Started

We'll assume you already own Minecraft for Java (legally). You can do this Workshop on both Windows, Mac and Linux.

Launch Minecraft in the **lastest version** (1.21.4). This is important since the Datapack formating is reguarly updated.

Create a new world with cheats enabled:

![Allow Commands: ON](doc/CreateNewWorld.png)

## Do It All The Time

Before everything, let's learn about commands. (you'll need them a lot!)

Open your chat, then write `Hello Bob!`. Then, to make it a command, write `/say Hello Bob!` instead.

The `/` is the root of every command. Need more information? Just type `/help say`.

![[Lipatant] Hello Bob!](doc/SayHelloBob.png)

## Creator

Now that you can harness this new power, you'll need to get an item through the use of commands.

If you type `/help give`, the game will answer with `/give <targets> <item> [<count>]`.

The `count` parameter is optional, so we'll leave it empty.

The `item` parameter can be filled with any identifier: you can use, for example, `minecraft:diamond`.

But what about `targets`? Well, here's a little cheat sheet:

| Selector              | Meaning           | Description                               |
| -------------         | -------------     | -------------                             |
| @a                    | All               | All the **players**                       |
| @e                    | Everyone          | All the **entites** (players, mobs...)    |
| @n                    | Nearest           | The nearest **entity**                    |
| @p                    | Player/Proximity  | The nearest **player**                    |
| @r                    | Random            | A random **player**                       |
| @s                    | Self              | The **entity** using the command (you)    |

If you need help more help with that, here's an useful page about selectors [Target selectors](https://minecraft.wiki/w/Target_selectors).

![Gave 1 [Diamond] to Lipatant](doc/GaveDiamond.png)

## It's Going Down Now

We'll learn how to create our datapack.

### **Directory**

You can open the world's folder.

If you don't know where it is, leave your world, go in Singleplayer, then select your world and edit it. You'll be able to click on **Open World Folder**

![Edit](doc/EditWorld.png)

![Open World Folder](doc/OpenWorldFolder.png)

If it still doesn't work, you can go directly to your directory `$env:APPDATA\.minecraft\saves\Workshop\`.

### **Import**

Now that you're in the right folder, go in `datapacks/` and import the given `WorkshopPart1` folder.

If you have troubles, you can consult the following page [Tutorials/Installing a data pack](https://minecraft.wiki/w/Tutorials/Installing_a_data_pack).

### **Testing the pack**

You can now test if everything is working correctly. But before that, use the `/reload` command.

**You'll have to use this command after every change on your code**.

Now, you can use `/datapack list` and check if `[file/WorkshopPart1 (world)]` appears.