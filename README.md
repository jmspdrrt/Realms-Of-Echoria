# Realms of Echoria

> *A living text-based fantasy MMO powered by Claude. 140+ systems. 28 named NPCs. A world that remembers what you do.*

**Version 21** · Claude.ai Skill · by [@marrowleaf](https://x.com/marrowleaf)

---

## What is this?

Realms of Echoria is a custom Claude.ai skill that turns Claude into a full Game Master for a persistent text-based MMO. Not a chatbot adventure — a real RPG engine with economies that respond to your actions, factions you can politically manipulate, and a world that grieves when named NPCs die.

It runs entirely through conversation. No server. No install. Just Claude.

---

## Getting Started

### Requirements
- [Claude Pro](https://claude.ai) or higher
- The `.skill` file from [Releases](../../releases)

### Installation
1. Download the latest `realms-of-echoria.skill` from [Releases](../../releases)
2. In Claude.ai, go to **Settings → Skills → Install from file**
3. Select the `.skill` file and confirm

### Starting a New Game
Open a new Claude chat and type any of the following:

```
let's play
new game
start a new character
```

Claude will walk you through character creation step by step:

1. **Name** — what's your character called?
2. **Race** — choose from 8 races, each with unique stat bonuses
3. **Class** — choose from 9 classes with distinct playstyles
4. **Stats** — distribute 3 free points after race modifiers apply
5. **Backstory** *(optional)* — any enemies? a guild debt? a lost family member?

You'll start in **Thornwall Village** with a class-appropriate weapon, basic armour, 3 Health Potions, and 10 Gold.

### Resuming a Game
At the end of any session, type `save`. Claude outputs a full save block — copy and paste it at the start of your next session to resume exactly where you left off.

### Roguelite Mode
Want permadeath? Type `roguelite` instead of starting a normal game. See [Roguelite Mode](#-roguelite-mode) below.

---

## Races

| Race | Stat Modifiers | Bonus |
|------|---------------|-------|
| **Human** | +1 to all stats | No penalty — fully versatile |
| **Elf** | +2 AGI, +1 INT, -1 STR | Rarely surprised in combat |
| **Dwarf** | +2 STR, +2 CON, -1 AGI | +5 Mining & Smithing, stone-sense in caves |
| **Half-Orc** | +3 STR, +1 CON, -2 INT | Survive at 1 HP once per session when downed |
| **Halfling** | +2 AGI, +1 LCK, -1 STR | +5 Thieving & Cooking, reroll one LCK check per session |
| **Tiefling** | +2 INT, +1 CHA, -1 CON | -20% fire damage taken |
| **Gnome** | +3 INT, +1 LCK, -2 STR | +5 Crafting & Enchanting, can repair any mechanical device |
| **Dragonborn** | +2 STR, +2 CHA, -1 AGI | Elemental breath attack 1x per combat (choose element at creation) |

---

## Classes

| Class | Role | Primary Stats | Starting Skills |
|-------|------|--------------|----------------|
| **Warrior** | Tank / DPS | STR, CON | Bash, Shield Wall, War Cry |
| **Rogue** | Stealth / Burst | AGI | Backstab, Pickpocket, Shadow Step |
| **Mage** | Arcane Power | INT | Fireball, Frost Nova, Arcane Surge |
| **Cleric** | Healer / Buffer | CHA, CON | Heal, Smite, Divine Shield |
| **Ranger** | Ranged / Survival | AGI, INT | Arrow Shot, Track, Animal Bond |
| **Warlock** | Dark / DoTs | INT, CHA | Drain Life, Hex, Shadow Bolt |
| **Paladin** | Holy Warrior | STR, CHA | Judgement, Lay on Hands, Consecrate |
| **Necromancer** | Death Magic | INT | Raise Dead, Bone Spear, Death Coil |
| **Bard** | Support / Debuff | CHA, AGI | Inspire, Dissonant Scream, Charm |

Each class unlocks a **subclass specialisation at Level 5** (e.g. Warrior → Guardian or Berserker) and additional talent tree perks at Levels 10, 15, and 20.

---

## Systems

### ⚔️ Combat

Turn-based with real tactical depth.

- **Positioning** — choose Frontline, Midline, or Backline each fight. Melee classes deal more from Frontline; mages and ranged deal more from Backline. Repositioning costs a half-action.
- **Momentum** — a 0–5 meter that builds as you land hits, crit, and kill. At 5 you enter **Flow State**: guaranteed hit, no cooldown on your next skill, narrated cinematically.
- **Combo Attacks** — at Momentum 3+, chain two actions in one turn. Shadow Step → Backstab. Frost Nova → Fireball (frozen targets take bonus damage).
- **14 Status Effects** — Burning, Frozen, Shocked, Poisoned, Bleeding, Stunned, Feared, Charmed, Cursed, Hexed, Rooted, Silenced, Weakened, Enraged. Multiple statuses stack.
- **Flanking** — player + hireling both at Frontline = +15% damage for both.

### 🌍 World

| Zone | Level | Description |
|------|-------|-------------|
| Thornwall Village | 1–3 | Starting hub — inn, shops, quest board, property agent |
| Ashwood Forest | 2–5 | Wolves, bandits, ruins. Rich in herbs and timber |
| The Goblin Warrens | 3–6 | Underground tunnels and traps. Copper and iron ore |
| Marefield Coast | 5–8 | Fishing village, smugglers, sea caves |
| Stoneback Mountains | 6–10 | Dwarven ruins, trolls, mithril ore |
| The Whispering Desert | 8–12 | Ancient tombs, scorpions, hidden vaults |
| The Blighted Moor | 10–15 | Undead, witches, cursed earth, death runes |
| The Ember Wastes | 12–16 | Volcanic landscape, fire elementals |
| The Sunken City | 15–20 | Ancient civilisation, constructs, underwater sections |
| The Frostpeak Spire | 17–20 | Frozen tower, ice dragons, Legendary gear |
| The Ashen Throne | 20+ | End-game dungeon — World Boss: Ignatharax |
| The Void Rift *(secret)* | 20+ | Found via lore quest — chaos runes, reality breaks |

### 🌦️ Weather

10 weather types that each affect **combat, gathering, and exploration** simultaneously.

| Weather | Combat | Gathering | Exploration |
|---------|--------|-----------|-------------|
| Clear | No modifiers | +5% Herbalism XP | +1 discovery roll |
| Rain | Fire spells -10% dmg | +10% Fishing catch rate | Tracks wash away |
| Storm | Lightning enchants +20% dmg | Fishing +15%, Herbalism -10% | Mountain paths dangerous |
| Blizzard | -2 AGI all combatants | Mining -20% | Some paths blocked entirely |
| Fog | Stealth +20%, ranged -20% | Herbalism +10% | Random encounters +30% |
| Blood Moon *(rare)* | +20% all dmg, undead +10 HP | Blood Moon Herb spawns | Undead wander into settled zones |
| Flood | Ranged -10% | Fishing spots move inland | Coastal zones altered |
| High Wind | Ranged -40%, flying enemies advantage | Woodcutting harder | Mountain travel blocked |

**Combo effects**: Fog + Night stacks stealth to +30%. The rarest combo — Blood Moon + Storm — is called the Red Storm. Survive a fight during it and earn a unique achievement.

### ⚗️ Gathering Skills

9 OSRS-style skills levelled 1–99 independently of your combat level. Reaching 99 earns a **Skill Cape** with a unique passive. All 99s earn the **Max Cape**.

| Skill | Stat | What You Gather |
|-------|------|----------------|
| Mining | STR | Ore — Copper through Runite |
| Woodcutting | AGI | Logs — Regular through Magic Trees |
| Fishing | LCK | Fish — Shrimp through Abyssal Eel |
| Cooking | INT | Cook raw food — burn chance decreases with level |
| Herbalism | INT | Herbs — primary ingredient for potions |
| Smithing | STR | Smelt ore into bars, forge weapons and armour |
| Crafting | INT | Armour, jewellery, and tools from raw materials |
| Thieving | AGI | Pickpocket NPCs, steal from stalls, crack vaults |
| Enchanting | INT | Infuse gear with runes — Fire, Ice, Shadow, Chaos, and more |

### 🏛️ Factions

Eight factions to build standing with (Hostile → Neutral → Friendly → Honoured → Exalted). Two pairs are mutually exclusive.

| Faction | What They Offer |
|---------|----------------|
| **Crown's Vanguard** | Armory access, bounty reduction, pardons, legal contracts |
| **Shadowmere Guild** | Fence stolen goods, heist contracts, bounty laundering |
| **Ember Circle** | Spell scrolls, arcane research, enchanting discounts |
| **Children of the Root** | Animal companions, nature healing, disease-free herb patches |
| **Iron Brotherhood** | Mercenary contracts, weapon discounts, raid invites |
| **Sunken Archive** | Sunken City access, lore quests, golem ally |
| **Bone Court** | Undead allies, Moor safe passage, death runes |
| **Merchant Consortium** | 30% better sell prices, bulk items, trade routes |

Each faction has a **5-act questline** and a unique Exalted perk. Crown's Vanguard and Shadowmere are mutually exclusive; so are Children of the Root and Bone Court.

### 📈 Dynamic Economy

The market responds to what you do. Prices shift and merchants notice.

- Sell 20+ units of a material in one session → that market goes **Oversupplied** (lower sell prices for 2 sessions)
- Sell 50+ units → market **Crashes** (4 sessions, merchants complain out loud)
- A Pirate Blockade hits Marefield → all goods there go **Inflated**
- Invest in the local tavern → earn passive gold per session and get early warnings on world events

**Investment types**: Tavern, Merchant Stall, Smithy, Apothecary, Faction Coffers, Town Defence Fund, Sea Trade Route, Black Market.

### 🏛️ Political Influence

Build influence (0–100) in every zone through quests, donations, arena wins, and faction work.

| Influence | What Unlocks |
|----------|-------------|
| 25 | +5% better prices, Town Crier mentions you positively |
| 50 | Install minor officials (inn keeper, guard captain) |
| 75 | Call a Town Council vote, veto one world event |
| 90 | Control trade relationships, deny rival factions entry |
| 100 | Install a leader of your choice, earn 50g/session from zone income |

Trigger or prevent faction wars. Broker peace treaties. At Dominant Influence in 3+ zones before the **Throne Quest** you unlock a fifth ending: the Power Behind the Throne.

### 🏠 Housing

Buy a home from Level 5+. Four locations from a 500g Thornwall cottage to a 5,000g Sunken City villa.

| Upgrade | Cost | What It Does |
|---------|------|-------------|
| Bedroom | 200g | Rest restores full HP |
| Kitchen | 300g | Cook with no burn chance |
| Herb Patch | 400g | 3 herbs grown passively per session |
| Enchanting Table | 500g | Enchant gear at home |
| Workshop | 600g | Craft and smith at home with +5% success |
| Trophy Room | 200g | Display boss drops — each gives a passive buff |
| Pet Stable | 300g | House up to 5 pets; inactive pets train passively |
| Portal Stone | 1,000g | Teleport home once per day from anywhere |
| Alchemy Lab | 400g | Advanced brewing at home |
| Vault | 750g | 50 extra storage slots |

### ⛵ Sailing

Unlock at Marefield Coast (Level 5+).

- **Ships**: Fishing Skiff → Sloop → Brigantine → Galleon → Ghost Ship (boss drop)
- **Sea zones**: Marefield Shallows → Amber Shallows → The Iron Sea → The Drowned Archipelago → The Abyssal Deep (Kraken boss, 1,500 HP)
- **Naval combat**: Manoeuvre for range, broadside, or board and fight the crew directly
- **Deep-sea fishing**: Swordfish, Shark, Giant Squid, Abyssal Eel

### 🗺️ Procedural Dungeons

Type `dungeon` to generate one. Every dungeon is unique.

- **Types**: Goblin Warrens, Undead Crypt, Ancient Ruins, Bandit Stronghold, Cave System, Arcane Laboratory, Sea Cave
- **Room types**: Combat, Puzzle, Treasure, Rest Point, Secret (always Rare+ loot), Mini-boss
- **Modifiers**: Cursed, Empowered, Haunted (enemies immune to physical), Darkness, Corrupted (status effects reflect back at 50%)
- **Delver's Streak**: Clear 5 consecutively without dying for the "Dungeon Crawler" title

### 💀 Roguelite Mode

Type `roguelite` to start a permadeath run tracked separately from your main character.

- **Start perks**: Iron Start, Blessed (LCK 14), Scholar's Edge, Well-Funded, Ghost Step, or Legacy Perk from a previous run
- **Difficulty tiers**: Casual (0.75×), Standard (1×), Brutal (1.5×), Ironclad (2×, no potions drop)
- **Scoring**: Levels, bosses, skills levelled, factions, sessions survived — multiplied by difficulty
- **Leaderboard**: Your top 5 runs tracked and displayed at the end of each run
- **Legacy bonuses**: Cross into future runs *and* your standard game — score 8,000+ pts and your standard character's death penalty drops from 50% gold to 30%
- **The Drifter**: A secret class unlocked after 5 completed runs

### 🙏 God Worship

Five gods, five devotion tracks (0–100). Build devotion through shrine offerings, aligned actions, and divine quests.

| God | Domain | Champion Power |
|-----|--------|---------------|
| **Osrick** | Memory & Death | Dead enemies sometimes speak one final truth |
| **Nael** | Transition & Change | Reroll any failed check once per session |
| **Verath** | Nature & Growth | Animals never aggro you unless attacked first |
| **The Ember** | Power & Ambition | First attack each combat deals +30% damage |
| **The Fifth God** *(secret)* | Dreams & the Unnamed | Dream Journal entries predict real events |

### 🔁 Prestige Cycles

After completing the main story, prestige into a new character in the same world. The world remembers.

- **Cycle 2**: NPCs reference your previous character by name. Enemies are 10% stronger.
- **Cycle 3**: New zone content unlocks. Enemies adapt to your known fighting style.
- **Cycles 4–5**: Mythic gear tier, Class Triple Specialisation, the Fifth God's story concludes.

---

## Commands

Every command is typed naturally in conversation — no slash prefix needed.

### Character
| Command | What It Does |
|---------|-------------|
| `stats` / `sheet` | Full character sheet |
| `inventory` / `inv` | Show your inventory |
| `skills` | Unlocked class skills and cooldowns |
| `gathering` | All 9 gathering skill levels |
| `talent` | Subclass and talent tree perks |
| `equipment` | All gear slots including accessories |
| `achievements` | View unlocked achievements |

### World & Exploration
| Command | What It Does |
|---------|-------------|
| `map` | Nearby zones and travel options |
| `weather` | Current weather and its mechanical effects |
| `quests` | Active and completed quests |
| `rest` | Rest to restore HP and advance time |
| `news` | Town Crier bulletin for this area |
| `world event` | Active world events in the region |
| `codex` / `encyclopedia` | Your lore collection |

### Combat & Action
| Command | What It Does |
|---------|-------------|
| `attack [X]` | Initiate or continue combat |
| `duel [NPC]` | Challenge an NPC to a formal duel |
| `talk to [NPC]` | Begin NPC dialogue |
| `mine` / `fish` / `chop` | Begin a gathering activity |
| `craft [item]` | Attempt to craft something |
| `enchant [item]` | Enchant gear at an enchanting table |
| `brew` | Open the alchemy lab |

### Economy & Politics
| Command | What It Does |
|---------|-------------|
| `market` | Local market prices and trends |
| `invest` | Invest in a business or faction |
| `influence` | Your political influence in this zone |
| `install [NPC]` | Attempt to install a political figure |

### Home, Pets & Mounts
| Command | What It Does |
|---------|-------------|
| `home` | Interact with your player home |
| `pet [name]` | Interact with a pet |
| `mount` | View, summon, or manage mounts |

### Factions & Social
| Command | What It Does |
|---------|-------------|
| `relationships` | NPC relationship standings |
| `hire` | Browse NPC party members for hire |
| `party` | Your current hired party |
| `wanted` | Bounty level and options |
| `heist` | Heist contracts (Shadowmere Guild required) |
| `contract` | Assassination contracts (Shadowmere Honoured+) |

### Dungeons, Arena & Challenges
| Command | What It Does |
|---------|-------------|
| `dungeon` | Generate and enter a procedural dungeon |
| `arena` | Enter the arena or check standings |
| `sail` | Sailing and the naval map |
| `gamble` | Gambling and mini-games at a tavern |
| `daily` / `weekly` | Active challenges |

### Roguelite
| Command | What It Does |
|---------|-------------|
| `roguelite` | Start a permadeath run |
| `leaderboard` | View your roguelite run leaderboard |

### Meta
| Command | What It Does |
|---------|-------------|
| `save` | Output your full save block to copy |

---

## Architecture

v21 was refactored from a single 8,500-line file into a modular structure. Claude loads reference files on demand — only what's needed for the current action.

```
realms-of-echoria/
├── SKILL.md                  # Core — GM rules, character creation, quick reference
└── references/
    ├── character.md          # Races, classes, subclasses, talent trees
    ├── combat.md             # Positioning, momentum, status effects, combos
    ├── world.md              # Zones, travel, weather, sailing
    ├── gathering-crafting.md # Gathering skills, crafting, alchemy, enchanting
    ├── npcs-factions.md      # NPCs, factions, quests, heists, karma
    ├── systems.md            # Housing, pets, mounts, arena, dungeons, bounty
    ├── progression.md        # Raids, bosses, prestige, god worship, codex
    ├── economy.md            # Dynamic market, investment system
    ├── politics.md           # Political influence, town control, throne quest
    ├── roguelite.md          # Permadeath mode, leaderboard, legacy bonuses
    └── lore-meta.md          # World history, NPC roster, save system, tone settings
```

---

## Version History

| Version | Highlights |
|---------|-----------|
| **v21** | Modular architecture · Dynamic economy · Political influence · Roguelite mode · Combat overhaul (positioning + momentum + 14 status effects) · Formal duelling · Weather combo interactions |
| **v20** | World Encyclopedia · NPC death & grief system · Postal network · Stealth layer · God worship · Dream events |
| **v15** | Sailing · Procedural dungeons · World events · Arena gladiator system · NPC hiring · Blacksmithing mastery |
| **v10** | Housing · Mounts · Alchemy lab · Pet breeding · Bounty hunting · Heists · Assassination contracts |
| **v1**  | Initial release — 9 classes, 9 gathering skills, factions, turn-based combat |

---

## Links

- **X / Twitter**: [@marrowleaf](https://x.com/marrowleaf)
- **Claude.ai**: [claude.ai](https://claude.ai)

---

*Built by @marrowleaf · 2025*
