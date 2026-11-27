# Acid type and draft move catalog

Acid is the sole new elemental type (19 total). Existing species and move typings are not retroactively changed: Acid and Acid Spray remain Poison-type, for example. New Acid species, regional forms and broader learnset compatibility introduce the type. Acid is a natural element as well as an industrial one.

## Type chart

| Existing type | Acid attacks | Attacks against Acid |
|---|---:|---:|
| Normal | 0.5 | 1 |
| Fire | 0.5 | 1 |
| Water | 0.5 | 2 |
| Electric | 1 | 1 |
| Grass | 2 | 0.5 |
| Ice | 1 | 1 |
| Fighting | 1 | 1 |
| Poison | 0.5 | 0.5 |
| Ground | 0.5 | 2 |
| Flying | 1 | 1 |
| Psychic | 1 | 1 |
| Bug | 2 | 0.5 |
| Rock | 2 | 0.5 |
| Ghost | 1 | 1 |
| Dragon | 0.5 | 1 |
| Dark | 1 | 1 |
| Steel | 2 | 0.5 |
| Fairy | 1 | 1 |
| Acid | 0 | 0 |

Offense: four strengths, six resistances, one immunity. Defense: two weaknesses, five resistances, one immunity. All other matchups are neutral.

## Corroded

A nonvolatile major status condition that pressures defensive and setup Pokemon off the field. At the end of each turn, reduce one randomly selected combat stat by one stage: Attack, Defense, Sp. Attack, Sp. Defense or Speed. No direct HP damage, accuracy or evasion changes. Switching resets stat stages normally but retains the status.

Acid, Water, Poison and Ground types are immune. Ordinary burn and poison immunities still apply to attacks of every type, including Acid. The new status does not bypass them.

Implementation decisions remaining: selection when stats are already at their minimum, interactions with stat-drop prevention and reversal, cures, status-cleansing abilities and ability suppression.

## Acid Rain

Sandstorm-like residual damage except Acid, Poison, Ground and Water types are immune. The Acid/Flying cloud/storm family and Vitriol have an ability that establishes this weather (working name Acidic Atmosphere); it is Vitriol's sole ability.

Draft baseline: damage equal to 1/16 maximum HP at end of turn; five turns of ordinary ability-set weather; immunity if either defensive type qualifies. No automatic type damage bonus, defensive bonus or additional status effect. Interaction with Thunder (rain-like accuracy without weakening Fire) is exploratory, not established. Ability and weather-extending item names, move parameters, immunity abilities/items, field visuals and exact weather interactions remain TBD.

### Primal Acid Rain
Primal Vitriol's sole ability (working name Primordial Corrosion) establishes persistent Acid Rain while it remains active. Ordinary weather moves and abilities cannot replace it, following Primordial Sea and Desolate Land mechanics; other primordial weather abilities (Desolate Land, Primordial Sea and Delta Stream) can override it. Pokemon switching is unrestricted. On ability activation, dissolve existing entry hazards on both sides (Stealth Rock, Spikes, Toxic Spikes, Sticky Web); hazards may be placed normally afterward. Weather retains ordinary Acid Rain residual damage and type immunities. Test activation timing relative to entry hazard damage, weather suppression, simultaneous primordial abilities and weather restoration when a competing setter leaves. Weather Ball should become Acid-type in Acid Rain with ordinary weather power behavior (draft).

## Draft move catalog

One row per new move or unresolved move concept. Names and numerical parameters are draft unless specified otherwise. BP is base power; accuracy is a percentage; a dash denotes not applicable; TBD denotes an unresolved parameter. Existing moves used in example sets or learnsets are not new move definitions.

The design includes Flamethrower, elemental punch, Rock Blast and Aqua Jet counterparts, weaker utility attacks, and attacks that target the opposite defensive stat.

| Move | Type | Category | BP | Accuracy | PP | Effect / design |
|---|---|---|---:|---:|---:|---|
| Caustic Spit | Acid | Special | 30 | 100 | 25 | 20% burn; noncontact; early Inchid attack |
| Corrosive Spit | Acid | Special | 40 | 100 | 25 | 10% poison |
| Erosion | Acid | Special | 40 | 100 | 25 | 30% chance to lower one random combat stat by one stage; noncontact; Shuckle disruption move; BP and effect chance are design targets |
| Caustic Spray | Acid | Special | 65 | 100 | 20 | 10% burn |
| Corrosive Jet | Acid | Special | 90 | 100 | 15 | 10% burn; Flamethrower counterpart |
| Chemical Torrent | Acid | Special | 110 | 85 | 5 | 10% burn |
| Caustic Beam | Acid | Special | 130 | 90 | 5 | User Sp. Attack -2 |
| Acidic Mist | Acid | Special | 80 | 100 | 10 | All adjacent; 10% poison |
| Penetrating Solution | Acid | Special | 80 | 100 | 10 | Uses user's Sp. Attack against target's Defense (special damage) |
| Etch | Acid | Physical | 40 | 100 | 30 | No additional effect |
| Caustic Fang | Acid | Physical | 65 | 95 | 15 | 10% burn, 10% flinch |
| Corrosive Punch | Acid | Physical | 75 | 100 | 15 | 10% burn; elemental punch counterpart |
| Caustic Rush | Acid | Physical | 40 | 100 | 20 | +1 priority; Aqua Jet counterpart |
| Chemical Barrage | Acid | Physical | 25 | 90 | 10 | 2–5 hits; Rock Blast counterpart |
| Corrosive Claw | Acid | Physical | 80 | 100 | 15 | High critical-hit ratio |
| Dissolving Strike | Acid | Physical | 120 | 100 | 15 | 1/3 recoil |
| Osmotic Strike | Acid | Physical | 80 | 100 | 10 | Uses user's Attack against target's Sp. Defense; a 60 BP version or weaker counterpart remains an option for Precision Sting, not a settled replacement |
| Corrode | Acid | Status | — | 85 | 15 | Inflicts Corroded |
| Caustic Coating | Acid | Status | — | 85 | 15 | Burn |
| Chemical Contamination | Acid | Status | — | 90 | 15 | Poison |
| Armor Dissolution | Acid | Status | — | 100 | 15 | Target Defense -2 |
| Solvent Mist | Acid | Status | — | 100 | 15 | Target Sp. Defense -2 |
| Concentrate | Acid | Status | — | — | 20 | User Sp. Attack +2 |
| Acid Rain (working name) | Acid (draft) | Status | — | — | TBD | Establish Acid Rain; duration and other details follow weather rules |
| Light Levy | Electric | Special | 75 | 100 | 10 | Solarceny signature candidate; restore 50% of damage dealt |
| Radical Blast | Rock | Special | 25 | 90 | 10 | 2–5 hits, Rock Blast counterpart; chance to burn or poison; normal status immunities apply. Exact status odds and per-hit versus per-use checks TBD; BP, accuracy and PP draft |

Move contact flags, targeting, animations, exact distribution and implementation details remain open unless stated. Do not create duplicate versions of Erosion or the cross-defense attacks by treating encounter notes as separate move definitions. Erosion excludes accuracy and evasion; its stat pool is the same five combat stats as Corroded.

## Move compatibility and balance

Many Water, Grass, Fire and Poison Pokemon should have access to suitable Acid moves without acquiring Acid typing. Choose learnsets by anatomy, chemical ecology and battle role. No blanket distribution of recovery plus Corroded to bulky species. Existing species may receive learnset improvements (including Ledian) without changing their type.

Precision Sting, Burning Brightly and Familial Bond are defined in the [Pokemon roster](pokemon.md#custom-abilities). Test secondary effects, multihit attacks, conditional power, priority, spread moves and cross-defense damage calculations in combination with these abilities. Individual Pokemon learnsets and encounter movesets belong in the roster and gym documents, not in duplicate move-definition tables.

## Acid-induced evolution

The canonical evolution paths are in the [Pokemon roster](pokemon.md). Togepi and Eevee use high friendship plus level-up while Corroded or in Acid Rain; ordinary Kakuna can evolve into alternate Bug/Acid Beedrill under either Acid condition without a friendship requirement. Provide a reliable overworld Acid Rain location, accessible by the [Gym 6 milestone](progression-and-player-access.md#competitive-access-milestone--before-gym-6). No dedicated Acid evolution item is needed for these branches.

## Implementation

Use existing pokeemerald-expansion effects, animations and logic where suitable. New type chart, UI assets, AI awareness, move/species data, cross-defense attacks and Corroded require implementation and testing. Audit status storage, save compatibility, cures, ability interactions and AI.
