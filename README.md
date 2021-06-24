# What this mod does

Modifies projectile's speed, gravity, and impact force to give arrows a more realistic feeling.
All values are based on real-life archery equipment performance, then scaled up slightly to improve gameplay.

Also patches a number of bugs in vanilla projectile records, which are not included in other similar mods, such as:
arrows randomly alerting NPCs even when far away or behind a wall,
ragdolls/objects over-reacting to projectile impacts,
missing sound effects for both arrows and bolts,
and the ballista traps in Dwemer ruins sucking.


The installer includes 6 different physics presets, which each have addons to carry over changes to mod-added projectiles.
(See the bottom of this page, or the installer, for details on each preset)
All files are flagged as .esl, merge instructions are in the readme.
Can be added, removed, swapped, or modified at any time!



# Why use this over other archery mods?

I've used many different archery mods but never felt satisfied with the results.
Projectiles were either too slow, too fast, had too little, or too much gravity. None of them had different presets to choose from, severely limiting players who don't use the same play-style as the mod author. None of them fixed the numerous bugs & inconsistencies present in the vanilla projectile records (Not even USSEP or WACCF!), and most of them didn't support projectiles added by other mods. After attempting to play a stealth archer and encountering seemingly random detection AI, arrows falling at my feet even with a fully charged bow, arrows bouncing off of thin air, and a whole host of other bugs, I decided to make my own archery mod.

First, I used xEdit to check the values & flags used by the game engine. Unfortunately, all of the distance/speed/gravity/force records are measured in "Units", an arbitrary unit of measurement with no easy methods to convert to real-life measurements. No conversion methods were available, and Bethesda's own CK conversion chart is very limited, much less a calculator-style automatic converter. So I decided to make my own. The results exceeded my expectations, allowing me to quickly and accurately convert real-life measurement units to in-game ones.
(The tool is available on my Github﻿ page along with source code)

As a result, I wasn't forced to rely on flat-increases, arbitrary percentages, or multipliers combined with trial-and-error methods, instead able to quickly and accurately (to within 0.001), modify projectile physics to act like real arrows and real bolts.
Another benefit from my conversion tool is the ability for users to quickly and accurately modify projectile physics (or any other kind of mod) to fit any playstyle! Combined with Automation Tools xEdit scripts, I can patch an entire expansion-sized mod in <5 minutes.

A guide on how to modify the physics values is available under "Misc Files"
(Feel free to make requests for addons, physics tweaks, etc. in the comments!)



## Compatibility


    Compatible / No Conflicts:
    (Patches are included in FOMOD)
    Requiem﻿ (Conversion Guide)﻿
    Archery Gameplay Overhaul﻿
    Beyond Skyrim: Bruma﻿
    Immersive Weapons﻿
    Ordinator - Perks of Skyrim﻿
    Skyrim Spear Mechanic﻿
    Shenk Thievery Overhaul﻿
    Sneak Tools
    ﻿Sunnies Tracer Arrows﻿
    Torch Arrows﻿
    All mesh/texture replacers
    (Some model replacers may require patching in xEdit.)

    Semi-Incompatible:
    ABT - Arrows and Bolts Tweaks SE
    The .esp file is incompatible, but the meshes are recommended

    Incompatible:
    Archery﻿
    Archery Tweaks﻿





# Physics Presets
In order of difficulty

### No-Gravity
Completely removes all gravity from projectiles. For people who want a laser rifle.
Arrows: (Gravity = 0.0, Speed = 6900)
Bolts: (Gravity = 0.0, Speed = 7300)

### Arcade-Style
Based on the "Modern" version, but with much less gravity. For people who don't like aiming up.
Arrows: (Gravity = 0.5, Speed = 6900)
Bolts: (Gravity = 0.5, Speed = 7300)

### Modern
Based on modern archery equipment. For people who don't like leading targets.
Arrows: (Gravity = 0.8, Speed = 6900)
Bolts: (Gravity = 0.8, Speed = 7300)

### Realistic-Lite
Based on "Realistic", but with slightly faster projectiles. This is the new default.
Arrows: (Gravity = 0.44, Speed = 5000)
Bolts: (Gravity = 0.44, Speed = 5800)

### Realistic
Based on the performance of actual medieval archery equipment.
Arrows: (Gravity = 0.4, Speed = 4300)
Bolts: (Gravity = 0.4, Speed = 4800)

### Requiem
(Requires Requiem SE)
Based on Requiem's modified archery physics, this version's goal is to fix vanilla projectile record bugs while making bows more predictable.
Arrows: (Gravity = 0.884, Speed = 4300)
Bolts:(Gravity = 0.84, Speed = 5000)


You can also make your own presets using my mod as a base, there is a tutorial available under Misc Files.
You have permission to upload them to the nexus with (brief) credit.
