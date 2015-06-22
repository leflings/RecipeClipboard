# Recipe Clipboard

This is a mod for the brilliant game of Factorio.

**Disclaimer: This is my first, and very quick'n'dirty, attempt at a factorio
mod. This might be a horrible hack, done completely against the idiomatic ways,
but hey it works, so here I'm sharing it.**

## Backstory
After playing quite a bit of Factorio with Bob's collection of mods, I grew very
tired of the repetitive task of setting up chains of item assemblies (mk1,
mk2... etc), configuring both Smart Inserters watching the network count, and
chests requesting the right items, in the right ratios. So I set out to make
a mod to, if not completely automate it, remove a lot of the hassle.

## So what does it do?
Recipe Clipboard adds the ability to
- Copy the ingredient list and count from any assembling machine (or anything
  with a recipe configured)
- Copy the product item from any assembling machine
- Paste ingredient list and count to logistic chest
- Paste recipe product item to any smart capable inserter

## Notes
**For some reason, the window of the inserter/chest being pasted into, will have
to be reopened for the changes to appear on the screen. Game-wise the settings
are pasted instantly.**

When copying/pasting the ingredient list, it will request twice (x2) the amount
listed in the recipe, of each ingredient. This can be configured in the lua
file.

When pasting to an inserter, it will limit the network capacity to 5 as default.
This can be changed in the lua file.

When pasting a recipe to a logistic chest, the mod will attempt to merge the
ingredient list, with any current reques slots set in the chest. The mod doesn't
do anything about the 10 slot limit though.

The mod filters out any ingredient which isnt a solid type (ie, no fluids).

## Screenshots
![Copy build requirements](/copy.jpg)
![Paste to inserter](/paste_inserter.jpg)
![Paste to requester chest](/paste_chest.jpg)
