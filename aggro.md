# Aggro


## No distance between you and the enemy

Once an enemy is "touching" you, you can never lose aggro from it unless you are able to break line
of sight TWO turns in a row. The most common example is by repeatedly walking diagonally around a
single tile of grass, but can also be done by mixing different methods together:

- Walking diagonally around a tile (grass or wall)
- Walking through a door
- Walking through a square of grass (Huntress)
- Going invisible
- Inflicting blindness on the enemy
- Inflicting affection on the enemy
    - This one must be done before another method
    - E.g., Inflict affection, then walk through a door
- Several other obscure methods

## One tile between you and the enemy

When there's one full tile between you and a melee enemy, NEVER walk up to them. If you take the
final step towards them, they will get a free attack on you. Let them come to you.


## Increasing distance between you and the enemy

If an enemy is following you, but hasn't caught you yet, you can easily increase the distance,
(and sometimes lose them), by walking through a door, then hugging the wall to either side, so when
the enemy opens the door, you're pressed up against the wall, and they cannot see you.

```
────┴E┴  <-- An enemy, who was following you (1 tile between you)
   Y     <-- You, running to the left
```

In the above diagram, if you were to wait your turn here, the enemy would of course take a single
step towards you, and be within melee distance. Then you will never lose them without items, tall
grass, or if you find 2 doors next to each other (very rare).

The critical thing to do is to just keep walking along the wall. It might feel like you're being
cornered, but that's okay. The enemy is guaranteed to be "confused" for a full turn while they
wonder where you went. Then, they'll have a 50-50 chance of walking back the way they came. And even
if they do walk into the same room as you, they won't neccesarily walk towards you, they might walk
away, further increasing the distance.

Using this method, you can get free hits on enemies with a whip, or weave in an extra wand zap or
thrown weapon. Just wait till they're showing the little "confused" popup, and then smack them.

This is also an excellent way to escape enemies you cannot deal with. For example, I will often

## Aggroing an enemy

Not all attacks are equal when hitting an enemy.

An enemy which is zapped by a wand will have no idea where it came from, and will not *neccesarily*
walk towards you.

Interestingly, if you have a melee weapon with extra range (projecting enchantment, spear, whip, or
glaive), and hit an enemy without them seeing you, they will not know where you are, and will walk
randomly.

An enemy which was hit by a thrown weapon, or a melee weapon with extra range (spear, whip,
projecting enchantment, etc), they will **immediately** know exactly where you are standing, and
will walk to that exact location that you were standing at when you hit them (even if you are no
longer there). This allows for very creative hit-and-run tactics.

This is especially important for understanding how to exploit the "blindness" debuff. The warrior in
particular can throw items at an enemy to inflict a few turns of blindness, but an unsuspecting
enemy won't even realise that something unusual is happening unless they receive "physical" damage
from a thrown weapon or melee weapon with extra reach. They'll just keep patrolling as if someone
didn't just throw an entire suit of plate armour at them.


## Exploiting line of sight


### Taking cover

Imagine you are walking to the end of the corridor, but see a ranged enemy around the corner just
before you reach the end. You are 1 square away. You should be wondering:

> Do I run toward the enemy, to avoid their powerful ranged attacks, but give them a free melee hit?
> Or can I safely stand here, knowing they will have to come to me, giving me the first melee hit?

This is a huge difference. This situation happens to me probably 10 times every playthrough,
and can be the difference between the best outcomes:
- Getting a free turn to make a ranged attack, and ALSO the first melee hit on the enemy
- Realising you're in a bad spot, and either choosing to take a melee hit or retreating

And the worst outcomes:
- Guessing wrong, playing it safe, and getting smacked in the face for no reason
- Guessing wrong, taking a risk, and getting zapped for 20% of your HP (plus any debuffs)

Here are examples of ranged enemies who CAN see you, but CANNOT target you:

```
│ │
│E│  <-- An enemy which CANNOT ranged-attack you (but can see you)
│ ├─
│ Y  <-- You (in a doorway)
│ ├─
│E│  <-- An enemy which CANNOT ranged-attack you (but can see you)
│ │
```

```
──┴Y┴── <-- You (in a doorway)
 E   E  <-- Enemies which CANNOT ranged-attack you (but can see you)
───────
```

What is fascinating about this, is that the code seems to give completely different results for
what appears to be very similar situations. If you swap yourself with an enemy in the above
examples, that enemy will now be able to attack you just fine.

This concept can be simplified and summarised, to help you visualise and remember it:

> You can take cover behind corners

Think of it like an action movie - You poke your head out from around the corner, fire off a spell
or throw a spear, and then duck back to cover. Of course the enemy cannot target you!

It's important to remember though, this is an oversimplification. You may have trouble remembering
it in more complicated situations like the following:

```
┌──────┐
│  Y   │ <-- You
│  G   │ <-- Skeleton
│   D  │ <-- DM-100 (ranged enemy)
└──────┘
┌──────┐
│   Y  │ <-- You
│  G   │ <-- Skeleton
│  D   │ <-- DM-100 (ranged enemy)
└──────┘
```

To figure these out, you need to imagine that the body of the skeleton is a wall, then ask yourself
who would be taking cover behind that corner (hint - it's the closest character). I will leave this
as an exercise for the reader.

<details>
<summary>Answer to targetting problem</summary>
In the first example, you are able to take cover behind the skeleton, as if there was a straight
wall through the skeleton, and yourself, that kept going.

In the second example, the opposite happens. The straight line always goes through the skeleton,
because the skeleton is the obstacle, and his body is like a wall. Walls cannot be diagonal,
and so you will see that from the perspective of the DM-100, you're standing in the middle of the
room, exposed!
</details>


### Manual ranged targetting

It's sometimes possible to be in a situation where you cannot "automatically" target an enemy with
a wand or thrown weapon, but you can "manually" target them, by aiming your weapon at the correct
tile (which may not be the tile they are standing on).

Some examples of this is when you see an enemy, and attempt to cast a wand on them, but you receive
a message saying "You can't target yourself!". Or perhaps it does allow you to cast it, but the bolt
of magic simply hits a wall before making it to them. The same thing sometimes happens as well with
ranged weapons.

A more extreme example is when the enemy is so far away or behind a corner that the "auto-target"
doesn't even suggest them as a plausible target.

I haven't actually calculated all the times where this happens, but the most common time is when
the enemy is "behind cover" as I talked about above this. You'll get a feel for it though.

```
    Y│  <-- You, very far away
1    │
2    │
3    ├─
4    E  <-- Enemy in a doorway
5    ├─
6    │
7    │
8    X  <-- This is where you need to target to hit the enemy
     │
```

The trick here is to target 2x the distance away, so that the enemy is in the middle. So if the
enemy is 6 tiles away, just count 12 tiles, and aim there.


### Asymmetric line-of-sight

In Shattered Pixel Dungeon, the line of sight mechanic is quite unique - it's possible to be in
a situation where you can see an enemy, but they cannot see you (or vice-versa). This can be
exploited to get you 2 or more ranged sneak attacks in a row on an enemy.

A good example is this one:

```
 Y│ <-- You
  │
  │ <-- Tall grass or a wall
  E <-- Enemy
```

In this example, you could hit the enemy with a thrown weapon, and they would start walking towards
you (You may also need to use **manual ranged targetting** if the blocker was a wall).

This is one of the best ways to kill enemies who cannot fit through doors, such as:

- DM-200 / DM-201
- DM-300 (boss)
- Golems
- Giant enemies (when playing with the "Hostile Champions" challenge)
