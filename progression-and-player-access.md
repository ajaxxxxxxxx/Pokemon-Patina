# Player progression and competitive access

Status: design requirements, not implemented. Applies to Pokemon Patina's native GBA campaign.

## Hard badge-based level caps

| Badges held | Next challenge | Gym ace target level | Player cap |
|---:|---|---:|---:|
| 0 | Gym 1 | 15 | 20 |
| 1 | Gym 2 | 25 | 30 |
| 2 | Gym 3 | 35 | 40 |
| 3 | Gym 4 | 45 | 50 |
| 4 | Gym 5 | 55 | 60 |
| 5 | Gym 6 | 65 | 70 |
| 6 | Gym 7 | 75 | 80 |
| 7 | Gym 8 | 85 | 90 |
| 8 | League/postgame | TBD | 100 |

Hard cap = min(100, 20 + 10 * badge count). Stop experience at the exact threshold for the cap; discard overflow and do not bank it. Rare Candies and Exp. Candies must respect the cap. EV and friendship gains remain possible at cap. Badge acquisition immediately unlocks the next cap. Level-up evolutions must remain possible at cap when all other requirements are met; proposed eligibility check when the Pokemon would otherwise gain XP, with safeguards for canceled evolutions, minimum levels, friendship, held items, and location/weather/status requirements. No obedience-based substitute for the hard cap. Policy for catching, receiving or trading Pokemon above cap remains TBD.

Use these bands to plan route encounters, trainer levels, gym teams and resource availability. Suggested common wild encounters per gym: 3–12, then 13–22, 23–32, 33–42, 43–52, 53–62, 63–72, 73–82; ordinary trainer ranges 5–13, then 15–23, 25–33, 35–43, 45–53, 55–63, 65–73, 75–83. These are guidelines, not mandatory restrictions. League levels (proposed Elite Four 90–95, Champion 95–100, Mewtwo gauntlet 100) remain provisional.

## Adaptive party-wide Exp. Share

Award catch-up XP individually based on the recipient's level gap below the current badge cap, not simply relative to the defeated opponent. No held item required. Preserve ordinary participation/shared XP rules as the baseline, then multiply each eligible recipient's award by the following factor:

| Levels below cap | Multiplier |
|---:|---:|
| 0 or above cap | 0x |
| 1–5 | 1x |
| 6–10 | 2x |
| 11–20 | 3x |
| 21–30 | 5x |
| 31+ | 10x |

The 10x multiplier applies to every gap of 31 levels or more. The aggressive curve compensates for nonlinear XP requirements and makes late-game captures and team changes viable without excessive grinding. Capped party members must not reduce others' awards. Proposed implementation: determine factor at each XP award, multiply using sufficiently wide arithmetic, clamp at the cap XP threshold for that species' growth curve, and test multi-level gains, level-up moves/evolutions and candy handling. Exact rounding and interaction with existing scaled XP, traded bonuses, Lucky Egg and fainted members TBD.

## Competitive access milestone — before Gym 6

Mandatory availability deadline: when the player first becomes eligible to challenge Gym 6 (five badges, cap 70), all seven requirements below must be met. Availability is not automatic ownership; costs, challenges, quests and exploration can still gate acquisition.

1. Competitive held items: repeatable Battle Tree-like random trainer battle facility with rewards exchange or equivalent reward system. Use player-owned Pokemon normalized to level 50, or rental teams. Facility battles should not require grinding to the current campaign cap; exact modes, rental rules, reward economy and opponent pools TBD.
2. All Mega Stones: an obtainable path to every planned stone by this milestone, including difficult or lengthy quests; possession is not guaranteed. Existing special requirements such as Eeveeite collection quest remain relevant. Mega activation access must be consistent with this goal.
3. Move tutor and move relearner: both services accessible.
4. EV management: means to reset and deliberately influence/train EVs.
5. Substantial Safari, Friend Safari and other limited-access encounter areas available, potentially with sponsorship-dependent access. Preserve the optional sponsorship model; exact access tiers TBD.
6. All environment types, weather conditions and locations necessary for special-condition evolutions accessible, including Acid Rain and other relevant location-based evolutions. Do not require a later badge just to reach a required environment.
7. TMs accessible by this milestone; exact distribution, acquisition cost and whether every individual TM must be obtainable at this point remain to be specified.

These requirements are a world-design acceptance checklist, not merely optional postgame content. Before finalizing maps and quests, verify availability routes against the five-badge milestone, including sponsorship restrictions and dependencies. Early access is permitted. No requirement to give everything away for free.

## Implementation

Use pokeemerald-expansion hard-cap and party-wide EXP facilities where suitable; custom adaptive XP and edge-case handling require implementation and testing. Level-50 facility normalization must be temporary, restoring actual party levels after the facility. No code implemented by this design document.

See [gym design](factions-groups-gyms.md), [Pokemon roster](pokemon.md), [narrative outline](narrative-outline.md), and [sidequests](sidequests.md).
