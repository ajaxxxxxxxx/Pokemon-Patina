# Player progression and competitive access

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
| 8 | League/postgame | 100 | 100 |

Hard cap = min(100, 20 + 10 * badge count). Stop experience at the exact threshold for the cap; discard overflow and do not bank it. Rare Candies and Exp. Candies must respect the cap. EV and friendship gains remain possible at cap. Badge acquisition immediately unlocks the next cap. Level-up evolutions must remain possible at cap when all other requirements are met; proposed eligibility check when the Pokemon would otherwise gain XP, with safeguards for canceled evolutions, minimum levels, friendship, held items, and location/weather/status requirements. No obedience-based substitute for the hard cap. Policy for catching, receiving or trading Pokemon above cap remains TBD.

Use these bands to plan route encounters, trainer levels, gym teams and resource availability. Suggested common wild encounters per gym: 3–12, then 13–22, 23–32, 33–42, 43–52, 53–62, 63–72, 73–82; ordinary trainer ranges 5–13, then 15–23, 25–33, 35–43, 45–53, 55–63, 65–73, 75–83. These are guidelines, not mandatory restrictions.

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

The aggressive curve compensates for nonlinear XP requirements and makes late-game captures and team changes viable without excessive grinding. Proposed implementation: determine factor at each XP award, multiply using sufficiently wide arithmetic, clamp at the cap XP threshold for that species' growth curve, and test multi-level gains, level-up moves/evolutions and candy handling. Exact rounding and interaction with existing scaled XP, traded bonuses, Lucky Egg and fainted members TBD.

## Competitive access milestone — before Gym 6

Mandatory availability deadline: when the player first becomes eligible to challenge Gym 6 (five badges, cap 70), all seven requirements below must be met. Availability is not automatic ownership; costs, challenges, quests and exploration can still gate acquisition.

1. Competitive held items: repeatable Battle Tree-like random trainer battle facility with rewards exchange or equivalent reward system. Use player-owned Pokemon normalized to level 50, or rental teams. Facility battles should not require grinding to the current campaign cap; exact modes, rental rules, reward economy and opponent pools TBD.
2. All Mega Stones: an obtainable path to every planned stone by this milestone, including difficult or lengthy quests; possession is not guaranteed. Existing special requirements such as Eeveeite collection quest remain relevant. Mega activation access must be consistent with this goal.
3. Move tutor and move relearner: both services accessible.
4. EV management: means to reset and deliberately influence/train EVs.
5. Substantial Safari, Friend Safari and other limited-access encounter areas available, potentially with sponsorship-dependent access. Preserve the optional sponsorship model; exact access tiers TBD. Specialized type-focused Safari habitats have increased hidden ability encounter rates and serve as alternative environmental evolution locations; see the Safari habitat section below and [abandoned Eeveelutions](sidequests.md#abandoned-eeveelutions). Existing evolution routes must remain available without relying on post-Eeveeite encounters.
6. All environment types, weather conditions and locations necessary for special-condition evolutions accessible, including Acid Rain and other relevant location-based evolutions. Do not require a later badge just to reach a required environment.
7. TMs accessible by this milestone; exact distribution, acquisition cost and whether every individual TM must be obtainable at this point remain to be specified.

Before finalizing maps and quests, verify availability routes against the five-badge milestone, including sponsorship restrictions and dependencies. Early access is permitted. No requirement to give everything away for free.

## Specialized Safari habitats

Eden Reserve operates compact, approximately single-screen, type-focused Safari habitats. Each has a square central encounter area (grass or equivalent), a surrounding encounter-free walking ring, and optionally a central 3x3-tile body of water where appropriate. Wild encounter pools emphasize the habitat's type and have increased hidden ability rates; exact rates and species pools TBD.

| Planned habitat | Type | Environmental Eevee evolution |
|---|---|---|
| Toxic Marsh | Poison | Noxeon |
| Dust Basin | Ground | Loameon |
| Crystal Cavern | Rock | Litheon |
| Butterfly Sanctuary | Bug | Papileon |
| Twilight Grove | Ghost | Spectreon |
| Caustic Wetlands | Acid | Erodeon |

Each habitat provides an alternative high-friendship level-up evolution trigger, comparable to Moss Rock or Ice Rock. Names may be refined during map development.

| Visit rule | Unsponsored | Eden-sponsored |
|---|---|---|
| Entry fee | 500 | Free |
| Step limit | 100 | Unlimited |
| Wild battle limit | 10 | Unlimited |

Unsponsored visits end at whichever limit is reached first; both counters reset on entry. Proposed implementation: count movement steps throughout the habitat, including the safe perimeter, and completed wild battles including captures, fleeing and defeats; if a limit is reached during a battle, eject after battle resolution. Sponsored visits disable both limits. Normal battle/capture mechanics are intended rather than traditional Safari Ball-only encounters, consistent with training and evolution in these habitats. Exact counter integration, exit behavior, encounter rates and special encounter retry handling require implementation/testing. The abandoned Eeveelution quest is separate from the access rules; see [sidequests](sidequests.md#abandoned-eeveelutions).

## Main Safari — abandoned breeding Pokemon

The region's one large Safari Zone, comparable in scale to Emerald's Safari Zone, houses Pokemon released en masse as unwanted products of competitive breeding. Use normal wild battles and ordinary Poke Balls, not bait, rocks or Safari Balls. All Pokemon caught here start at zero friendship, reflecting their previous treatment. Wild encounters provide access to egg moves. NPCs scattered throughout the reserve lament releasing the wrong Pokemon, neglecting to check shininess, or releasing a Pokemon carrying an important item. Free overworld pickups include discarded special grasses (herbs), EV training items and staple TMs. Exact item placement, species pools, egg move distribution, IV/shiny/hidden ability rates, admission and visit limits are TBD. Second Chance Reserve is the location name; joint Eden/Pedigree involvement is a proposal. This large reserve is distinct from the six compact specialized Safari habitats.

The mandatory pre-Gym-6 road-closure investigation requires entering Second Chance Reserve and finding the fugitive former Gym Leader. Either surrendering him or submitting false evidence of his departure reopens the roads; only surrender preserves eligibility for sponsorship after Gym 6. See [narrative outline](narrative-outline.md#pre-gym-6-road-closure--fugitive-former-gym-leader). Reserve admission must permit unsponsored story progression; the investigation must not delay the competitive access milestone beyond eligibility for Gym 6.

## Postgame gym progression

After the League, all eight gyms reopen with revamped subordinate and leader battles; the incumbent or reinstated former leader depends on the historical badge petition quest. Historical badges are separate quest inventory items from the eight original progression badge flags, so surrendering or returning a historical badge does not reduce the player's level cap. Defeating a reinstated leader awards the historical badge again, allowing delayed legendary prerequisites to be satisfied. Timing relative to the Mewtwo gauntlet, repeatability and precise difficulty TBD. See [historical badge collection](sidequests.md#historical-badge-collection).

## Sponsored traversal and fishing equipment

The highest-quality fishing rod and fastest bicycle are exclusive sponsorship benefits. Lower-quality fishing rods and a standard bicycle remain available without sponsorship. Proposed assignments: Eden Reserve provides the Super Rod; Catalyst Industries provides the High-speed Bike. Exact item names, speeds, fishing encounter differences, acquisition timing and handling on loss of sponsorship remain TBD. Unsponsored equipment must permit all mandatory story traversal.
