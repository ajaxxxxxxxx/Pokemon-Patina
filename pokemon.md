# Pokemon roster

This is the canonical roster design record. Existing species retain their original typing; new regional forms retain the original species' base HP and BST (modern baseline), with other stats redistributed to improve viability. New species and regional-exclusive evolutions may use their own stat budgets. Moves and learnsets may be expanded without retyping a species.

Stat order: HP / Atk / Def / SpA / SpD / Spe. All stat spreads, names, abilities and evolution methods are drafts unless identified as fixed below. TBD denotes an unresolved design, not an omitted species. Each planned Pokemon appears in one roster table only. Unselected concepts are marked exploratory and excluded from totals.

## Original Pokemon

| Pokemon / family | Type | Draft stats (BST) | Abilities and design |
|---|---|---|---|
| Caustloom → Corrostorm | Acid/Flying | 55/30/45/65/65/50 (310); 90/45/85/100/115/65 (500) | Single cloud to storm; Acid Rain-setting ability; other slots TBD |
| Sulflet → Sulfurmander | Acid/Fire | 45/45/40/65/50/65 (310); 75/75/70/115/80/100 (515) | Natural volcanic salamander; candidate Flame Body / Flash Fire / HA Corrosion |
| Radion → Isotore | Acid/Rock | 80/50/80/60/45/25 (340); 80/65/110/130/85/55 (525) | Large dim radioactive mineral evolves into smaller, brighter form (half-life motif); candidate Static, Power Spot, Aftermath or Levitate |
| Filamite → Incandent | Electric/Fire | 45/30/45/75/55/50 (300); 75/45/75/125/95/85 (500) | Litwick-like single candle to group of candles; Flame Body / Flash Fire / HA Burning Brightly |
| Wispy → Wispur → Wispful | Fire/Fairy | 35/20/35/65/55/70 (280); 55/35/50/90/80/95 (405); 75/45/65/115/105/120 (525) | Fixed names; mote to orb to differently colored orb with small attendant motes; candidate Flash Fire / Illuminate; HA Burning Brightly |
| Voltacid → Plumbolt → Accumulacid | Electric/Acid | 45/35/55/65/55/30 (285); 65/45/75/95/75/40 (395); 95/65/95/125/100/50 (530) | Leaking single battery to pair sharing pool to stack with rising caustic body; candidate Volt Absorb / Battery / HA Corrosion |
| Drumuck → Barrotten → Vatoxic | Steel/Acid | 50/55/65/30/60/20 (280); 75/75/90/45/85/30 (400); 105/95/120/60/110/40 (530) | Overturned rusty drum to upright steel barrel with distinct fluid shape to multiple barrels feeding one body; Vatoxic name fixed; Poison Point / Magnet Pull / HA Levitate |
| Inchid → Acidcoil → Corrosaur | Acid → Acid/Dragon → Acid/Dragon | 30/15/40/35/35/45 (200); 70/65/80/85/70/50 (420); 105/100/120/125/100/50 (600) | Fixed names; Inchid candidate Run Away / Shield Dust; evolution at level 21+ with high friendship, then held item (item and trigger TBD); see family notes below |
| Heliosnore | Normal/Electric | 160/60/80/110/100/30 (540, draft) | Distinct Snorlax-derived species; relaxed sleeping posture, passive solar energy storage. Abilities and relationship to Munchlax TBD. Solarceny is its unique corrupted form. |
| Solarceny (corrupted Heliosnore) | Dark/Electric | 160/125/75/100/65/75 (600, draft) | Unique corrupted form of Heliosnore, central to Mewtwo plot; menacing forward-hunched predatory posture replaces relaxed sleeping pose. Reallocate bulk and special offense toward Attack and medium Speed; BST target at least 600, exact spread TBD. Monopolizes sunlight; candidate Solar Power / Opportunist / HA Lightning Rod; signature Light Levy in [move catalog](acid-type.md#draft-move-catalog). Species ID and permanent/reversible form mechanics TBD. |
| Vitriol | Acid | 600 BST target; distribution TBD | Sole ability Acidic Atmosphere (working name); establishes Acid Rain. Environmental climax and criminal exploitation; weather legendary affiliation favored for Yellow Orb plot, final mythology TBD. See learnset notes below and [narrative](narrative-outline.md). |
| Charmite → Charmoth | Bug/Fairy | 60/30/45/55/65/45 (300, draft); **85/40/85/100/100/90 (500)** | Cute termite-like first stage evolves into elegant moth with intricate butterfly-like wings. Candidate Compound Eyes / Shield Dust; Charmoth HA Magic Bounce. Flexible setup attacker, Baton Pass support or doubles partner. Learnset includes Sweet Scent, Baton Pass, Minimize, Protect, Substitute and Ominous Wind; additional candidates Quiver Dance, Pollen Puff, Moonblast, Draining Kiss, Silver Wind, Bug Buzz, Sleep Powder, Stun Spore, Tailwind, Rage Powder and Aromatherapy. Evolution trigger and exact learnset distribution TBD. |
| Vialit → Flaskor → Retortox | Ghost/Acid | 35/25/45/65/65/45 (280); 55/35/65/90/90/65 (400); 75/45/85/125/115/75 (520) | Possessed/animated alchemical or chemistry equipment; candidate vial → flask → interconnected retorts; candidate Cursed Body / Liquid Ooze / HA Contrary; stats and evolution triggers draft |
| Cucorrosive → Picklevat | Water/Acid | 50/30/40/70/50/70 (310); 70/45/65/120/85/125 (510) | Fast special attacker; sea cucumber and pickling/brine motif; candidate Swift Swim / Liquid Ooze / HA Regenerator; stats and evolution trigger draft |

| Primal Vitriol | Acid (base typing retained provisionally) | TBD | Yellow Orb held-item Primal Reversion; sole ability Primordial Corrosion (working name), persistent Acid Rain that blocks ordinary weather replacement; dissolves existing entry hazards on both sides on activation. Pokemon switching and subsequent hazard placement are unrestricted. See [weather rules](acid-type.md#acid-rain). No independent learnset. Sprite, stats and exact reversion behavior TBD. |

### Inchid family
Inchid is common in wild grass and kept as a cute pet in some regions, despised in industrial and agricultural areas. Its low BST should be comparable to Magikarp or cocoons; early burn-capable Acid damage and utility make it trainable. Acidcoil is temperamental, requires trust, and appears on ordinary trainer teams. Corrosaur is an enormous segmented tube worm; its existence as a final evolution is largely unknown, with NPC clues to the required held item. Reserve it for ace trainers, gym leaders, Elite Four, bosses and comparable opponents; no routine wild evolved-stage encounters planned.

Inchid's draft level-up learnset: 1 Caustic Spit and String Shot; 4 Sand Attack; 7 Harden; 10 Charm; 13 Sticky Web; 16 Erosion; 19 Acid Armor; 23 Draining Kiss; 25 Baby-Doll Eyes; 27 Dazzling Gleam; 29 Moonblast. Minimum evolution level 21 and high friendship, plus Fairy moves at levels 23/25/27/29, are fixed design requirements. Exact move choices and early levels are draft. Delayed evolution should grant useful Fairy coverage; evaluate reminder/TM access so the tradeoff is meaningful.

### Vitriol learnset
Broad coverage across Acid, Fire, Water, Ground, Poison and Rock moves; staple/universal Normal moves; Thunder Punch, Thunder Fang, Snarl, Tri Attack, Weather Ball and Dragon Tail. Exact move selection within each type, level-up schedule, TM/tutor compatibility and signature moves TBD. Weather Ball should interact with Acid Rain (draft Acid typing and normal weather power behavior). Primal Vitriol inherits this learnset.

## Regional forms

A selected regional family includes its evolutionary stages unless an explicit exception applies. Related-stage typings marked draft are inferred, not finalized. Ordinary forms remain available. Beedrill's alternate form is listed under alternate evolution paths because ordinary Kakuna is its precursor; it counts as a regional/alternate form, not a new National Dex species.

| Pokemon / family | Type | Draft stats (BST) | Abilities and design |
|---|---|---|---|
| Sandshrew → Sandslash | Ground/Acid | TBD | Chemical excavation |
| Staryu → Starmie | Acid → Psychic/Acid | TBD | Caustic sludge rather than ocean |
| Bellsprout → Weepinbell → Victreebel | Grass/Acid | TBD | Digestive fluids |
| Shellos → Gastrodon | Acid/Ground (Shellos draft) | TBD | Candidate Storm Drain / Water Absorb for Gastrodon |
| Ekans → Arbok | Acid (Arbok draft) | TBD | Corrosive secretions |
| Tentacool → Tentacruel | Water/Acid (Tentacruel draft) | TBD | TBD |
| Grimer → Muk | Acid (Muk draft) | TBD | TBD |
| Shellder → Cloyster | Acid → Acid/Ice | TBD | Cloyster candidate Skill Link; Chemical Barrage, Icicle Spear, Rock Blast, Shell Smash |
| Shuckle | Bug/Acid | 20/10/230/10/230/5 (505) | Fermented corrosive berries; candidate Sturdy / Gluttony / HA Regenerator; see gym design |
| Dunsparce → Dudunsparce | Acid (Dudunsparce draft) | 100/45/90/75/90/15 (415); TBD | Chemical excavation; candidate Serene Grace disruption |
| Girafarig → Farigiraf | Psychic/Acid (Farigiraf draft) | 70/45/65/110/65/100 (455); TBD | Corrosive secondary head; candidate Armor Tail support |
| Sneasel → Sneasler | Fighting/Acid | 55/110/60/15/75/115 (430); TBD | Corrosive claws; candidate Tough Claws; no Patinian Weavile |
| Corsola | Rock/Acid | 65/35/115/45/115/35 (410) | Acid-adapted mineral structures; candidate Regenerator / Solid Rock; evolves exclusively into Caustola (alternate paths table) |
| Houndour → Houndoom | Dark/Acid (Houndour draft) | TBD; 75/50/60/125/80/110 (500) | Corrosive secretions; candidate Competitive |
| Horsea → Seadra → Kingdra | Dragon/Acid (first two draft) | TBD; TBD; 75/65/100/110/100/90 (540) | Acidic deep-water habitats; candidate Sniper / Adaptability for Kingdra |
| Corrupted Celebi | Grass/Acid | 100/60/120/110/120/90 (600) | Forest guardian altered by environmental destruction; candidate Regenerator; ordinary Celebi unchanged |
| Carnivine | Grass/Acid | 74/110/85/40/110/35 (454) | Digestive secretions; candidate Levitate / Strong Jaw / HA Liquid Ooze |
| Finneon → Lumineon | Water/Ice (Finneon draft) | TBD; 69/31/100/95/110/55 (460) | Surface pollution forces deeper habitat; enhanced bioluminescence, anglerfish-like light organ, bulk and Water/Ice/Electric coverage. Lumineon: Storm Drain / Lightning Rod / HA Burning Brightly |
| Heatmor | Fire/Acid | 85/75/85/115/85/39 (484) | Superheated caustic fluids; candidate Flash Fire / Liquid Ooze; HA Contrary |
| Purrloin → Liepard | Dark/Fairy (Purrloin draft) | TBD; 64/50/65/85/70/112 (446) | Prankster Liepard; other abilities TBD |

### Regional Shuckle — Corroded disruption specialist
Late-game stall encounter: Power Split / Corrode / U-turn / Erosion. Candidate Sturdy and Leftovers; no Protect or reliable recovery in this set. Power Split averages actual offensive stats, not stages; switching clears stat changes and Power Split but retains Corroded. See [gym design](factions-groups-gyms.md) and [Acid mechanics](acid-type.md).

## Alternate evolution paths and additional evolutions

| Pokemon / path | Type | Draft stats (BST) | Evolution and design |
|---|---|---|---|
| Togepi → Togecidic → Togechymic | Fairy/Acid (both new stages) | 65/40/85/80/100/35 (405); 95/50/100/120/120/60 (545) | High friendship plus level-up while Corroded or in Acid Rain; then Shiny Stone. Candidate Hustle / Serene Grace / HA Liquid Ooze; cute aesthetic, disruption via Erosion, Caustic Spit, Moonblast, Corrosive Jet |
| Porygon2 → Porygon-C | Normal/Acid | 85/60/80/125/100/85 (535) | Failed chemical experiment; candidate Chemical Disc, Download / Adaptability / HA Contrary |
| Patinian Corsola → Caustola | Rock/Acid | 85/45/135/65/135/45 (510) | New species, not Cursola; living chemically adapted reef; candidate Regenerator / Natural Cure / HA Solid Rock; evolution trigger TBD |
| Sunflora → Sumflarea | Fire/Grass | 85/35/75/135/110/60 (500) | Special attacker; evolution method TBD; candidate Chlorophyll / Solar Power / Drought |
| Kakuna → Patinian Beedrill | Bug/Acid | 65/80/40/70/65/75 (395) | Ordinary Kakuna evolves in Acid Rain or while Corroded; ordinary Weedle/Kakuna and Beedrill remain unchanged. Candidate Swarm / Technician / HA Poison Touch |
| Mega Butterfree | Bug/Dragon | 60/45/65/135/95/95 (495) | Mega of ordinary Butterfree; draconic wing tails and horns; candidate Compound Eyes / Tinted Lens |
| Mega Patinian Beedrill | Bug/Acid | **65/90/65/90/60/125 (495)** | Fixed spread; Precision Sting; fast technical physical/mixed/special attacker, not a raw physical glass cannon |

### Togepi branch narrative
Double down on cuteness rather than horror. Corporate culture claims Togetic/Togekiss were ugly mistakes and the Acid-induced branch is aesthetically superior, parodying nostalgia-driven redesign. Heritage Revival and PokeWonder are candidate promoters. The alternative is genuinely cute; ordinary forms are not objectively inferior. Candidate dialogue: “The brochure says it only works if your Togepi really trusts you. Isn't that sweet?” / “I've had my Togetic for eighteen years. Apparently it's unfashionable now.”

### Patinian Beedrill and Mega Beedrill — technical attacker
Precision Sting supports low-power utility and status attacks. Preserve original HP and BST; Mega gains physical bulk and mixed offense at the expense of immediate Attack and Speed. Candidate moves: Erosion, Caustic Spit, Poison Fang, Acid Spray, Pounce, Bug Bite, Twineedle, Caustic Rush, U-turn, Corrode, Swords Dance, Fell Stinger, Fake Out, Pursuit, Knock Off, Osmotic Strike (or a weaker counterpart). Fell Stinger can finish weakened opponents then enable priority or fast-move sweeping. Special gym ace set: Ancient Power / Silver Wind / Ominous Wind / Electroweb; encounter assignment and EVs in [gym design](factions-groups-gyms.md). Test multihit effects, conditional power and Poison Fang's doubled chance.

## Eeveelutions

All 19 types represented, including Normal; every evolution has 525 BST using the traditional permutation of 130,110,95,65,65,60. Eevee itself is unchanged. Collect one of each evolution for Eeveeite; see [sidequests](sidequests.md). Full Mega roster is exploratory; only the Normal Mega is established. All Mega forms are intended to retain monotype and 625 BST if developed.

| Pokemon | Type | Evolution method / status | Stats / ability notes |
|---|---|---|---|
| Vaporeon | Water | Existing | Unchanged |
| Jolteon | Electric | Existing | Unchanged |
| Flareon | Fire | Existing | Unchanged |
| Espeon | Psychic | Existing | Unchanged |
| Umbreon | Dark | Existing | Unchanged |
| Leafeon | Grass | Existing | Unchanged |
| Glaceon | Ice | Existing | Unchanged |
| Sylveon | Fairy | Existing | Unchanged |
| Familieon | Normal | Draft max friendship + Silk Scarf | **130/65/60/65/95/110 (525)**; candidate Adaptability / HA Protean |
| Championeon | Fighting | Draft level up knowing Fighting move | TBD |
| Zephyreon | Flying | Draft level up holding Pretty Feather | TBD |
| Toxeon | Poison | Draft level up while poisoned | TBD |
| Duneon | Ground | Draft Soft Sand or dedicated item | TBD |
| Lithoneon | Rock | Draft Hard Stone or dedicated item | TBD |
| Lepideon | Bug | Draft level up in ancient woodland | TBD |
| Spectreon | Ghost | Draft Dusk Stone | TBD |
| Ferreon | Steel | Draft level up holding Metal Coat | TBD |
| Drakeon | Dragon | Draft level up knowing Dragon move | TBD |
| Vitrioleon | Acid | High friendship + level up while Corroded or in Acid Rain | TBD |
| Mega Familieon (Mega Eevee) | Normal | Eeveeite; established | **130/90/100/90/100/115 (625)**; Family Bond |
| Mega Vaporeon | Water | Exploratory | 130/65/100/125/125/80; Poison Heal or Regenerator (alternate Water Absorb + Regenerator) |
| Mega Jolteon | Electric | Exploratory | 65/65/85/135/110/165; Transistor (alternate Volt Absorb + Transistor) |
| Mega Flareon | Fire | Exploratory | 65/130/100/95/130/105; Huge Power (alternate Flash Fire + Tough Claws) |
| Mega Espeon | Psychic | Exploratory | 65/65/80/175/100/140; Psychic Surge (alternate Magic Bounce + Psychic Surge) |
| Mega Umbreon | Dark | Exploratory | 95/65/130/65/180/85; Fur Coat (alternate Fur Coat + Magic Guard) |
| Mega Leafeon | Grass | Exploratory | 65/150/150/60/80/120; Tinted Lens (alternate Chlorophyll + Tinted Lens) |
| Mega Glaceon | Ice | Exploratory | 65/60/135/155/125/85; Adaptability (alternate Snow Warning + Slush Rush) |
| Mega Sylveon | Fairy | Exploratory | 95/65/90/145/155/75; Pixilate (alternate Pixilate + Punk Rock) |
| Mega Championeon | Fighting | Exploratory | Tough Claws |
| Mega Zephyreon | Flying | Exploratory | Aerilate |
| Mega Toxeon | Poison | Exploratory | Merciless |
| Mega Duneon | Ground | Exploratory | Sand Force |
| Mega Lithoneon | Rock | Exploratory | Solid Rock |
| Mega Lepideon | Bug | Exploratory | Skill Link |
| Mega Spectreon | Ghost | Exploratory | Shadow Tag |
| Mega Ferreon | Steel | Exploratory | Filter |
| Mega Drakeon | Dragon | Exploratory | Contrary |
| Mega Vitrioleon | Acid | Exploratory | Serene Grace |

All new Eeveelution names are working names. Evolution triggers require priority/conflict checks. Mega Familieon uses one large Eevee surrounded by chibi Eeveelutions. A single shared Mega Stone for every Eeveelution is a candidate approach. Universal Wonder Guard is exploratory, not selected; its effectiveness varies sharply with type weaknesses. Mega Vaporeon cannot hold Toxic Orb with Eeveeite; Huge Power Flareon and Fur Coat Umbreon require balance testing.

## Custom abilities

- **Burning Brightly:** prevents accuracy-reducing effects and improves move accuracy by 10%. Draft implementation: 1.1x multiplier, blocks accuracy-stage reductions; evasion and other accuracy interactions TBD.
- **Precision Sting:** Technician (1.5x power for eligible moves of 60 BP or less) plus Serene Grace (double eligible secondary-effect chances).
- **Family Bond:** eligible damaging moves strike twice, second hit at 50% damage; universal 1.5x STAB; immunity to major statuses including Corroded. Nominal eligible damage multiplier 2.25x. Draft standard Parental Bond exclusions for spread and multihit moves; test secondary effects, Power-Up Punch, priority, contact punishment, Focus Sash, recovery, ability suppression and existing/volatile statuses.
- **Acidic Atmosphere (working name):** establishes ordinary Acid Rain on entry; Vitriol's sole ability, also available to the Acid/Flying cloud family.
- **Primordial Corrosion (working name):** Primal Vitriol's sole ability; persistent Acid Rain while active; ordinary weather cannot replace it, but other primordial weather abilities can. Clears existing entry hazards on both sides on activation; neither switching nor subsequent hazard placement is restricted. See [weather rules](acid-type.md#acid-rain) for unresolved interactions.

## Existing species learnset improvements

Ledian receives a better movepool without a new form or evolution; exact additions TBD. Many Water, Grass, Fire and Poison Pokemon should learn suitable Acid moves without changing type. See [move catalog](acid-type.md).

## Roster totals

Minimum planned roster: 1,025 official Gen IX species + 29 original species + 1 corrupted Heliosnore form + 16 new evolutions (11 Eeveelutions and 5 other species) + 38 regional/alternate/corrupted forms (37 in regional table and Beedrill in alternate paths table) = **1,109** species/forms, with **1,070–1,071** unique National Dex species (depending on whether Solarceny receives a separate species ID). Of these, 60 are Acid type under provisional family-stage typings. Three established new Megas, 18 exploratory Mega Eeveelutions and proposed Primal Vitriol are excluded, as are official alternate forms.

Acid/Poison is intentionally unrepresented; do not force type-pair coverage. No regional Weedle, Kakuna, Weavile or Cursola. Rejected lower-tier and earlier regional brainstorms are not part of the roster.

## Production

No species or moves implemented yet. Finalize TBD stats, names, evolution rules, moves, sprites, cries, encounters and balance. See [progression](progression-and-player-access.md) for availability requirements.
