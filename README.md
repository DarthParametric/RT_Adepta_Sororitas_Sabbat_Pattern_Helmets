#  Adepta Sororitas Sabbat-Pattern Helmets
A mod for Owlcat's Rogue Trader cRPG. Adds several Sabbat-pattern helmets for Argenta (or mod-added Sororitas background RTs) throughout the game.

***N.B.: As of patch 1.4.0.195, Owlcat have officially added the pre-release Sabbat-pattern helmet. Some consider this mod overpowered, so stick with the vanilla one if all you want is a fancy hat.***

## Overview
This mod adds the familiar Sabbat-pattern helmet employed by the Adepta Sororitas. Owlcat did initially showcase Argenta wearing one in the pre-release trailers, but for whatever reason this was removed and no longer exists in the game files. This is a new model made by me (although a hooded version uses one of Owlcat's hood models).

The mod contains four helmets. The first two - the standard base version and a hooded Celestian version - are available in chapters 2 and 4, respectively, via the Drusian vendor. The remaining two are paired with Argenta's mutually exclusive quest armours, available at the very end of chapter 4 at the conclusion of her quest. Additionally, this mod makes a minor tweak to the final cutscene/conversation of this quest to ensure that Argenta actually equips the armour and helmet she gains.

## Installation
This is an Owlmod, made using the Unity template supplied by Owlcat. Currently the game has a bug that prevents Owlmods from working. To fix this, you ***must*** install the Unity Mod Manager-based mod [MicroPatches](https://github.com/microsoftenator2022/MicroPatches/releases) by microsoftenator2022. You can install it manually or via [ModFinder](https://github.com/CasDragon/ModFinder/releases/latest).

To install this mod, first make sure you have run the game at least once. Download the [latest release](https://github.com/DarthParametric/RT_Adepta_Sororitas_Sabbat_Pattern_Helmets/releases/latest) or get it from [Nexus Mods](https://www.nexusmods.com/warhammer40kroguetrader/mods/178) and extract it into:

%LocalAppData%Low\Owlcat Games\Warhammer 40000 Rogue Trader\Modifications\
Each Owlmod needs to be in its own sub-folder in the Modifications folder.

Afterwards, you need to edit OwlcatModificationManagerSettings.json in the base Warhammer 40000 Rogue Trader folder in a text editor (Notepad++ recommended). It should look something like this:

```
{
"$id": "1",
"SourceDirectories": [],
"EnabledModifications": ["DPAdeptaSororitasSabbatHelmet"],
"ActiveModifications": ["DPAdeptaSororitasSabbatHelmet"],
"DisabledModifications": []
}
```

If you have other mods, list them in quotes separated by commas. For example:

```
"EnabledModifications": ["DPAdeptaSororitasSabbatHelmet", "ModName2", "ModName3"],
"ActiveModifications": ["DPAdeptaSororitasSabbatHelmet", "ModName2", "ModName3"],
```

You can move individual mods from the ActiveModifications section to the DisabledModifications section if you want to disable them without physically removing them.

Alternatively, use [ModFinder](https://www.nexusmods.com/warhammer40kroguetrader/mods/146) to install the mod.

It should be fine to install the mod in an existing game at any point right up to completing Argenta's quest in chapter 4 (or after if you're willing to use Toybox to manually spawn the helmets).

## Known Issues
Additional localisation support has been added for non-English languages, but these have mostly been machine translated aside from those noted below. Expect errors and terrible/nonsensical grammar.

This mod creates a save dependency! You won't be able to load a save that used it if you later uninstall the mod.

With the engine version change in the v1.5 update, Owlcat broke the modding pipeline. This caused a few issues, amongst them custom body part assets being unloaded, resulting in characters turning invisible. See the [pinned comment](https://www.nexusmods.com/warhammer40kroguetrader/mods/178?tab=posts) on the Nexus Mods page for a workaround if you are still using an older version of the mod.

The mod will be incompatible with any other mod that edits the CommandAction9 and CommandAction10 blueprints for the Argenta_Q2_ArgentaReturn_KTC cutscene. It's an unfortunate limitation of the way Owlmod blueprint patches work. It will probably also break (at least until I update it) if Owlcat patch those blueprints or otherwise alter the scene at some point to fix the vanilla bug.

## Acknowledgements
Many thanks to the modders on the Owlcat Dicord, but particularly microsoftenator2022 and Kurufinve, for helping to coach me through my ineptitude in order to get the mod working.

Chinese localisation kindly supplied by Komoechan.
