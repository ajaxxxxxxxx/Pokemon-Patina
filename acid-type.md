# Acid type

## Confirmed design
Acid is the sole proposed new elemental type (19 total). Do not retroactively retype existing species or moves, including Acid and Acid Spray. Introduce original species, regional variants and new moves. Acid does not bypass normal burn or poison immunities.

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

Offense: 4 strengths, 6 resistances, 1 immunity. Defense: 2 weaknesses, 5 resistances, 1 immunity. Fighting and Fairy are neutral both ways, superseding earlier drafts.

## Corroded
Agreed concept: random stat reduction every round, to pressure defensive and setup Pokemon off the field without bypassing poison immunity. Proposed details: nonvolatile major status; at end of turn reduce one randomly selected Attack, Defense, Sp. Attack, Sp. Defense or Speed by one stage; no HP damage; no accuracy/evasion changes; skip stats already at -6. Switching clears stages but retains status. Acid types immune; mutually exclusive with other major statuses; Full Heal, Full Restore, Lum Berry and normal status cures work. No bypass of conventional burn/poison immunities. Clear Body, White Smoke, Contrary, Simple, Natural Cure, Guts, Synchronize, Shed Skin and Defiant/Competitive interactions need explicit testing/decisions. Keep Corroded distribution limited; most Acid attacks that cause status should burn or poison instead.

## Move design
User requirements: equivalents of Flamethrower, elemental punches, Rock Blast and Aqua Jet, including lower-power moves; special attack using target Defense and physical attack using target Sp. Defense. All names and numeric values below are draft proposals.

| Move | Category | BP | Accuracy | PP | Effect |
|---|---|---:|---:|---:|---|
| Corrosive Spit | Special | 40 | 100 | 25 | 10% poison |
| Caustic Spray | Special | 65 | 100 | 20 | 10% burn |
| Corrosive Jet | Special | 90 | 100 | 15 | 10% burn; Flamethrower equivalent |
| Chemical Torrent | Special | 110 | 85 | 5 | 10% burn |
| Caustic Beam | Special | 130 | 90 | 5 | User SpA -2 |
| Acidic Mist | Special | 80 | 100 | 10 | All adjacent; 10% poison |
| Etch | Physical | 40 | 100 | 30 | None |
| Caustic Fang | Physical | 65 | 95 | 15 | 10% burn, 10% flinch |
| Corrosive Punch | Physical | 75 | 100 | 15 | 10% burn |
| Caustic Rush | Physical | 40 | 100 | 20 | +1 priority |
| Chemical Barrage | Physical | 25 | 90 | 10 | 2–5 hits |
| Corrosive Claw | Physical | 80 | 100 | 15 | High critical ratio |
| Dissolving Strike | Physical | 120 | 100 | 15 | 1/3 recoil |
| Penetrating Solution | Special | 80 | 100 | 10 | SpA vs Defense |
| Osmotic Strike | Physical | 80 | 100 | 10 | Attack vs SpD |
| Corrode | Status | — | 85 | 15 | Corroded |
| Caustic Coating | Status | — | 85 | 15 | Burn |
| Chemical Contamination | Status | — | 90 | 15 | Poison |
| Armor Dissolution | Status | — | 100 | 15 | Defense -2 |
| Solvent Mist | Status | — | 100 | 15 | SpD -2 |
| Neutralize | Status | — | — | 20 | Reset user's stat stages |
| Reconstitute | Status | — | — | 5 | Recover 50% HP |
| Chemical Polish | Status | — | — | 20 | Speed +2 |
| Concentrate | Status | — | — | 20 | SpA +2 |

## Implementation notes
Prefer existing pokeemerald-expansion effects, animations and battle logic. New type chart, UI assets, AI awareness, move data and species data required. Physical vs SpD and Corroded require custom work; audit status storage, save compatibility, cures, ability interactions and AI. Avoid universal access to recovery plus Corroded on bulky species. No implementation or playtesting yet.
