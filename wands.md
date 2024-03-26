# Wands

Wands are one of the most powerful items in the game.

They provide a way to soften up enemies before engaging, and escape from tough situations.

The majority of wands are powerful all game, because their effects scale regardless of enemy
strength, so are just as useful even on the final fight of floor 26 as when you bought it on floor 6.

Even the wands which do not scale (magic missile, lightning, disintegration) are still fantastic,
as the damage cannot be blocked and cannot miss. **Anything** is better than hitting the "wait" button.

All wands are guaranteed to hit, and ignore armour, meaning that a +0 wand can still be a massive
help. Even the most powerful enemies in the game sometimes end up with 1 or 2 HP, and knowing you
don't have to risk another melee attack, which might miss, but can instead just ping them down with
a wand at point-blank is huge.

Try to make sure none of your wands are ever fully charged, or that means they are not recharging,
which is a huge waste of resources. If you have too many wands to use, you need to approach enemies
from further away, create more distance when you aggro an enemy, or turn a wand into arcane resin.


## Upgrading wands

I rarely choose to sink a scroll of upgrade into a wand, but it's not a terrible idea to use one on
a utility wand, especially if you only have one, and it's always on 0 charges. I probably wouldn't
do so for a damaging wand though. The main reason I don't is because arcane resin exists.

If you end up with more than about 2 or 3 wands, it's definitely worth **considering** converting
one into arcane resin - A +0 wand is nice... but turning two other +0 wands into +1 wands is often
better. Late game, you may want to more aggressively convert wands to arcane resin depending on
your thrown weapon arsenal and number of wands.


## Using wands

As mentioned in fighting.md, you should use your wands to chip away at enemies before they are in
melee distance.

Never get into a ranged battle with an ranged enemy, regardless of how powerful your wands are.

Make ranged enemies come into melee distance, and make melee enemies stay at range.

Try to apply damage at long range (Lightning, Fire, Disintegration), and status effects at close range
(Corruption, Frost, Transfusion).


## Recharge formula

Wands (and artifacts) actually recharge slightly faster when they are lower charge.
For example, a wand missing 1 charge will take 45 turns to recharge, but a wand missing 3 charges
will only take 37 turns to recharge - which means you can zap 25% more often!

The formula is:

```10 + (40 * (0.875 ^ missing_charges))```

Which gives the sequence:

 - 1 Missing Charge: 45 turns to gain a charge
 - 2 Missing Charges: 41 turns to gain a charge
 - 3 Missing Charges: 37 turns to gain a charge
 - 4 Missing Charges: 33.5 turns to gain a charge
 - 5 Missing Charges: 30.5 turns to gain a charge
 - 6 Missing Charges: 28 turns to gain a charge
 - 7 Missing Charges: 26 turns to gain a charge
 - 8 Missing Charges: 24 turns to gain a charge
 - 9 Missing Charges: 22 turns to gain a charge

Note: Having your wands in the magical holster increases their recharge rate by a very small amount,
about 3% per missing charge.

You can see the [code](https://github.com/00-Evan/shattered-pixel-dungeon/blob/master/core/src/main/java/com/shatteredpixel/shatteredpixeldungeon/items/wands/Wand.java) here.

## Getting wands

You should always, without exception, take a wand, regardless of what other sacrifices must be made.
Buy them even before health potions - they will save you more life in the long run.

For example, in "Vault" rooms, when there are two crystal chests, but you only have one key,
you should always choose a wand, if available. You can tell what's in each chest by inspecting it.

Even in "Crystal Choice" rooms, I usually take the chest over the assorted potions/scrolls, because
I often value a 1/3 chance of a wand more than the consumables.

Read the farming section for how to farm for a wand or two in the Caves.
