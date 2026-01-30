# Plan: New Dawn Wiki Documentation

Based on the patch notes (49 patches, 1,577 lines), I need to document ~20 custom systems and major UO deviations that are currently missing or incomplete in your wiki. The core game mechanics are well-covered, but New Dawn's unique features are largely undocumented.

## Steps

1. **Create docs/custom-systems section** with index and 8 flagship feature pages: codex-rifts.md, pirate-adventures.md, capture-the-flag.md, archaeology.md, conquest-of-virtues.md, spirit-summoner.md, gardening.md, achievements.md

2. **Create game-mechanics/pvp subsection** with murder-system.md (short/long-term kills, forged pardons, dungeon bans, stat loss 20-40%) and index.md overview

3. **Expand game-mechanics/crafting.md** with BOD points system, Tailoring Guild dyes (10k gold at GM, 250 dungeon materials per dye), and gardening/sheep farming mechanics

4. **Update game-mechanics/combat.md** with stamina-loss-on-hit system (replaces dex penalty), archery snare ability (80+ Anatomy/Archery, 25% at GM, 3s immobilize), parrying shield bash, explosion potion changes (1.5s delay, min damage bonus from alchemy), and poison vs immune mobs (50% chance at GM)

5. **Create game-mechanics/currencies.md** documenting Champion Tokens, Harrower Shards, Pirate/Rift/Codex currencies, and Dawn reward vendor locations

6. **Expand game-mechanics/magic.md** with comprehensive Spirit Speak section: special 5th circle summons, boosted 8th circle stats, BS/EV poison chance (10-40%), GM controllability, and Animal Lore synergy (Patch 1.0)

## Further Considerations

1. **Create docs/getting-started/whats-different.md** as quick reference for classic UO players? This would summarize combat changes, custom systems, and QoL improvements in one page.

2. **Housing documentation** - expand world/index.md or create dedicated world/housing.md with decay (14 days), IDOC windows (1-3hr random), 5-tile spacing, custom house types, and co-owner system?

3. **Update mkdocs.yml** navigation structure - should I add the new "Custom Systems" section at top-level or nest it under "Game Mechanics"? Current structure is Getting Started → Game Mechanics → Items → World → Community.

## Research Summary

### Currently Well-Documented
- Core Game Mechanics: Skills, Combat, Magic (8 circles), Stats
- Crafting: Blacksmithy, Tailoring, Carpentry, Alchemy, Inscription
- World: Town/dungeon structure exists (Britain, Moonglow, Trinsic, Vesper, Covetous, Despise, Shame)
- Getting Started: New player guide, character creation, controls

### Critical Gaps (Completely Missing)

**Custom Systems:**
- **Codex Rifts** (Patch 0.27): Rift spawns (1-50% gate chance based on fame), instanced content, 60min timer, 3 of 8 active champs, rift masters drop statues, Felucca rules, rift shards currency
- **Pirate Adventures** (Patch 0.16+): Multiple map tiers, instanced encounters, bosses (Ancient Drowner, Captain Grimjaw), pirate cannons, smuggler merchants (Patch 0.43)
- **Capture the Flag** (Patch 0.26): 10v10 PvP, two maps, point system, automated scheduling, stat tracking, flag mechanics (120s carrier timer, 20s capture cooldown)
- **Archaeology System** (Patch 0.43): Map fragments from fishing, journal/book page clues, 3-stage excavation (Shovel→Pick Hammer→Brush), requires Mining 80-90/Cartography 70+/Inscription 70+/Item ID 80+, artifact rarity tiers
- **Conquest of the Virtues** (Patch 0.42): Four ruined locations (Britain, Trinsic, Shadowlords, Moonglow), guild-based territory control
- **Gardening/Plants** (Patch 0.44): Seeds from animals, fertile dirt, cotton/flax farming, sheep hunger system (wool production 1.5-12 hours based on food)
- **Tailoring Dyes** (Patch 0.33): Dungeon-specific materials (250 per dye - Patch 0.45), Tailoring Guild membership (85.1+), tailors dye kit (10k gold at GM), unique hues per dungeon
- **Achievement System** (Patch 1.0): Completely rewritten, point-based progression, titles and item rewards, multiple categories

**Modified Classic Systems:**
- **Spirit Summoner/Spirit Speak** (Patches 0.15, 0.16, 0.18, 0.29, 0.48, 1.0): Major custom mechanic - special 5th circle creatures, boosted 8th circle stats/skills, BS/EV affected (poison 10-40%, controllable at GM), summon healing buffed, Animal Lore synergy added (Patch 1.0)
- **Murder/PvP System** (Patch 0.31): Long-term vs short-term murders, forged pardons (Yew courthouse), dungeon bans (15min for 5+ murders), decay times (24-48 logged hours), stat loss (20-40% scaling)
- **Housing System** (Multiple patches): Decay (14 days), IDOC mechanics (1-3hr random window), custom house types, 1 house per account, 5-tile spacing (Patch 0.44), co-owner system (all accounts - Patch 0.51)
- **BOD System** (Patch 0.40): Points-based rewards, specific tailoring rewards with point values (1-700 points), runic tools, dyes, power scrolls, books no longer blessed
- **Champion/Harrower** (Multiple patches): Champion tokens & Harrower shards currency, Harrower scroll system (Patch 0.36), temp guild region option, reward vendors in Dawn, champ leash (60 tiles)

**Special Mechanics:**
- **Archery Snare** (Patch 0.51): 80+ Anatomy & Archery, 25% at GM, 3s immobilize + spell disruption, 20s cooldown, 15 stamina cost
- **Parrying Shield Bash** (Patch 0.15): Custom ability
- **Taming Quest** (Patch 0.25): Animal bonding quest, sketch book, bonding slot rewards, requires 80+ Taming & Lore
- **Escort System** (Patch 0.46): Distance-based rewards, "Seekers of Adventure" dungeon escorts, possible artifact clue rewards

### Key Combat/Balance Changes from Classic UO
- **No Dexterity Penalty**: Replaced with stamina loss on damage based on armor type and hit location
- **Archery**: 500ms delay standing still, snare ability at 80+
- **Explosion Potions**: 1.5s delay, alchemy bonus to min damage (not total), min/max 15-20 at GM vs players
- **Poison**: GM Poisoning has 50% chance vs immune mobs, GM Magery+Poison can land lethal (1% within 2 tiles) or deadly (10% within 3 tiles)
- **PvP Spell Damage**: Custom min/max ranges, Magic Resist cuts damage by 1/3 (not 1/2)
- **Weapon/Armor**: Converted to UOR era values (Patch 0.16)
- **Stamina**: Running doesn't drain stamina (removed Patch 0.29)
- **Armor Damage**: Hit location probabilities - Chest 40%, Arms 20%, Legs 15%, Hands/Head 10%, Neck 5%

### Skills & Progression Changes
- **Tracking**: Distance-based success, 100 tiles at GM (50 in dungeons), region/level restricted
- **Stealth**: Auto-stealth option at 80+, step counter displayed
- **Lumberjacking**: Special wood types (Oak, Ash, Yew) with bark/amber drops, 3-tile range
- **Mining**: 3-tile range (Patch 0.49)
- **Skill Gains**: Custom global modifiers, slowed for 3x GM or less

### World & Systems Changes
- **Paragons**: Enabled, 100% loot drop, double gold, can't be hirelings
- **Young Player System**: Ocllo-based, 120 hour limit OR 450 total skills OR leaving Ocllo OR murder OR crafting 80+ OR voluntary exit, can rejoin 2x per account
- **Account Limits**: 3 accounts per Discord, 1 house per account, multi-client dungeon restrictions, 1 account in Codex Rift
- **Light Levels**: Day/night cycle, moon phases affect darkness (8 phases lasting multiple in-game days), Night Sight spell skill-based brightness, greater night sight potions (8 spider silk, 15-25min)
- **Boats**: 2 per account, smooth sailing, key-based control, 6400 weight cargo holds (Patch 0.49)

### Currency System
- **Champion Tokens**: From champion spawns
- **Harrower Shards**: From harrower
- **Pirate Currency**: From pirate map instances
- **Rift Shards/Codex Shards**: From Codex Rifts (rift masters give 1-5 based on damage, low chance from any rift mob)
- **Reward Vendors**: Located in Dawn (Event Center)

### Missing Documentation by Priority

**Immediate (Most Impactful):**
1. Spirit Summoner mechanics (major custom system, completely undocumented)
2. Codex Rifts (flagship content)
3. Pirate Adventures (popular recurring content)
4. Murder/PvP system (affects all players)
5. Housing comprehensive guide

**High Priority:**
6. CTF guide
7. Archaeology system
8. BOD system with New Dawn specifics
9. Champion/Harrower mechanics and rewards
10. Tailoring dyes

**Medium Priority:**
11. Conquest of the Virtues
12. Gardening/Plants
13. Achievement system
14. Taming quest
15. Custom combat abilities (Snare, Shield Bash)

**Low Priority (but needed):**
16. Seasonal events (base system exists but minimal content)
17. Escort system updates
18. Daily rares (currently disabled - Patch 0.46)
19. Reward bags (Beta bags, Charter Member bags, Vanguard rewards - Patch 1.0)

## Organizational Structure Proposal

### Option A: Top-Level "Custom Systems" Section (Recommended)
```
mkdocs.yml:
- Getting Started
- Game Mechanics
- Custom Systems     ← NEW
  - Overview
  - Codex Rifts
  - Pirate Adventures
  - Capture the Flag
  - Archaeology
  - Conquest of Virtues
  - Spirit Summoner
  - Gardening
  - Achievements
- Items
- World
- Community
```

### Option B: Nest Under "Game Mechanics"
```
mkdocs.yml:
- Getting Started
- Game Mechanics
  - Core Mechanics
  - Custom Systems   ← NEW SUBSECTION
    - (same pages as above)
- Items
- World
- Community
```

### Recommendation
**Option A** is better because:
1. Highlights New Dawn's unique features at top-level
2. Easier for returning players to find "what's new"
3. Separates classic UO mechanics from custom content
4. Better matches user's intro text structure (Classic Foundation vs Custom Content)

## Content Writing Guidelines

For each new page:
1. Start with brief overview (1-2 paragraphs)
2. Include "How to Access" section
3. Document requirements (skills, items, level restrictions)
4. Explain mechanics step-by-step
5. List rewards/benefits
6. Add tips & strategies section
7. Note relevant patch numbers for updates
8. Cross-link to related pages

Tone: Informative but engaging, assume reader knows basic UO but not New Dawn specifics
