Dwarf Fortress from scratch
===========================

_The entirely player-made universe._

DF from scratch (dfscratch) is a project to redesign and rebuild the world of [Dwarf Fortress](http://www.bay12games.com/dwarves/) entirely from scratch. We start with a vanilla version of DF, delete all raws with their creatures and bodies and templates and materials, and build an entire new player-made universe by hand.


How to play?
------------

1. Download [Dwarf Fortress](http://www.bay12games.com/dwarves/) for your OS and unzip it.  We highly recommend using a separate installation of DF for dfscratch.

2. **Delete the entire `raw` folder.**  Failure to do this will give you a crazy (and probably broken) mix of vanilla DF and dfscratch.

3. Download the latest dfscratch release (or one of the earlier releases, if you want to try them out).  Unzip it **into the same folder you installed DF into**.

4. Start playing.

Dfscratch is a work in progress, and we're <s>glad</s> _desperate_ to receive feedback from players!  If your try it out, you're more than welcome to post a journal of your game events at the [official forum thread](http://www.bay12forums.com/smf/index.php?topic=127552.0).  Any reports of bugs or any unexpected weirdness are particularly welcome.


How to contribute?
------------------

If you're reasonably familiar with [DF modding](http://dwarffortresswiki.org/index.php/Modding) and want to take part in the project, feel free to sign up for a modding turn.  Dfscratch is developed as a "succession" project, meaning that modders take turns being responsible for the development of the world.  Currently, each turn lasts two weeks; a list of past and upcoming turns can be found in the [forum thread](http://www.bay12forums.com/smf/index.php?topic=127552.0), where you can also request a turn for yourself.

You're also welcome to contribute code outside your turn, or even without signing up for a turn at all, e.g. by posting it to the thread or by submitting a pull request on GitHub.  In that case, you also need to ask the person whose turn it currently is to approve your code for inclusion.


### Rules for modders:

* **You are not allowed to copy-and-paste any raws from vanilla DF** or from other mods.  (Copying existing code _within_ dfscratch is acceptable, though.)  The _point_ of this mod is to create a completely new and different set of raws, not to pick and mix stuff from vanilla.

* Copying specific values (like, say, the tensile strength of iron) from vanilla DF is OK, although you should use common sense in doing so.  There's not much point in making a value different _just_ for the sake of being different, but on the other hand, there's also no need to follow vanilla slavishly -- our iron doesn't have to be exactly the same as vanilla iron.

* You are explicitly encouraged to make use of infrastructure (such as material templates, body detail plans, etc.) added by other contributors.  However, **don't change other people's code without their permission** (except for bugfixes).  If you want to implement something that requires, say, adding a new tag to all creatures, please ask first.

* To make the world eventually more varied, you are, in violation of the above, allowed to reduce the frequency of old creatures or materials or limit them to biomes when new creatures are added, but not remove them entirely -- nor assign them to an impossible biome (badgers to the ocean). The new frequency must not be less than 10% of the old frequency, or 1, whichever is greater, and you must mark this edit with a comment to prevent repeating it.

* Suggestion: when defining materials, try to add a <code>[STATE_COLOR:ALL:<i>COLOR</i>]</code> where <code><i>COLOR</i></code> is a color of your choice. This is so StoneSense can figure out what color a sprite should be.

* **Test your changes before submitting them!**  At the very least, check that:

  * nothing is written into the DF error log (except for the "`missing body gloss RCP_GLOSS_PAW`" message, which is an unavoidable side effect of the hack used to eliminate vanilla DF's random creatures),

  * any creatures you added or changed work as expected in arena mode, and have an appropriate difficulty level,

  * worldgen works and doesn't crash,

  * any new playable civs, workshops, reactions, etc. work in fortress mode, and

  * any new adventurer races, interactions, etc. work in adventure mode.

**IMPORTANT:**

* To force compatibility with both vanilla DF and other players' contributions, so that raws never clash, and novelty so that copypasting simply does not work, you _must_ add "`_XYZ`" to the end of every object that you newly add/define, where "`XYZ`" is a three-letter (or longer) tag of your choosing (e.g. "`HLG`" for Halfling). The exception to this is language words.

* Similarly, whenever possible, place all your raws in new files that include your name / tag, (e.g. `creature_domestic_halfling.txt` for Halfling), so we can keep track of who contributed which files.

* Lastly, you must not take a week to add only one material. Sorry. I can't really tell you how much you should add, but if you're not comfortable making new objects, you should probably not take a turn. Consider doing a playtest turn instead.

_(To do: add other stuff from the initial forum post here?)_


### How does this Git thing work?

The idea behind having a GitHub repository is to make tracking the changing raws easier, and to have a single place where the entire history of the project can be found.  **You don't have to use Git to contribute**, although you might want to give it a try -- it's very useful once you get the hang of it.

Here's how the GitHub repo is supposed to work:

* There's one main development branch ("master"). The person whose turn it is decides what goes on this branch (subject to the rules, of course, i.e. no broken code on the main branch, please). If you don't want to use Git yourself, just send your updates to a repo maintainer (currently Vyznev, but others are welcome to help too).

* At the end of each turn, a "release branch" is split from the master branch. Only bugfixes go on release branches. The latest release branch is what playtesters should download.  For development, you should generally download the latest version from the master branch.

* If you want to contribute stuff but it's not your turn, send it to a repo maintainer (or just post it in the thread) and ask the person whose turn it is if they'll approve it. If they do, it goes on the main branch; if not, it goes on a new "topic branch" (git jargon) where it can be kept, improved and possibly merged into the main branch later.

  The exception to this are simple bugfixes, which don't require approval and can (and should) be automatically backported to all releases affected by the bug. Contributed code should be based on the current master branch or the latest release, unless it fixes a bug specific to an earlier release. In any case, to make maintaining the repo easier, please try to make it clear which version your submitted changes are based on.

* If you use Git yourself, you can either [fork the repo](https://help.github.com/articles/fork-a-repo) and submit [pull requests](https://help.github.com/articles/using-pull-requests) for your stuff, or you could ask for direct push access to the main repo (as long as you promise not to mess it up) so you can merge in your own stuff. All "work in progress" should be kept on topic branches, and only tested and working code should be merged into the master branch.

  The nice thing about using Git is that whenever new updates are added to the master branch, you can tell Git to fetch and merge them into your working branch with a few simple commands (or mouse clicks, if you're using a [GUI front-end](http://git-scm.com/downloads/guis)).  Assuming there are no conflicts, everything just works.  (The one exception is if you've edited the exact same part of some file that has also been changed in the upstream repo, in which case you'll need to resolve the conflict by hand.  Then again, you would've had to do the same thing in that case anyway, with or without Git.)

_(To do: need to add some instructions here about how to clone the dfscratch Git repo into your DF folder.)_

Links
-----

* Official forum thread: http://www.bay12forums.com/smf/index.php?topic=127552.0

* Project wiki: http://dfscratch.shoutwiki.com/

  * Alternative wiki 1: http://df-from-scratch.wikia.com/

  * Alternative wiki 2: http://dffs.wikia.com/

* Things we found useful / Modding resource collection:

  * Perl scripts for editing DF data files: http://www.bay12forums.com/smf/index.php?topic=127552.msg4641172#msg4641172 _(To do: put these in Git.)_

  * Wiki rip reference of modding tokens: http://dffd.wimbli.com/file.php?id=6588

  * Workshop graphics utility: http://dffd.wimbli.com/file.php?id=2068 (honorable mention for providing source)

  * Language generator: http://dffd.wimbli.com/file.php?id=7174 
