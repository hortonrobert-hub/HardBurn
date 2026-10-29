# Hard Burn: Core Loop Test

A playable prototype of a single-player, Expanse-style "Oregon Trail in space" fleet management game. It has no art yet. This build exists to answer one question: **is the core loop fun?**

Your feedback on that question is what this test is for.

## The premise

You own the *Kestrel*, a worn-out freighter with four crew. You owe **Marta Quill 6,500 credits**, due **day 50**. She wants **1,500 at your first dock after day 25**. Haul cargo between the inner system and the Belt, keep the crew alive, and pay off the note. One run takes about 15 to 25 minutes.

## The world and your role

The solar system is settled but not at peace. Earth and Luna hold the money, Mars holds the guns, the Belt holds the water and ore, and the Outer worlds around Ganymede hold the cold, hungry frontier. The lanes between them are dangerous, with pirates, raiders, patrol cutters, and plain bad luck. You are not a hero or a soldier. You are the captain of a small, indebted freight company, and your whole job is staying solvent and keeping your people alive. Your stops are Ceres and Vesta (the Belt), Mars, Luna (Earth), and Ganymede (the Outer worlds). Every job you take, every fight you pick, and every favor you do for one faction costs you standing with another. A water dispute in the Belt eventually forces you to pick a side.

## How a run flows

1. **At a station** you take jobs, shop, handle crew and ship repairs, refit, and pay the loan.
2. **Plan a trip.** Pick a destination and a burn mode. Hard Burn is fast and thirsty. Economy is slow and cheap.
3. **Travel day by day.** Along the way, incidents interrupt you and you decide what to do.
4. **Arrive, get paid, repeat.** Fights, breakdowns, and story events change your odds along the way.

The run ends when you pay off the debt, run out of days, lose the ship, or lose the crew. On the last day you get a **final reckoning** so you can still sell up, repair, and settle before the end screen.

## The dice

Everything uses **2d6 + skill + modifiers**:

| Total | Result |
| --- | --- |
| 4 or less | Disaster |
| 5-6 | Failure |
| 7-9 | Mixed |
| 10-11 | Success |
| 12+ | Critical |

Every choice shows its **odds bar** before you commit. Crew skills are shown as PLT (pilot), ENG (engineering), MED (medical), GUN (gunnery), SYS (sensors and systems), NEG (negotiation). The best-suited crew member is picked for each job, but you can choose who handles an incident.

**Fate** (the diamonds at the top, 2 per run) lets you reroll one bad result.

## Incidents

An incident gives you a few approaches, usually **Safe**, **Bold**, or **Gamble**. Safer options have smaller downsides and smaller rewards. The crew's traits (Cautious, Reckless, Paranoid, and so on) tilt the odds for certain approaches. There is also a three-stage story quest, **Water Rights**, that pays well and changes who likes you (Earth, the Belt, and others).

## Crew

- **Stress** builds from hard burns, danger, and short rations: Steady, Strained, Frayed, Breaking. Higher stress means worse rolls. Shore leave (80 cr per crew, costs a day) clears it.
- **Injury**: hurt crew roll worse. At a station you can pay to heal them. Away from a station, the **Treat** button spends 1 med.

## Ship, supplies, and the hold

- **Hold space is shared** by cargo, food, spares, meds, and ammunition. Fuel has its own tanks.
- **Rations** (full, half, quarter) trade food for morale.
- **Field repair** costs 1 spare and can be done once per day, in port or in flight.
- **Cannibalize** and **jury-rig** options are available when you are desperate.
- **Refit tab** (stations only): armor plating, fuel tanks, cargo bay, drive tuning, railgun capacitors, a second PDC, sensor refit, ECM suite, auto-doc, better berths. Upgrades last for the whole run.

## Combat

Fights use **range bands** (Close, Medium, Long). Each weapon is good at different ranges, and the small map shows the modifier for each weapon at each range. The enemy has a preferred range and will try to pull the fight there.

Each round you give orders:

- **Helm**: close in, open range, evade, or hold. Or use a **heading order** instead (face the enemy, bring your guns to bear, cover with your PDCs, turn away). The pilot rolls to turn the ship.
- **Gunnery**: pick a weapon, a **fire level**, and a target (hull or a subsystem).
- **Engineering**: damage control, power weapons, power helm, or overload.
- **Command**: stance (aggressive or defensive), disengage, parley, or surrender.
- **Torpedo defense** (when the enemy has torpedoes): choose your first line of defense.

### Bearing and weapon arcs

The enemy is not just at a range. It is also at a **bearing**: one of six sectors around your ship (bow, starboard bow, starboard quarter, stern, port quarter, port bow). The tactical scope shows your ship in the middle of the range rings, the enemy as a contact, and:

- **Weapon arcs.** Each mount only covers some sectors. The Kestrel starts with a fixed railgun and forward torpedo tubes that cover the bow and both bow sectors, and a port PDC and a starboard PDC that cover three sectors each. A weapon can only fire if the enemy is inside the arc of a working mount. Green shading on the scope is the arc of the weapon you have selected.
- **PDC coverage band.** The outer ring of the scope counts the working PDCs covering each sector. An ✕ is a gap.
- **Turning.** Heading orders turn the ship so the enemy lands in a better sector. It costs your helm action that round. A good pilot turns farther.
- **The enemy moves too.** It tries to slide to a sector where your guns are thin.
- **Hits land on the side they come from.** Damage to your weapons knocks out specific mounts, and the log names them.
- **Refits.** An aft PDC mount closes the stern gap. A railgun turret widens the railgun arc to five sectors at -1 to hit.

### Munitions

| Weapon | Ammo and price | Hold each | Fire levels |
| --- | --- | --- | --- |
| Railgun | Slugs, 8 cr | 0.2 | Cheap and steady. 1 slug, 2 (+1 hit, +2 dmg), 3 (+2 hit, +4 dmg) |
| Torpedo | Torpedoes, 85 cr | 1.5 | Heavy hitter. 1 torpedo, or a 2-torpedo salvo |
| PDC | Belts, 3 cr | 0.1 | Close-range spray. 1, 2, or 4 belts |

Torpedoes can be shot down by the enemy's point defense. Firing more at once costs more per point of damage.

### Defending against torpedoes

An incoming torpedo is stopped by a chain of defenses. Your choice sets which one goes first and the rest follow automatically:

- **PDC fire** (1 belt)
- **Flak screen** (3 belts, stronger)
- **Decoys** (1 decoy, 25 cr each)
- **Jam / hack** (free, uses your systems officer)
- **Spin to cover** (free, pilot and gunner together): when no working PDC covers the side a torpedo is coming from, the ship swings round so one does, and then it fires. It needs both pilot and gunner for the best chance, and a lone crew member does it badly. Long range gives you two tries, close range only one. The spin also changes your heading, so your guns may no longer bear.
- **Hard turn** (free, your pilot dodges; costs you -1 attack)

PDC fire only counts PDCs that cover the torpedo's sector; each covering PDC gets a shot. Knocked-out systems take their defenses away: no PDC means no PDC or flak, dead sensors mean no jam or decoys, and a dead drive means no hard turn.

## What we want to know

Please play a couple of runs and tell us:

- **Where were you bored?** Which stretches felt like clicking through, not deciding?
- **Which decisions felt real**, and which had an obvious right answer?
- **Was it fair?** Did bad outcomes feel like your fault or like random punishment?
- **Combat**: do the weapon, ammo, and defense choices feel meaningful?
- **Pacing and difficulty**: too easy, too hard, too long, too short?
- **Would you play another run?** What would make you?

Use the **Feedback** button in the game. If it can't send, use the Copy as text option and send it to us another way.

## Known limitations

- **No saving.** Closing the page or pressing Restart loses the run.
- **Placeholder balance.** Prices, pay, and difficulty are not tuned.
- **Arcs are new.** Only your ship has weapon arcs. The enemy fires from wherever it sits, and the scope's bearing is the same for every enemy.
- **No art or sound.** This is a systems test.
- **One ship only.** No fleet, no boarding, and enemy strength does not yet scale with how dangerous the lane is.
- **Test bots win about 80% of runs** because they play fairly simply. A thoughtful human should find it harder, and we want to hear if it is not.
