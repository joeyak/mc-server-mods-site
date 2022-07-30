<script>
/* My Stuff */
  let startDate = new Date(Date.UTC(2022, 6, 16, 19, 0, 0));
  let netherDate = new Date(startDate);
  let endDate = new Date(startDate);

  netherDate.setDate(netherDate.getDate() + 4);
  netherDate.setHours(netherDate.getHours() + 2);
  endDate.setDate(endDate.getDate() + 14);

  setInterval(() => {
    fetch("https://raw.githubusercontent.com/mckamey/countdownjs/master/countdown.js")
        .then(res => res.text())
        .then(txt => {
            var js = document.createElement("script");
            js.textContent = txt;

            document.head.appendChild(js);
        })
        .then(_ => {
          let now = new Date();
          document.getElementById("timeStart").innerText = now < startDate ? countdown(startDate).toString() : "Live!";
          document.getElementById("timeNether").innerText = now < netherDate ? countdown(netherDate).toString() : "Live!";
          // document.getElementById("timeEnd").innerText = now < endDate ? countdown(endDate).toString() : "Live!";
        });
  }, 1000)
</script>

<style>
  img {
    width: 400px;
  }
</style>

# AzaleaPlays Server Info

Url: `mc.azaleaplays.com`

## Dates

### Server Start: <span id="timeStart"></span>

### Enter the Nether: <span id="timeNether"></span>

### Enter the End: <span id="timeEnd">TBD</span>

## Table of contents

* [Server Side Mods](#server-side-mods)
* [Datapacks](#datapacks)
* [Suggested Client Side Mods](#suggested-client-side-mods)
* [Custom Recipes](#custom-recipes)

## Server Side Mods

### [Copper Hopper](https://www.curseforge.com/minecraft/mc-mods/copper-hopper)

* Hopper Item Filtering

### [DeathLog](https://www.curseforge.com/minecraft/mc-mods/deathlog)

* Shows information on your deaths

### [Simple Voice Chat](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat)

* Allows proximity voice chat
* Client side required (server can be joined without this mod though)

## Datapacks

### [Terralith](https://www.curseforge.com/minecraft/mc-mods/terralith)

* Overworld Terrain Generation

### [Incendium](https://www.curseforge.com/minecraft/mc-mods/incendium)

* Nether Terrain Generation

### [Nullscape](https://www.curseforge.com/minecraft/mc-mods/nullscape)

* End Terrain Generation

### [Structory](https://www.curseforge.com/minecraft/mc-mods/structory)

* Adds a variety of structures

### [Towns and Towers - Structure Add-on](https://www.curseforge.com/minecraft/mc-mods/towns-and-towers-structure-add-on)

* Add more villages, outposts, and Terralith structures

### [Vanilla Tweaks](https://vanillatweaks.net/picker/datapacks/)

* Armor Statues - Can make Armor Statues change potition and hold items - [video](https://www.youtube.com/watch?v=nV9-_RacnoI)
* Custom Nether Portals - Nether portals can have different shapes now - [video](https://www.youtube.com/watch?v=WfqUtUhI7qM)
* Double Shulker Shells - Killing a shulker will give 2 shells - [video](https://www.youtube.com/watch?v=lfcwKXhjC9Y&t=319s)
* Track Raw Statistics - Stats tracking
* Track Statistics - More stats tracking

## Suggested Client Side Mods

The server uses the [Fabric Mod Loader](https://fabricmc.net/use/)

A curseforge profile with the suggested mods and the server pre added can be found [here](https://www.azaleaplays.com/minecraft/curseforge-profiles/Brooke%20Server%20Summer%202022-1.0.zip)

The mods in the profile are summarized below

### [Simple Voice Chat](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat)

* Allows proximity voice chat
* Version [1.19-2.2.45](https://www.curseforge.com/minecraft/mc-mods/simple-voice-chat/files/3825854) is required
* Is compatible with Sound Physics Remastered

### [Better Recipe Books](https://www.curseforge.com/minecraft/mc-mods/brb)

* Adds some quality of life changes to the recipe book

### [Chat Heads](https://www.curseforge.com/minecraft/mc-mods/chat-heads)

* Shows players head next to chat message

### [Crowmap](https://www.curseforge.com/minecraft/mc-mods/crowmap)

* Updates map in inventory instead of having to hold it

### [DeathLog](https://www.curseforge.com/minecraft/mc-mods/deathlog)

* DeathLog tracks your deaths in all worlds and servers

### [Inventory Sorting](https://www.curseforge.com/minecraft/mc-mods/inventory-sorting)

* Adds multiple ways to sort inventories

### [Iris Shaders](https://www.curseforge.com/minecraft/mc-mods/irisshaders)

* Shaders mod that works with sodium

### [Sodium](https://www.curseforge.com/minecraft/mc-mods/sodium)

* Increases framerate and reduces microstutters

### [ShulkerBox Tooltip](https://www.curseforge.com/minecraft/mc-mods/shulkerboxtooltip)

* Shows preview of what's inside shulker boxes

### [Sound Physics Remastered](https://www.curseforge.com/minecraft/mc-mods/sound-physics-remastered)

* Adds physics to sounds
* Works with Simple Voice Chat

### [Spyglass Improvments](https://www.curseforge.com/minecraft/mc-mods/spyglass-improvements)

* Adds various functionality and improvements to the vanilla minecraft spyglass

### Brooke's Favorite Shaders

* [Complementary](https://www.complementary.dev/)
* [Slidurs Vibrant Shaders](https://sildurs-shaders.github.io/)

## Custom Recipes

These recipes were pulled from [vanillatweaks](https://vanillatweaks.net/picker/crafting-tweaks/)

![Unpackable Wool](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/unpackable%20wool.png?v2)

![Unpackable Ice](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/unpackable%20ice.png?v2)

![Unpackable Nether Wart](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/unpackable%20nether%20wart.png?v2)

![Craftable Bundles Leather](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/craftable%20bundles%20leather.png?v2)

![Craftable Name Tags](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/craftable%20name%20tags.png?v2)

![Craftable Blackstone](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/craftable%20blackstone.png?v2)

![Craftable Horse Armor](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/craftable%20horse%20armor.png?v2)

![Rotten Flesh to Leather](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/rotten%20flesh%20to%20leather.png?v2)

![Dropper to Dispenser](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/dropper%20to%20dispenser.png?v2)

![Blackstone Cobblestone](https://vanillatweaks.net/assets/resources/previews/craftingtweaks/1.19/blackstone%20cobblestone.png?v2)


<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

###### Hi there <3 o/
