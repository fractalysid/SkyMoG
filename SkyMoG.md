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

>UsePatchSpeedhackWithoutGraphics=true

Now set the *ReservedMemorySize* and *VideoMemorySize* following this [guide](http://wiki.step-project.com/Guide:ENBlocal_INI/Memory)

## Optional Tools
You may want to install these optional tools for troobleshooting (read the guides on the mod's pages on how to use them):

1. [Save game script cleaner](http://www.nexusmods.com/skyrim/mods/52363/?)
2. [TES5Edit](http://www.nexusmods.com/skyrim/mods/25859/?)
3. [Optimizer Textures](http://www.nexusmods.com/skyrim/mods/12801/?)
4. [Skyrim Performance Monitor](http://www.nexusmods.com/skyrim/mods/6491/?)

## Mods

Time to start downloading and installing the mods. You'll be doing this through MO with just a few exceptions.

#### Unoffical Patches
1. [USLEEP](http://www.nexusmods.com/skyrim/mods/71214/?)

#### Textures
Let's start with the textures. You won't need to adjust their order, so it's probably best to install them before anything else. A lot of them will come in different resolutions, it's up to you (depending on your hardware) to decide what version to download. With 2GB of VRAM it'd be better to stand with 1K or at most 2K.

1.
