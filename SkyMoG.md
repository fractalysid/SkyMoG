# Skyrim Modding Guide

Well, there won't be a lot of explanations here. Just an ordered (not always) list of mods and a few instructions on how to install them correctly. There will be links, so if you're curious, just click them and quench your thirst for knowledge.

##### Prerequisites
1. RAM >= 4GB
2. VRAM >= 2GB
3. HDD space available >= 60 GB (14 GB Skyrim, 20+-GB Compressed Mods, 35+-GB Installed Mods)

## First Steps
1. Download Skyrim from Steam; English language would be better (it makes sure not to come across translation related bugs).
2. Download and install the latest version of [SKSE](http://skse.silverlock.org/)
3. Download and install [LOOT](https://loot.github.io/)
4. Time to get the Mod Manager [MO](http://www.nexusmods.com/skyrim/mods/1334/?)

## Setting Up MO
I'm not going to explain how to use MO, just what to do with it (maybe I will later on, if I'll be in the right mood to do so):

1. Add LOOT and SKSE (if not already present) as executables.
Always launch the game through MO selecting SKSE.


## Memory Management
Create the file skse.ini in Skyrim/Data/SKSE or in ModOrganizer/overwrite/SKSE and copy the following content:
>[General]

>ClearInvalidRegistrations=1

>[Memory]

>DefaultHeapInitialAllocMB=768

>ScrapHeapSizeMB=256

If the system RAM is 4GB or less you may want to use [Memory Blocks Log](http://www.nexusmods.com/skyrim/mods/50471/?) to find the lowest values for the *Initial Heap Block* and the *ScrapHeapSize*

## ENBoost

The ENB can be set to only use *enbhost.exe* to manage the dynamic memory allocation without applying any graphical effect. This is recommended as Skyrim will likely go out of memory with a lot of mods installed.
If you're going to use an ENB, skip this section, it will be taken care of later. Otherwise, download the latest version of [ENB](http://enbdev.com/download_mod_tesskyrim.htm). Copy the files *d3d9.dll*, *enbhost.exe* and *enblocal.ini* from the Wrapper directory inside the Skyrim directory (where you find the Skyrim binaries). Open enblocal.ini and make sure you have:

>[GLOBAL]  
>UsePatchSpeedhackWithoutGraphics=true  
>
>[MEMORY]  
>ExpandSystemMemoryX64=true  
>ReduceSystemMemoryUsage=true

Now set the *ReservedMemorySize* and *VideoMemorySize* following this [guide](http://wiki.step-project.com/Guide:ENBlocal_INI/Memory)

## Optional Tools
You may want to install these optional tools for troobleshooting (read the guides on the mod's pages on how to use them):

1. [Save game script cleaner](http://www.nexusmods.com/skyrim/mods/52363/?)
2. [TES5Edit](http://www.nexusmods.com/skyrim/mods/25859/?)
3. [Optimizer Textures](http://www.nexusmods.com/skyrim/mods/12801/?)
4. [Skyrim Performance Monitor](http://www.nexusmods.com/skyrim/mods/6491/?)

## Mods

Time to start downloading and installing the mods. You'll be doing this through MO with just a few exceptions.

### Unoffical Patches
1. [USLEEP](http://www.nexusmods.com/skyrim/mods/71214/?)
2. [Unofficial High Resolution Pack](http://www.nexusmods.com/skyrim/mods/31255/?)

### Base Tools, Utilities and Tweaks
1. [Amazing Follower Tweaks](http://www.nexusmods.com/skyrim/mods/15524/?)
3. [Alternate Start](http://www.nexusmods.com/skyrim/mods/9557/?)
4. [A Quality World Map](http://www.nexusmods.com/skyrim/mods/4929/?)
5. [A Matter Of Time](http://www.nexusmods.com/skyrim/mods/44091/?)
6. [ASIS Patcher](http://www.nexusmods.com/skyrim/mods/18436/?)
7. [Better Dialogue Controls](http://www.nexusmods.com/skyrim/mods/27371/?)
8. [Better Message Box Controls](http://www.nexusmods.com/skyrim/mods/28170/?)
9. [Dual Sheat Redux](http://www.nexusmods.com/skyrim/mods/34155/?)
10. [Enhanced Camera](http://www.nexusmods.com/skyrim/mods/57859/?)
11. [SKYUI](http://www.nexusmods.com/skyrim/mods/3863/?)
12. [Extended UI](http://www.nexusmods.com/skyrim/mods/57873/?)
13. [Fuz Roh Doh](http://www.nexusmods.com/skyrim/mods/14884/?)
14. [HDT Physics Extensions](http://www.nexusmods.com/skyrim/mods/53996/?)
15. [Helmet Toggle](http://www.nexusmods.com/skyrim/mods/22765/?)
16. [Improved Closefaced Helmets](http://www.nexusmods.com/skyrim/mods/15927/?)
17. [Jaxon Smart Looter](http://www.nexusmods.com/skyrim/mods/52927/?)
18. [Player Headtracking](http://www.nexusmods.com/skyrim/mods/23600/?)
19. [Realistic Ragdolls and Force](http://www.nexusmods.com/skyrim/mods/601/?)
20. [The Skyrim Distance Overhaul](http://www.nexusmods.com/skyrim/mods/19446/?)
21. [VioLens a Killmove Mod](http://www.nexusmods.com/skyrim/mods/56980/?)
22. [Brawl Bugs Patch](http://www.nexusmods.com/skyrim/mods/24020/?)
23. [Height Adjusted](http://www.nexusmods.com/skyrim/mods/7587/?)
24. [Auto Unequip Ammo](http://www.nexusmods.com/skyrim/mods/10753/?)
25. [Barenziah Quest Marker](http://www.nexusmods.com/skyrim/mods/9385/?)
26. [Unique Items Level Up](http://www.nexusmods.com/skyrim/mods/7590/?)
27. [Dragon Priest Quest Markers](http://www.nexusmods.com/skyrim/mods/22647/?)
28. [Dungeon Quest Awareness](http://www.nexusmods.com/skyrim/mods/9720/?)
29. [Glowing Ore Veins](http://www.nexusmods.com/skyrim/mods/193/?)
30. [Unread Books Glow](http://www.nexusmods.com/skyrim/mods/10012/?)
31. [Faster Horses](http://www.nexusmods.com/skyrim/mods/934/?)
32. [Weapons and Armors Fixes Remade](http://www.nexusmods.com/skyrim/mods/34093/?)
33. [Clothing and Clutter Fixes](http://www.nexusmods.com/skyrim/mods/43053/?)
34. [Complete Crafting Overhaul](http://www.nexusmods.com/skyrim/mods/49791/?)
35. [Acquisitive Soul Gems](http://www.nexusmods.com/skyrim/mods/5312/?)
36. [Think TO Yourself Messages](http://www.nexusmods.com/skyrim/mods/32060/?)

##### Extra
1. [Marriable Serana](http://www.nexusmods.com/skyrim/mods/28685/?)
2. [The Paarthurnax Dilemma](http://www.nexusmods.com/skyrim/mods/18465/?)
3. [DYNAVISION](http://www.nexusmods.com/skyrim/mods/12525/?)
4. [Imaginator](http://www.nexusmods.com/skyrim/mods/13049/?)
5. [FNIS](http://www.nexusmods.com/skyrim/mods/11811/?)
6. [FNIS Sexy Moves](http://www.nexusmods.com/skyrim/mods/54521/?)
7. [FNIS PCEA2](http://www.nexusmods.com/skyrim/mods/71055/?)

### Character Creation
1. [Race Menu](http://www.nexusmods.com/skyrim/mods/29624/?)
2. [Caliente's Beautiful Bodies Edition](http://www.nexusmods.com/skyrim/mods/2666/?)
3. [Apachi SkyHair](http://www.nexusmods.com/skyrim/mods/10168/?)
4. [Female Facial Animations](http://www.nexusmods.com/skyrim/mods/35303/?)
5. [KS Hairdos Renewal](http://www.nexusmods.com/skyrim/mods/68311/?)
6. [Lovely Hairstyles](http://www.nexusmods.com/skyrim/mods/7403/?)
7. [Superior Lore Friendly Hair](http://www.nexusmods.com/skyrim/mods/36510/?)
8. [SG Female Eyebrows](http://www.nexusmods.com/skyrim/mods/35327/?)
9. [Brows](http://www.nexusmods.com/skyrim/mods/30411/?)
10. [The Eyes of Beauty](http://www.nexusmods.com/skyrim/mods/13722/?)
11. [Better Vampires Fangs and Eyes](http://www.nexusmods.com/skyrim/mods/38829/?)
12. [No More Blocky Faces](http://www.nexusmods.com/skyrim/mods/30/?)
13. [Detailed Faces](http://www.nexusmods.com/skyrim/mods/26/?)
14. [Better Females By Bella](http://www.nexusmods.com/skyrim/mods/2812/?)
15. [Better Females By Bella - Natural Edition](http://www.nexusmods.com/skyrim/mods/26113/?)
16. [Smile in HD](http://www.nexusmods.com/skyrim/mods/34346/?)
17. [Better Makeup for SKSE](http://www.nexusmods.com/skyrim/mods/31665/?)
18. [No More Ugly Bronze Shiny](http://www.nexusmods.com/skyrim/mods/71054/?)

### NPCs
1. [Bijin Warmaidens](http://www.nexusmods.com/skyrim/mods/40038/?)
2. [Bijin Wives](http://www.nexusmods.com/skyrim/mods/63473/?)
3. [Bijin NPCs](http://www.nexusmods.com/skyrim/mods/71054/?)
4. [Interesting NPCs](http://www.nexusmods.com/skyrim/mods/8429/?)
5. [Inconsequential NPCs](http://www.nexusmods.com/skyrim/mods/36334/?)

### Weapons
1. [Immersive Weapons](http://www.nexusmods.com/skyrim/mods/27644/?)
2. [LOTR Weapons](http://www.nexusmods.com/skyrim/mods/5727/?)

### Armors
1. [Caliente's Vanilla Outfits](http://www.nexusmods.com/skyrim/mods/12273/?)
2. [Immersive Armors](http://www.nexusmods.com/skyrim/mods/19733/?)
3. [Cloaks of Skyrim](http://www.nexusmods.com/skyrim/mods/12092/?)

##### Extra
1. [nsk13's Armors](http://www.nexusmods.com/skyrim/users/3373573/?tb=mods&pUp=1)
2. [Dark BrotherHood Shrouded Armor](http://www.nexusmods.com/skyrim/mods/39964/?)
3. [Tribunal Robes and Masks](http://www.nexusmods.com/skyrim/mods/20077/?)
4. [Whatever you like](http://www.nexusmods.com/skyrim/mods/searchresults/?src_cat=54)

### Creatures
1. [Skyrim Immersive Creatures](http://www.nexusmods.com/skyrim/mods/24913/?)
2. [SkyTEST - Realistic Animals and Predators](http://www.nexusmods.com/skyrim/mods/10175/?)
3. [Bellyaches New Dragon Species](http://www.nexusmods.com/skyrim/mods/20889/?)
4. [Deadly Dragons](http://www.nexusmods.com/skyrim/mods/3829/?)

### Expansions and Quests
1. [Falskaar](http://www.nexusmods.com/skyrim/mods/37994/?)
2. [Wyrmstooth](http://www.nexusmods.com/skyrim/mods/25704/?)
3. [The Forgotten City](http://www.nexusmods.com/skyrim/mods/70219/?)
4. [The Gray Cowl of Nocturnal](http://www.nexusmods.com/skyrim/mods/64651/?)
5. [Amorous Adventures](http://www.nexusmods.com/skyrim/mods/70495/?)
6. [The Notice Board](http://www.nexusmods.com/skyrim/mods/70142/?)

##### Extra
1. [Better Falskaar and Wyrmstooth Maps ](http://www.nexusmods.com/skyrim/mods/51339/?)

### Locations
1. [Dark BrotherHood Reborn](http://www.nexusmods.com/skyrim/mods/20700/?)
2. [Immersive College of Winterhold](http://www.nexusmods.com/skyrim/mods/36849/?)
3. [Nightingale Hall and Sepulcher Improved](http://www.nexusmods.com/skyrim/mods/34743/?)
4. [Skyforge Plus](http://www.nexusmods.com/skyrim/mods/54544/?)
5. [BreezeHome Fully Upgradable](http://www.nexusmods.com/skyrim/mods/11158/?)


####To order
1. [Campfire](http://www.nexusmods.com/skyrim/mods/64798/?)
2. [Frostfall](http://www.nexusmods.com/skyrim/mods/11163/?)

### Meshes
1. [Ruins Clutter Improved](http://www.nexusmods.com/skyrim/mods/14227/?)
2. [Static Mesh Improvements Mod](http://www.nexusmods.com/skyrim/mods/8655/?)

##### Extra
1. [xp32 Maximum Skeleton](http://www.nexusmods.com/skyrim/mods/26800/?)


#### Textures
Let's start with the textures. You won't need to adjust their order, so it's probably best to install them before anything else. A lot of them will come in different resolutions, it's up to you (depending on your hardware) to decide what version to download. With 2GB of VRAM it'd be better to stand with 1K or at most 2K.

1. [Skyrim HD 2K](http://www.nexusmods.com/skyrim/mods/607/?)
2. [SkyRealism - Shiny](http://www.nexusmods.com/skyrim/mods/48526/?)
3. [aMidianBorn Book of Silence](http://www.nexusmods.com/skyrim/mods/24909/?)
4. [Bellyaches Animal and Creatures Pack](http://www.nexusmods.com/skyrim/mods/3621/?)
5. [Bellyaches HD Dragon Replacer Pack](http://www.nexusmods.com/skyrim/mods/29631/?)
6. [Better Circlets](http://www.nexusmods.com/skyrim/mods/6495/?)
7. [Bloody Dragon Bones](http://www.nexusmods.com/skyrim/mods/30620/?)
8. [CoverKhajits](http://www.nexusmods.com/skyrim/mods/5941/?)
9. [More Dramatic Alduin](http://www.nexusmods.com/skyrim/mods/54070/?)
10. [Enhanced Blood Textures](http://www.nexusmods.com/skyrim/mods/60/?)
11. [Enhanced Night Skyrim](http://www.nexusmods.com/skyrim/mods/85/?)
12. [HQ Food and Ingredients](http://www.nexusmods.com/skyrim/mods/1192/?)
13. [Improved NPC Clothing](http://www.nexusmods.com/skyrim/mods/2674/?)
14. [Real Ice](http://www.nexusmods.com/skyrim/mods/5388/?)
15. [REN's HD Shrines](http://www.nexusmods.com/skyrim/mods/50327/)
16. [Rustic Windows](http://www.nexusmods.com/skyrim/mods/54302/?)
17. [Septim HD](http://www.nexusmods.com/skyrim/mods/3018/?)
19. [Dawnguard Fortress Improved](http://www.nexusmods.com/skyrim/mods/32809/?)
20. [Ultimate HD Torch](http://www.nexusmods.com/skyrim/mods/28060/?)
21. [Unique Dragon Priests Masks](http://www.nexusmods.com/skyrim/mods/35117/?)
22. [Dust Effects](http://www.nexusmods.com/skyrim/mods/44201/?)
23. [Detailed Rugs](http://www.nexusmods.com/skyrim/mods/29608/?)
24. [Ultimate HD Fire Effect](http://www.nexusmods.com/skyrim/mods/28642/?) OR [Cinematic Fire Effect](http://www.nexusmods.com/skyrim/mods/2692/?)
25. [Realistic Smoke And Embers](http://www.nexusmods.com/skyrim/mods/836/?)

##### Extra
1. [Footprints](http://www.nexusmods.com/skyrim/mods/22745/?)
2. [LOTR Weapons Retextures](http://www.nexusmods.com/skyrim/mods/29730/?)
3. [Realistic HD Mushrooms](http://www.nexusmods.com/skyrim/mods/61289/?)
4. [Realistic HD Ores](http://www.nexusmods.com/skyrim/mods/60340/?)
5. [Rustic Clutter Collection](http://www.nexusmods.com/skyrim/mods/62506/?)
6. [Rustic Potions and Poisons](http://www.nexusmods.com/skyrim/mods/62701/?)
7. [Rustic Alchemy and Enchanting Table](http://www.nexusmods.com/skyrim/mods/62328/?)
8. [Rustic Soulgems](http://www.nexusmods.com/skyrim/mods/63766/?)
9. [Rustic Clothing](http://www.nexusmods.com/skyrim/mods/69784/?)
10. [Night Mother HD](http://www.nexusmods.com/skyrim/mods/4947/?)
11. [The Notice Board Retexture](http://www.nexusmods.com/skyrim/mods/70260/?)

###### Parallax
1. [Tamriel Reloaded](http://www.nexusmods.com/skyrim/mods/46925/?)
2. [Project Parallax Remastered](http://www.nexusmods.com/skyrim/mods/40512/?)
3. [4K Parallax Treebark](http://www.nexusmods.com/skyrim/mods/61875/?)

##### Install These After Skyrim Flora Overhaul
1. [Unique Grasses and GroundCovers](http://www.nexusmods.com/skyrim/mods/42370/?)
2. [aMidianBorn Landscape](http://www.nexusmods.com/skyrim/mods/37865/?)
3. [aMidianBorn Solstheim Landscape](http://www.nexusmods.com/skyrim/mods/50013/?)
4. [Vivid Landscapes](http://www.nexusmods.com/skyrim/mods/49344/?)
5. [Quality Snow](http://www.nexusmods.com/skyrim/mods/49011/?)
6. [High Definition Ivy](http://www.nexusmods.com/skyrim/mods/30971/?)
7. [HD Plants and Herbs](http://www.nexusmods.com/skyrim/mods/1546/?)

### Environmental
1. [Skyrim Flora Overhaul](http://www.nexusmods.com/skyrim/mods/141/?)
2. [Verdant Grass Plugin](http://www.nexusmods.com/skyrim/mods/60220/?) OR [Grass On Steroids](http://www.nexusmods.com/skyrim/mods/33582/?) OR [Grass Field](http://www.nexusmods.com/skyrim/mods/50875/?)
3. [Skyfalls and Skymills](http://www.nexusmods.com/skyrim/mods/40564/?)
4. [Lanterns of Skyrim](http://www.nexusmods.com/skyrim/mods/18916/?)
5. [Wonders of Weather](http://www.nexusmods.com/skyrim/mods/64941/?)
6. [Pure Waters](http://www.nexusmods.com/skyrim/mods/1111/?)

### Cities
1. [TaVE Whiterun](http://www.nexusmods.com/skyrim/mods/19799/?)
2. [TaVE Riften](http://www.nexusmods.com/skyrim/mods/20185/?)
3. [TaVE Solitude](http://www.nexusmods.com/skyrim/mods/21148/?)
4. [TaVE Windhelm](http://www.nexusmods.com/skyrim/mods/22608/?)
5. [LoS and TaVE Villages](http://www.nexusmods.com/skyrim/mods/27395/?)

### Weather
TODO: Add detailed descriptions on the installation of these mods
1. [Climates of Tamriel v3.1](http://www.nexusmods.com/skyrim/mods/17802/?)
2. [Expanded Snow System](http://www.nexusmods.com/skyrim/mods/28110/?)
3. [Supreme and Volumetric Fog](http://www.nexusmods.com/skyrim/mods/24460/?)
4. [Supreme Storms](http://www.nexusmods.com/skyrim/mods/27022/?)
5. [Climates of Tamriel - Weather Patch](http://www.nexusmods.com/skyrim/mods/39799/?)
6. [Realistic Nights](http://www.nexusmods.com/skyrim/mods/49472/?)

### Visual and Graphics
1. [Smoking Torches and Candles](http://www.nexusmods.com/skyrim/mods/35819/?)
2. [Better Torches](http://www.nexusmods.com/skyrim/mods/27443/?)
3. [Wet And Cold](http://www.nexusmods.com/skyrim/mods/27563/?)
4. [Enhanced Lights and FX](http://www.nexusmods.com/skyrim/mods/27043/?) OR [Realistic Lighting Overhaul](http://www.nexusmods.com/skyrim/mods/30450/?)

### Visual and Performance Fixes
1. [Skyrim Performance Plus](http://www.nexusmods.com/skyrim/mods/6387/?)
2. [Remove Underwater Grass](http://www.nexusmods.com/skyrim/mods/55240/?)
3. [Distant Decal Fix](http://www.nexusmods.com/skyrim/mods/32426/?)
4. [Revamped Exterior Fog](http://www.nexusmods.com/skyrim/mods/9930/?)
5. [Skyrim Projext Optimization](http://www.nexusmods.com/skyrim/mods/32505/?)

### Sound
TODO: Add infos. Eg. Install the SoS patches for Cot.
1. [SoS - The Wilds](http://www.nexusmods.com/skyrim/mods/10886/?)
2. [SoS - The Dungeons](http://www.nexusmods.com/skyrim/mods/8601/?)
3. [SoS - Civilization](http://www.nexusmods.com/skyrim/mods/20193/?)
4. [Audio Overhaul for Skyrim](http://www.nexusmods.com/skyrim/mods/43773/?)
5. [Immersive Sounds - Compendium](http://www.nexusmods.com/skyrim/mods/54387/?)
6. [Better Animals Footsteps](http://www.nexusmods.com/skyrim/mods/24805/?)
7. [Hearth of the Beast - WereWolves Sounds and Textures](http://www.nexusmods.com/skyrim/mods/13779/?)

##### Extra
1. [Fantasy Soundtrack Project](http://www.nexusmods.com/skyrim/mods/46518/?)
2. [Celtic Music in Skyrim](http://www.nexusmods.com/skyrim/mods/53689/?)

## Gameplay

### Miscellaneous
1. [More Dragon Loot](http://www.nexusmods.com/skyrim/mods/10050/?)
2. [OBIS](http://www.nexusmods.com/skyrim/mods/31264/?)
3. [WarZones 2015](http://www.nexusmods.com/skyrim/mods/9494/?)
4. [Realistic Room Rental](http://www.nexusmods.com/skyrim/mods/25029/?)
5. [Trade and Barter](http://www.nexusmods.com/skyrim/mods/34612/?)
6. [Hunting in Skyrim](http://www.nexusmods.com/skyrim/mods/18866/?)
7. [The Hunting Game](http://www.nexusmods.com/skyrim/mods/45724/?)
8. [Hunterborn](http://www.nexusmods.com/skyrim/mods/33201/?)
9. [Realistic Needs and Disease](http://www.nexusmods.com/skyrim/mods/26228/?) OR [iNeed](http://www.nexusmods.com/skyrim/mods/51473/?)
10. [Sneak Tools](http://www.nexusmods.com/skyrim/mods/19447/?)
11. [Wearable Lanterns](http://www.nexusmods.com/skyrim/mods/17416/?)

### Combat and Difficulty mods
1. [Combat Evolved](http://www.nexusmods.com/skyrim/mods/56147/?)
2. [Duel Combat Realism](http://www.nexusmods.com/skyrim/mods/2700/?)
3. [Revenge of the Enemies](http://www.nexusmods.com/skyrim/mods/40491/?)

### Perks and Magic
1. [Spectraverse](http://www.nexusmods.com/skyrim/mods/53780/?)
2. [Dwemertech](http://www.nexusmods.com/skyrim/mods/56037/?)
3. [Wintermyst](http://www.nexusmods.com/skyrim/mods/58635/?)
4. [Aurora](http://www.nexusmods.com/skyrim/mods/29311/?)
5. [Imperious](http://www.nexusmods.com/skyrim/mods/61218/?)
6. [Thunderchild](http://www.nexusmods.com/skyrim/mods/41376/?)
7. [Skyrim Community Uncapper](http://www.nexusmods.com/skyrim/mods/1175/?)
8. [Ordinator](http://www.nexusmods.com/skyrim/mods/68425/?)
9. [Uncapper for Ordinator](http://www.nexusmods.com/skyrim/mods/68720/?)
10. [Apocalypse](http://www.nexusmods.com/skyrim/mods/16225/?)
11. [More Apocalypse](http://www.nexusmods.com/skyrim/mods/65527/?)
12. Apocalypse Ordinator Patch (in the Apocalypse Page)
13. [Forgotten Magic Redone](http://www.nexusmods.com/skyrim/mods/35339/?)

## ENB
