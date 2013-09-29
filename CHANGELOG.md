Dwarf Fortress from scratch
===========================
_The entirely player-made universe._

Change log
----------

_(Note: This change log is pieced together from notes posted alongside the original release archives. Some entries may be missing or incomplete.)_


### Turn 8 (Putnam)

- Added a few secrets: nigh invulnerability, mastery, insect attacks and knowledge of the creation and metaphysics of the universe.

- Added a semimegabeast--giants--and 2 megabeasts: elements of balance, which take the form of kung-fu halflings and elements of order, which take the form of 4-spheres 8 times as tall as a halfling.

- Added creeping grass and their motile parts.

- Changed the fortressintro and kingarrive files to more creature-neutral ones (subject to change for later; they're still pretty vanilla).

- Added myomorphs, little hamster-like creatures that live in hives and give milk in combs which can be used to make butter and cheese.

- Fixed a few bugs, including:

  - Apple trees not being processed correctly
  - Mamaphints becoming mayor


### Turn 7bis (HugoLuman)

Major bugfix, cleaning things up, mostly overhauling creatures and syndromes to the new classification system. Targetting is now more specific and (hopefully) makes more sense in existing syndromes

**Changes to existing content include:**
-Too many to list
-Occulentibus now targets only Organics
-Garish purple icon for tea plants changed
-Complete reclassification of all creatures
-Lizardfolk blood nerfed, no longer a contact poison
-Panserblekk now war trainable
-Progress triggers added to Halflings, Trolls, Adherents
-Organ tissue is now edible

**New content includes:**
-Adherents of the Mind + Psionic interactions
-Trolls + their taunting interactions
-Mutant Halflings as Night Creatures
-More Cephalopods
-Several marine and aquatic avians


### Turn 7 (Reemer30)

* Added two types of cacti to deserts, the spiny cactus and the Dragon's Tail cactus
* Added a type of fruit to the desert, brewable/edible, and semi-valuable, the heart of the desert
* Added extra ground cover to the Taigas, along with a fern, edible when cooked, and the frost nettle, which was planned for some kind of fireproofing process
* Added snowcaps to the taigas, a wide, tall, white tree-like mushroom to the taigas
* Changed apple tree spawning to temperate only
* Added purple tea, which is only usable by the hobbits, bushes must be dried before brewed into purple tea
* Added a Green Sand known as grunstaub
* Includes the bug fixed version of the latest DFFS raws
* Now includes Gnorm's Demonic Cherubs


### Turn 6 (Zanzetkuken)

**What I Added:**
* All those dragon variants.
* Lizardfolk, large bipedal lizards, as a playable civilization. This civilization has the child snatcher tags, so all civilizations are hostile to them. (Manual will come later.)
* Dragonkin, the bipedal draco-morphed lizardfolk. Currently needs an item snatching civilization. I give a later modder freedom to create this civilization.
* Wandering spirits that are only vulnerable to Aerisium (needs testing). You don't really need to worry about them, though. All they can do is emit a small cloud of ether occasionally.


### Turn 5 (HugoLuman)

-Six new creatures: 2 varieties of dirigible antelope, 4 wildly different Cephalopods
-Mallards now limited to lakes, rivers, ponds, and wetlands. [COMMON_DOMESTIC] still lets any civ anywhere use them, though.
-Hounds no longer exist in the wild, replaced by "Feral Hounds". They are restricted to badlands, tundras, mountains, and temperate forests, making room for other creatures to appear.
-Halfling's eye template changed so that eye injuries don't cause instantaneous bleedout
-Carts and palanquins added
-Had to move the Dirigible Antelope to my creatures file so that the variant would work
-Halflings no longer active during the summer
-Numerous bugs fixed, including all the fixes Halfling requested, no errorlog on my end.


### Turn 4 (sackhead)

_To do: Write a change log for this turn!_


### Turn 3 (LaularuKyrumo):

Striking the Earth just got slightly more interesting!

**New things include:**

* 1 creature -- Hell Riders, eternally flaming beasts that drop Magmaline when killed and, while being rather fragile, regenerate at STUPID rates--so if you don't chop their limbs off, they'll heal nearly all damage if they get away from you.

* 3 new metals -- Iridium, high tier metal that takes a lot of effort to smelt; Aeresium, magma-safe building metal; Lunanium, non-magma-safe, very dense weapons-grade metal

* 5 new soils -- Brown dirt (just soil), Blue dirt (aquifer soil), Red sand (sand that appears in deserts and non-deserts), Black Ooze (oceanic soil), and Blue Ooze (oceanic aquifer soil). New soil template included.

* 9 new layer stones, including one for Hell. (It's still ice.) Experience them yourselves!

* 3 new non-layer stones. Magmaline, a dragonfire-safe stone that never shows up (hopefully) and drops from killing Pale Riders. Oxyline, an aquifer stone that is required (along with Magmaline) to process Iridium. Horichoko, a generic stone that literally exists to keep oxyline from showing up GODDAMN EVERYWHERE, and is ideal for making engraved mugs. (There's a joke in there somewhere.)

* Halflings and Formics have been updated with two lines:

        [PERMITTED_REACTION:IRIDIUM_MAKING_STAGE1_LKR]
        [PERMITTED_REACTION:IRIDIUM_MAKING_STAGE2_LKR]

Have !!fun!!, everyone!

**Updates:**

Turns out that I didn't stick _LKR on a bunch of material names, so fixed that. Also, StLeibowitz and Halfling teamed up and both included a copy of FINE_SAND_HLG, somehow doing the impossible and creating duplicate raw entries. Finding walls made out of FROZEN BLOOD was pretty much the reason we found this. It's fixed in this version and should be fixed soon in Leibowitz's raws, if it isn't already.

* 3.2 update: blue ooze is now properly located in the oceans instead of everywhere else. Whoops!

* 3.3 update: Chaosine (an otherwise unremarkable rock) now has DEEP_SPECIAL, to keep the game from defaulting to the alphabetically first file, which happens to be goddamned jaded slade. Future versions have permission to switch Chaosine back to METAMORPHIC once we have an official DEEP_SPECIAL material. Also, ice looks less ugly now.

* 3.4: Added appropriate colors and tiles to all of my rocks. They no longer look identical! I think.


### Turn 2 (StLeibowitz):

**Additions:**

* multifarious insectoid lifeforms, including a milkable giant aphid, water grubs, swarming giant wasps, shearable giant bees, and a Savage Giant Sea Scorpion to prowl the depths abandoned by the Giant Sperm Whale
* Some annoying vermin - a wisp of rage in Evil biomes to turn your colonists against each other violently, and two types of mosquitoes - one of which carries dengue fever (note: not all dengue becomes hemorrhagic. Except for a very few cases, the poor halfling will just get a little mouth bleeding, nausea, bad fevers, and muscle pain. And to keep everyone away from the pitchforks, the dengue version lives only in savage tropical areas.)
* some lovely new plants - a farmable cave fungus, several new types of trees, and two new flavors of grass.
* ability to prepare chitin from butchered insects, turning it into a metal for armor usage
* new clothing and armor (chainmail robes)
* new weapons: scimitar, lance, morningstar, spiked whip (last two are for the Spider-Centaurs)
* two new civs - the twisted Spider-Centaurs, who hate you, and the playable Formics, an ant-derived species with short lifespans and high birthrates.
* language translation for the Formics that seems to have turned out properly fast-paced
* creature alcohol: Honeywine, from those giant aphids (note:may not actually work properly in terms of "it goes in the barrel after you brew it, Halfwit.")
* two new metals: Celestium and Promethium
* three new gemstones: Fallen Stars, Diamonds, and Amethyst
* new rock type: Celestial Marble
* weather for deserts and good biomes (sunshine rain!) (note: have seen no evidence indicating the game lets them trigger. Playtests needed!)
* some genuine water vermin to fish. I fixed the flying trilobites, I swear!

No glaring bugs except maybe the reaver ants, who will likely be doing a lot of glaring at you when you plug up the caverns again.

Suggested starting point for Modding Turn 3. I mean, who doesn't like giant bugs?

UPDATE 1: Various bugfixes. Honeywine works now, Formics can now open doors ( :oops: ). Forgot to add in wood revisions...uh...don't use Frostheart/wood. I did, however, add in some optional disease-causing vermin. Just find the file "creature_disease_insects_STL" and follow the instructions inside.

UPDATE 2:
* Spider-Centaurs and Formics now properly have furnace operators, and should now arm themselves with metal gear.
* Frostheart trees moved down to caverns 2-3. The role of cavern 1 tree shall now be played by the lovely actress Giant Aspergillum Mold, with support from Cave Mold Grass.
* Breakbone/Dengue fever pain symptom has been tweaked for realism (no, this does not mean it's harder. This means it no longer cripples with pain instantly. It's milder now).
* Mastahcheese's alcohol templates and plant included
* Honeywine updated to use the above's alcohol template
* latest version of BFEL raws merged
* The bloodlessness of spider-centaurs was not intentional. This has been rectified.
* "The Shakes", from the optional disease insects, has been expanded to cause dizziness, and now affects everyone. The Red Death from the same file has been tweaked to prolong the suffering of terminal patients. Antennae rot has been removed entirely, as I was displeased with it.

UPDATE 3:
* Added "equips" token to Spider-Centaurs.
* Spider-Centaur entity edits: No longer tolerate cities, can be bandits, no longer use wood weapons
* Formic edit: can now be bandits (they are sentient, so some extremely eccentric individuals may decide to duck out of the caste system)
* Merged in Halfling's Paladin interactions, to allow for magic immunity.
* Duplicated MC's alcohol template for creature alcohols and updated Honeywine again to use it.

UPDATE 4:  
Everything _seems_ pretty stable (no bug reports, at least) so this should be the last update, barring any new bugs uncovered in the future.
* Added Shadows to the HFS, with a syndrome that turns victims into Shades in under twenty ticks (fun!)
optional plague flies are now restored to optionality, i.e. they are now not active by default.

UPDATE 5:  
Getting rid of some persistent, though not major, bugs.
* Shadows now have the "crazed" token, for some extra incentive to kill everything that isn't them.
* Bandit Moth wing scales should work properly now. I've got my fingers crossed behind my back as I'm typing this, honestly, but it should work. I hope.
* Fixed the Dengue/Breakbone Fever syndrome as Knight Otu suggested. Hemorrhagic fever should now involve actual hemorrhages now.
* unneeded duplicate creature variations in the formic creature raws have been excised, also as Knight Otu suggested.

UPDATE 6:  
DIE MOTH BUG DIE
* Finally got moth wing scales to work. It was a typo. Oops.
* New template for gems that doesn't have ITEMS_HARD. Hopefully, this should stop people from using fallen stars as doors and anvils, which is almost a cool enough image to merit it an upgrade to a full feature.

UPDATE 6.5:  
Added Halfling's fancy new vampire modifications.
* see above

UPDATE 7: FINAL UPDATE
* My sincerest apologies for the "unintended feature" that was causing duplicated raws (ie, frozen blood walls). The coders responsible have been sacked.
* Just to be clear, I got rid of the dupe and now things should be fine and dandy and pleasantly bug-filled once more.
* Good bugs, I mean. The intended kind.
* The ones also known as "insects".
* If there are more not-insect bugs than this one, I will feel most silly.


### Turn 1 (BFEL):

**New features:**

* New non-playable civ (elves and their treelord masters)
* New surprise stone (jaded slade)
* An interaction set for vampirism by Halfling (_not_ the same as vanilla DF vampires)

**Bugfixes to this release:**

* Update I: Treelords no longer are made entirely of "skin" and "molten skin" and bleed sap as intended.
* Update II: Moved to mastahcheese's enhanced raws and updated minimal world raws
* Update III: Everybody no longer turns into a vampire upon fortress mode exit and reload. Vampires no longer initially visible.
* Update IV: Properly named vampirism interactions for adv mode.
* Update V: Jaded slade no longer is immediately useful. Instead if it can be obtained, it must be activated at a smelter and can then be used as before. This is so civilizations don't make their equipment out of it.
* Update VI: Includes newest version of minimal world raws


### Turn 0 (Halfling):

This is a "minimalist" version of DF, created "from scratch", entire raws folder is now 144.3 kB. Fully playable. Intended for building an entirely player-made world on.

**Features:**

* new, small language vocabulary and symbols
* no creatures, materials, tissues or templates from vanilla are available
* random creature generation suppressed, the massive error messages generated by this suppressed (by the _shutupdf files).
* meant to be ideal for creating new things out of scratch!

**Included:**

* some body, material, tissue templates written "from scratch" (values were rounded from vanilla for balance). Intentionally different and not out-of-the-box compatible with vanilla in any way. Everything is marked with ending `_HLG` so will not clash by name
* one intelligent and playable race
* "plain english" translation for new vocabulary
* two domestic animals: hound and mallard
* one megabeast, one semimegabeast
* one type of soil and one type of rock
* one metal and its two ores
* one edible plant, one tree, one cloth-producing plant
* very plain basic underground and overground grass ("moss")

**Parts of vanilla included:**

* `item_default`: some items needed to run fortress mode and that it would not make sense to define twice, such as wheelbarrows
* `descriptor_color_standard`: really no point in making new color definitions for now... or is there? If so, it's easily replaceable.

**Notes:**

The `raw/objects/text` folder contains empty files required by DF to run. It's suggested to generate a world with megabeasts (the included ones ensure it works) but without random creatures. Worldgen always generates one error message from suppressing random creatures, "Cannot generate random creatures -- missing body gloss RCP_GLOSS_PAW". **Don't add a RCP_GLOSS_PAW ever.**

Happy modding!

**Fixes added after initial upload:**

* Bugfix 1: no longer in unix linefeed format (durr)! Halfling carpentry reaction fixes
* Bugfix 2: it came up that Halflings were upset about not having shoes. Created open sandals for now.
* Bugfix 3: MEAT IS NO LONGER WORTH INFINITE NEGATIVE MONEY (sorry, being god is hard)!  Enabled more professions because it was a little frustrating to play. Maybe to be removed when there's more trade partners. Limited naming somewhat for slightly less ludicrous names.
* Balance 1: Hounds more aggressive. More hounds and mallards in biomes. A reaction is now called "make wooden shovel". Slapping things with your bow does less damage. Some other things, including fixes in language. More fixes in language.
* Bugfix 4: new egg and organ materials are now edible when cooked.
* Bugfix 5: keratin is actually obtainable from non-bird creatures too now. Organ and nervous tissues labeled correctly upon butchering. Creatures overall improved (http://www.bay12forums.com/smf/index.php?topic=127552.msg4352787#msg4352787). Added screws to make pumps.
* Bugfix 6: a basic sand is added to make deserts work better
* Bugfix 7: halflings can no longer bring shovels at embark due to this leading to bugs sometimes. The reaction in the player guide can still be used to make them and they still work the same.
* Bugfix 8: minifix: a token `HAS_VAMPIRES` had crept back upstream from a later development. Removed. This doesn't affect anything other than errorlog.txt.