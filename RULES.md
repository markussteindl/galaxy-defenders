# Galaxy Defenders — Condensed Rules <!-- omit in toc -->

Cooperative tactical battle game, 1–5 players. Each player controls one agent; the aliens are run by the game's AI (Alien cards + Close Encounter cards). Missions and setup come from the Storybook. **Card/mission text always overrides this rulebook.** A player may run several agents; each acts independently and counts as one operative player. A player is operative as long as their agent is alive.

## Table of Contents <!-- omit in toc -->

- [§1 Game preparation](#1-game-preparation)
- [§2 Terrain \& line of sight](#2-terrain--line-of-sight)
- [§3 Round sequence](#3-round-sequence)
- [§4 Agent turn](#4-agent-turn)
  - [Movement](#movement)
  - [Combat](#combat)
  - [Actions (one per turn)](#actions-one-per-turn)
- [§5 Agent conditions](#5-agent-conditions)
- [§6 Weapons, powers \& items](#6-weapons-powers--items)
- [§7 Optional rules \& difficulty](#7-optional-rules--difficulty)
- [§8 GD-Wings (experience)](#8-gd-wings-experience)
- [§9 Alien tech](#9-alien-tech)
- [§10 The aliens](#10-the-aliens)
  - [Aliens turn](#aliens-turn)
  - [Signals](#signals)
  - [Teleport](#teleport)
  - [Alien assignment](#alien-assignment)
  - [Alien movement](#alien-movement)
  - [Alien combat](#alien-combat)
  - [Alien death](#alien-death)
- [§11 Swarm units (future sets)](#11-swarm-units-future-sets)
- [§12 Card clarifications (FAQ)](#12-card-clarifications-faq)
- [§13 FAQ \& errata change log](#13-faq--errata-change-log)

## §1 Game preparation

- Set up the mission according to the Storybook.
- Choose agents, assign gear, start at full health and ammo.
- Campaign: weapon number is a cap, other weapons stay in HQ.

## §2 Terrain & line of sight

- **Hex**: smallest map unit; used for movement and melee. One figure *or* signal per hex.
- **Area**: group of 7 hexes with a white border and a sight-marked center hex; used for distances (adjacent = 0, 1 area…), alien/signal movement, ranged combat.
- **Room**: an area (or part of one) enclosed by doors/windows.
- Terrain types:
  - **Standard hex**: freely crossed.
  - **Blocked hex side** (thick line): can't be crossed; blocks LOS; hexes across it are not adjacent.
  - **Door**: crossable; blocks LOS unless the attacker is adjacent to/on the door side/hex.
  - **Locked door**: acts as blocked until removed via *Bash a Locked Door*.
  - **Blocked door/window** (token): acts as blocked; only mission actions remove it.
  - **Window**: crossed only via *Leap Through Window*; does **not** block LOS.
  - **Edge hex** (half hex): unusable; blocks LOS.
- **LOS** — legal if a straight line from the source hex's center to the target hex's center crosses no blocked hex/side or door.
  - Attacks/powers require LOS unless stated otherwise.
  - Door exception: LOS is clear if the attacker is adjacent to/on the door side/hex.
  - Boundaries of blocking hexes also block LOS (FAQ).
  - Tokens (Flame, Signal, Teleport Point, etc.) never block LOS; only map tiles and overlays do (FAQ).
- **Human View (optional, default ON)**: agents see only through their 3 front hexes (180°).
  - Figure may be freely rotated at end of movement.
  - Drones (GD-209, Sentry-Gun) always see 360°.
  - Signal reveals always use normal 360° LOS.

## §3 Round sequence

1. **Refresh** — all powers/items refresh simultaneously:
   - Flip up used skills.
   - Regain energy shield tokens.
   - Replace Guard tokens.
2. **Strategy**
   - **Alpha Agent** — choose a leader (living agents only):
     - Plays first, draws the Event card, breaks ties/decisions.
     - Tiebreak order: Marine, Biotech, Infiltrator, Sniper, Hulk.
     - If the Alpha dies mid-round, next agent clockwise takes over.
   - **GD-Wings** — If ≥1 alien died last round:
     - Living agents may attempt the GD-Wings roll (see [§8](#8-gd-wings-experience)).
     - Order: Alpha first, then clockwise.
   - **Reinforcements** — the Alpha may discard 4 Alien Tech fragments for either:
     - one chosen generic device, or
     - one random improved weapon; class-restricted \
       (drawn from generic + in-play-class tokens).
   - Weapon replacement:
     - New weapon replaces old one and gains full ammo.
     - Agents can store declined weapons at HQ to equip before missions.
     - House-rule: swap infinite-ammo weapons only for other infinite-ammo weapons.
   - Dead agents may revive here for 1 Alien Tech fragment (see [§5](#5-agent-conditions)).
   - **Mission Status check** — check the mission's Objectives table top-down; first matching condition applies.
3. **Battle** — starting with the Alpha, clockwise, each operative player takes an **Agent Turn**, then an **Aliens Turn**.
4. **Event** — Alpha Agent draws an Event card; resolve all effects in printed order:
   - Signals entering agent LOS reveal immediately.
   - Card types:
     - *Standard* — resolve & discard.
     - *Weather* — stays in play until replaced by the next Weather event.
     - *Special* — see Storybook.
   - Signal teleports scale with agents in play (or an aliens-vs-agents comparison). Don't count inoperative players for the signal teleport table.

Play continues until a mission end condition is met (Accomplished / Partially Accomplished / Failed). If all players become inoperative, the mission fails immediately.

## §4 Agent turn

Three activities, any order, each at most once per turn: **Movement**, **Combat**, **Action**. Movement and Combat can never be split/interleaved; an Action may combine with them (e.g., powers that boost a roll, or special actions below).

### Movement
Move up to the Movement value, 1 movement point per hex. May not cross blocked hexes/sides, edge hexes, or alien-occupied hexes. May pass through (not end on) agents/friendly drones.

### Combat
1. **Hit roll**: attacker picks target + weapon, rolls the weapon's dice (BLUE/RED).
2. **Defend roll**: if the defender has an energy shield, it **must** first cancel hits, 1 shield *point* per hit (a "2" token covers two hits: it becomes a "1" on the first, is removed on the second). Then roll 1 BLUE die per remaining hit; each shield result cancels a hit. Each uncancelled hit = 1 wound. Armor Bolt effects resolve **before** wounds are inflicted (FAQ; cf. rulebook combat example 2).

Dice symbols:

| Symbol | Effect                                                                                                                         | BLUE | RED |
| ------ | ------------------------------------------------------------------------------------------------------------------------------ | ---- | --- |
| Hit    | Successful hit (attack only)                                                                                                   | ×5   | ×7  |
| Shield | Cancels a hit (defense only)                                                                                                   | ×4   | —   |
| Bolt   | Triggers weapon/power bolt effect (attack) or armor bolt effect (defense); applied **once** regardless of count, unless stated | ×2   | ×3  |
| GD     | No combat effect; used for GD-Wings rank-up rolls and Search results*                                                          | —    | ×2  |
| Ammo   | Discard 1 ammo token (max 1 per hit roll); ignore for melee/auto-ammo weapons                                                  | ×1   | ×1  |
| Jam    | Ranged weapon jams (place Jam token); unusable until unjammed                                                                  | ×1   | ×1  |
| Alien  | Fail; agents may not re-roll it unless a power says so; aliens with re-roll may                                                | ×1   | ×1  |

\* The rulebook's own p.17 symbol table omits the Search use — see p.20 and the Alien Tech section (p.28); note the official errata confirms other icon errors in this rulebook (e.g., the drone dice icons, [§6](#6-weapons-powers--items)). Don't "fix" this back to match p.17.

- No die may be re-rolled more than once, ever.
- Never target an empty hex/area. No friendly fire (unless optional rule): agents can't target/harm agents except with healing weapons.

### Actions (one per turn)
- **Use a power/item**: activate one standard ability, skill, tactic, or device.
- **Leap Through Window** *(Action)*: from a hex adjacent to a window hex, move to the other side.
- **Search** *(Action)*: inside a mission search area, not engaged. Roll 1 RED die: **Bolt** → 1 First Aid Kit (heal 1 HP now) or 1 ammo; **GD** → 1 random generic device or 1 Alien Tech fragment (fragment max once/round). Any other result: nothing. Repeatable.
- **Bash a Locked Door** *(Action + Combat)*: adjacent to (or on) the locked door hex; remove the lock token.
- **Evade** *(Action + Combat)*: roll 1 BLUE die; on a Shield result, disengage and may move; otherwise stay engaged.
- **Tactical Redeployment** *(Action + Combat)*: reposition to any empty hex in the current area (in addition to normal movement).
- **Unjam Weapon** *(Action + Movement or Combat)*: discard the Jam token; the forfeited activity is lost.
- **Mission special actions** as defined by the Storybook.

## §5 Agent conditions

- **Wounds/HP**: track with wound tokens; HP and ammo can't exceed the printed/starting maximum (FAQ).
- **Bleeding** (HP ≤ 0): forfeit Combat; Movement = 1 hex; Action only to use one power/item; lay figure down. Still a valid alien target and defends normally. Healing ≥1 wound restores healthy state. Any further wound = death.
- **Death**: player becomes inoperative — remove figure, lose 1 GD-Wings rank (if possible; can't drop below Copper), skip Agent & Aliens turns (but still holds/plays assigned alien cards when others activate them). Revive during Reinforcements for 1 Alien Tech fragment, placing the figure on any GD start hex.
- **Engaged**:
  - Trigger: starting a turn or ending movement adjacent to an alien, or coming into contact with one outside your own turn.
  - Passing adjacent mid-move does not engage.
  - Can't move away until the alien dies, a successful Evade, or a skill allows it.
- **Immobilized**: no movement (or movement-based actions) until next Refresh.
- **Paralyzed**: skip the entire turn until next Refresh; also counts as immobilized.

## §6 Weapons, powers & items

- **Campaign**: researched weapons stay in HQ and remain available for later missions (up to each mission's listed cap).
- **Armoury tokens** (Blue/Red): an agent moving over one discards it; next Reinforcements step the squad receives one random Improved/Alien weapon (FAQ). Blue→Improved, Red→Alien is inferred from the weapon rank colors, not stated in the FAQ.
- **Melee**: range 0; no ammo; never jams (ignore Ammo/Jam results).
- **Ranged**: ranged even against adjacent targets. Human ranged weapons use ammo tokens; some need ≥1 ammo to fire.
- **Healing**: heal 1 wound per hit rolled; the only weapons that may target agents (incl. self).
- **Alien weapons**: no ammo, never jam. Without the *Alien Knowledge* skill, any Alien or Jam result = total attack failure (all successes ignored); re-roll powers on Alien results still apply. The Lasergun is generic (any class) but still needs Alien Knowledge for normal use.
- **Energy shielded armor**: shield token regenerates each Refresh; spend to cancel hits before the defend roll.
- Power/item categories: **Standard** (uses your Action, once/turn), **Passive** (always on), **Reaction** (usable outside your turn, no Action needed). Skills/abilities refresh each round; tactics and devices are once per mission (tactics flip back on "Act of Valor" events; devices return via Reinforcements).
- **Basic damage** (unmarked attacks from powers) doesn't trigger melee/ranged-specific defenses. **"On hit effects"** trigger on any Hit rolled even if all hits are cancelled. **"Suffers X wounds"** = unavoidable, no defend roll.
- **Grenades** are devices (Action, not Combat); area damage; on-hit effect applies if ≥1 hit is rolled regardless of defense. *Grenadier* skill: re-roll grenade dice + gain 3 grenades (if available in the Warehouse).
- **Sentry-Gun** (Biotech device) / **GD-209** (Biotech skill): drones deployed adjacent to the Biotech via Action; activated with the Biotech's Action on later turns. Count as agents on the map (occupy hex, can be attacked) but have no own turn, can't regain ammo or be healed, see 360°, never jam, and don't count for event cards. Cannot be Engaged by aliens; may disengage from melee freely, no Evade test (FAQ). Their attack die is RED — the rulebook images on p.26/27 erroneously show green (Errata). Destroyed at 0 HP. Sentry-Gun can't move and has Guard; a destroyed one returns only via Reinforcements. GD-209 deploys once per mission; if destroyed it's out for the mission but usable again next campaign mission.
- **Guard** (reaction; Chromium and Sentry-Gun by default): once per round, attack a just-moved or just-revealed alien with any weapon. Track with the Guard token; return it at Refresh.

## §7 Optional rules & difficulty

- **Human View** — see [§2](#2-terrain--line-of-sight).
- **Close Fight**: an engaged agent may only attack aliens it is engaged with.
- **Friendly Fire**: agents can hit agents; immune to own weapons but not own devices (grenades, strikes).
- **Permanent Death**: dead agents rejoin the campaign at Copper rank (keeping researched weapons).
- **Rank-based Defense** (Storybook §5.4): caps defense dice by color rank.
  - Alien: Green 3, Blue 4, Red/Purple 5; Drones 3, NPCs 4, Agents 5.
  - Shields/energy shields work as usual
- **Official difficulty tips** (FAQ Tips):
  - Faster/easier: remove one Close Encounter #1 card from each Core Set mission (experienced players play as written).
  - Mission 5: play the short version from the site's Utility/Missions section if too hard or long.

| Option             | easy | normal | hard | very hard |
| ------------------ | ---- | ------ | ---- | --------- |
| Human View         | off  | on     | on   | on        |
| Close Fight        | off  | on     | on   | on        |
| Friendly Fire      | off  | off    | on   | on        |
| Permanent Death    | off  | off    | off  | on        |
| Rank Based Defense | on   | on     | on   | off       |

## §8 GD-Wings (experience)

During Strategy (if ≥1 alien died last round), roll 3 RED dice for GD results:

| Rank      | Enhancement                       | GD needed |
| --------- | --------------------------------- | --------- |
| Copper    | Ability (printed)                 | start     |
| Bronze    | Basic Tactic                      | 1         |
| Silver    | 1st Skill                         | 1         |
| Gold      | Improved Tactic                   | 2         |
| Palladium | Elite (flip sheet; energy shield) | 2         |
| Platinum  | 2nd Skill                         | 3         |

Max one rank gained per mission in a campaign (no limit in standalone). Death costs 1 rank. Campaigns may grant ranks in other ways (training missions, specific goals).

## §9 Alien tech

Gained by: first alien kill per Battle phase (1 fragment, max 1/round) and Search **GD** results in designated areas (max 1/round). 4 fragments → Reinforcements delivery; 1 fragment → revive a dead agent.

## §10 The aliens

- Ranks: **GREEN** normal, **BLUE** stronger, **RED** elite. Species: Xeno-Beta, Spine Critter, Xeno-Alpha, Aracnos, Xeno-Grey, Nexus, Xeno-Beast.
- **Alien cards** hold AI (movement/combat behavior), powers (BLACK standard, PURPLE passive, RED weapon, BLUE reaction), weapons, HP, armor, energy shields (some cancel up to 2 hits/round).

### Aliens turn
Active player draws a **Close Encounter card**; all matching aliens (by species/rank/condition) activate, starting with the Alpha's, clockwise (a player orders their own aliens freely). Apply the **first** applicable AI behavior rule (usually distance-based; requires LOS and a legal path; the "blind" rule needs only a path). Only one rule per activation; if none applies, the alien stays put. If no aliens match and the card has the **danger** symbol, new aliens teleport in. Reshuffle discards when either deck empties.

### Signals
- Face-down tokens (alien or human) forming the mission's signal reserve; teleport/move mostly during Events. If the reserve is empty when a teleport is needed, reshuffle the signal discard pile into it.
- Move center-hex to center-hex per area (another hex if blocked); one signal/alien per hex; treat unlocked doors/windows as open; may pass through (not end on) figures; can't cross blocked sides. If sent toward the closest Teleport Point while already on it, it stays put. With no legal walking path, a signal doesn't move (FAQ confirms: this applies to aliens too).
- **Reveal**: a signal in agent LOS is revealed immediately — top priority in any phase; check after every single movement step (hex by hex for agents, area by area for signals); a revealed signal's movement ends. If a signal can choose between a revealing and a non-revealing move, it must take the revealing one. Human signal → remove it (or per mission). Alien signal → draw the top Alien card + figure.

### Teleport
Roll 1 BLUE die to pick the Teleport Point matching the symbol (re-roll until a present symbol comes up; if a face shows both, the **Bolt** symbol takes precedence over the **starburst**); place the signal on the TP or nearest free hex (Alpha decides ties). Teleporting an *alien* directly: fetch its exact card (species + rank) from the alien deck instead of a signal.

### Alien assignment
The Alpha assigns each new alien card to the first player, in clockwise order, who has no (or the fewest) alien cards; if still tied, it goes to the Alpha. Exception: duplicate cards (same species + rank) go to the controller of the first copy. If all cards are in play, no more aliens can spawn until one dies (revealed signals just get discarded).

### Alien movement
- Center-to-center per area; movement ends on the destination area's center hex (off-center only if occupied/blocked; then pick the hex worst for the agents).
- May redeploy within the destination area to engage the target and as many agents as possible.
- "Move adjacent to X" = enter the target's area next to it (or the nearest adjacent area otherwise).
- Aliens disengage from melee freely, no Evade test needed; may pass through figures but not end on them.
- "Move back/away" = the way it came, else away from the closest agent.
- If sent toward the closest Teleport Point while already on it, it stays put.
- If a behavior rule can't be applied, use the next one.

### Alien combat
Same combat rules with exceptions: aliens ignore Ammo and Jam results; Alien results are re-rollable only via alien re-roll powers; no alien friendly fire ever. Target priority: **most wounded agent**, tiebreak **fewest remaining HP**. Ambiguities are resolved in the way most favorable to the aliens.

### Alien death
Wounds = HP → dead: remove figure, discard card. First kill of the round grants the Alpha 1 Alien Tech fragment.

## §11 Swarm units (future sets)

One card = multiple figures; starting figures = total HP; each figure defends as a 1-HP alien; unit LOS/distance uses its closest figure; nearest figure moves first, others follow adjacent; single attacks hit one figure, area damage hits all in the area.

## §12 Card clarifications (FAQ)

- **"Attack twice" AI**: perform the first attack normally; the second attack targets the same agent if still alive, otherwise another legal target at the same distance (if any).
- **Xeno-Grey**: cannot be activated by another Xeno-Grey; not a legal target for "Save The Master".
- **Xeno-Beast rage**: discard its card (with all inflicted wounds) and take the Enraged Xeno-Beast card at full health.
- **Reinforced Armor** (device): once activated, incoming hits **must** be absorbed by its shield tokens first — no choosing to defend normally.

## §13 FAQ & errata change log

All rules in this document that were changed, added, or corrected based on official sources ([galaxy-defenders.com/faq.php](http://galaxy-defenders.com/faq.php)), rather than the rulebook alone. Each is tagged inline with *(FAQ)*, *(FAQ Tips)*, or *(Errata)*. No forum-thread-based changes have been incorporated.

| §                                  | Rule                                                                                       | Source                       | Type                                  |
| ---------------------------------- | ------------------------------------------------------------------------------------------ | ---------------------------- | ------------------------------------- |
| [§2](#2-terrain--line-of-sight)    | Tokens (Flame, Signal, T.P., …) never block LOS                                            | FAQ                          | Clarification                         |
| [§2](#2-terrain--line-of-sight)    | Boundaries of blocking hexes block LOS                                                     | FAQ                          | Clarification                         |
| [§4](#4-agent-turn)                | Armor Bolt effects resolve before wounds are inflicted                                     | FAQ                          | Clarification                         |
| [§4](#4-agent-turn)                | GD symbol also used for Search (dice table footnote)                                       | Rulebook p.20/p.28 vs p.17   | Rulebook internal inconsistency       |
| [§5](#5-agent-conditions)          | HP **and ammo** capped at printed/starting maximum                                         | FAQ                          | Clarification                         |
| [§6](#6-weapons-powers--items)     | Limited-ammo weapons replaceable by any; infinite-ammo only by infinite-ammo               | FAQ (Tricks & Tips)          | Official restriction (house-ruleable) |
| [§6](#6-weapons-powers--items)     | Armoury tokens: discard on move-over → random Improved/Alien weapon at next Reinforcements | FAQ (color mapping inferred) | Rule missing from rulebook            |
| [§6](#6-weapons-powers--items)     | Drones cannot be Engaged; disengage without Evade test                                     | FAQ                          | Correction                            |
| [§6](#6-weapons-powers--items)     | Sentry-Gun/GD-209 attack die is RED, not green                                             | Errata (rulebook p.26/27)    | Image correction                      |
| [§7](#7-optional-rules)            | Remove one Close Encounter #1 card per Core Set mission for easier/faster play             | FAQ (Tricks & Tips)          | Official difficulty variant           |
| [§7](#7-optional-rules)            | Short version of Mission 5 available (site Utility/Missions)                               | FAQ (Tricks & Tips)          | Official difficulty variant           |
| [§10](#10-the-aliens)              | Alien/signal with no legal walking path stays put                                          | FAQ                          | Confirmation of rulebook rule         |
| [§12](#12-card-clarifications-faq) | "Attack twice" AI: second attack vs same target, else same-distance target                 | FAQ                          | Clarification                         |
| [§12](#12-card-clarifications-faq) | Xeno-Grey: not activatable by another Xeno-Grey; immune to "Save The Master"               | FAQ                          | Clarification                         |
| [§12](#12-card-clarifications-faq) | Xeno-Beast rage: swap to Enraged card at full health                                       | FAQ                          | Clarification                         |
| [§12](#12-card-clarifications-faq) | Reinforced Armor: shield tokens must absorb hits first                                     | FAQ                          | Clarification                         |
