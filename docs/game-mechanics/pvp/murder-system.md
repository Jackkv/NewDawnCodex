# PvP & Murder System

New Dawn features a robust PvP and murder system with meaningful consequences for criminal activity. Understanding these mechanics is essential for both aggressors and victims navigating the dangers of Felucca.

## Overview

Player vs Player combat is enabled throughout New Dawn's single facet (Felucca). The murder system tracks kills, applies consequences, and creates a dynamic criminal ecosystem where actions have lasting impacts.

## Murder System

### Short-Term vs Long-Term Murders

New Dawn distinguishes between recent and historical kills:

**Short-Term Murders:**

- Recently committed murders
- Decay over **24-48 logged hours** (time actually played)
- Can be removed with forged pardons
- Contribute to stat loss calculations
- Affect temporary red status

**Long-Term Murders:**

- Murders that have "aged" past short-term
- **Permanent once you reach 5 long-term murders**
- Cannot be removed or decayed
- Permanent murderer status at 5+ long-term
- Represents your true criminal history

!!! warning "Permanent Consequences"
    Once you reach 5 long-term murders, you are permanently marked as a murderer. This is irreversible through normal decay.

### How Murder Counts Work

**Receiving a Murder Count:**

1. You kill another player
2. Victim can report you for murder (if eligible)
3. You receive 1 short-term murder count
4. Murder announcements visible to all players

**Who Can Report:**

- Players who were killed by another player
- **Cannot report if you killed yourself** (even if someone dealt 99% damage)
- Must not have been in consensual combat (duel, guild war, etc.)

**Murder Count Limits:**

- No maximum number of murders
- Each murder count contributes to penalties
- Stat loss scales with murder count

### Stat Loss System

Murderers suffer stat and skill penalties based on their short-term murder count:

**Stat Loss Formula:**

- Scales from **20% to 40%** based on short-term murders
- Applies to both stats (STR/DEX/INT) and skills
- Formula: Base 20% + (murder count × scaling factor)
- **Maximum:** 40% at 25+ short-term murders

**Example:**

- 5 short-term murders = ~24% stat/skill loss
- 15 short-term murders = ~32% stat/skill loss
- 25+ short-term murders = 40% stat/skill loss (maximum)

**When Applied:**

- Occurs upon death as a murderer
- Temporary penalty
- Can be restored (see below)

### Viewing Your Status

Use the **"I must consider my sins"** gump:

- Shows short-term murder count
- Shows long-term murder count
- Displays when you can use forged pardon
- Stat loss percentage
- Other criminal status info

### Forged Pardons

**What Are They:**

- Special items that clear your murder counts
- Found at the **Yew Courthouse**
- Single use
- Expensive or difficult to obtain

**How They Work:**

- Use on yourself
- Removes **all short-term murders**
- Sets **long-term murders to zero**
- Removes red (murderer) status if under 5 murders
- **Does not work if you have 5+ permanent long-term murders**

!!! tip "Pardon Strategy"
    Use forged pardons before hitting 5 long-term murders to avoid permanent murderer status.

## Dungeon Restrictions for Murderers

### 15-Minute Dungeon Ban

If you die in a dungeon with **5+ murders**, consequences apply:

**Ban Mechanics:**

- **All your accounts** (linked by IP and Discord) are banned from that specific dungeon
- Ban lasts **15 minutes** from time of death
- If you die in another dungeon, the timer resets to 15 minutes for all dungeons
- Attempts to enter during ban eject you to Dawn (Event Center)

**Linked Accounts:**

- Ban applies account-wide
- Linked by IP address
- Linked by Discord ID
- Prevents multi-client abuse

!!! warning "Multiple Dungeon Deaths"
    Dying in Despise resets the timer. Dying again in Covetous before those 15 minutes are up resets it again.

## Resurrection for Murderers

**Reds (murderers) can only resurrect at:**

- **Chaos Shrine** (specific location)
- Party/guild members with resurrection spells
- Wandering healers (sometimes)

**Cannot use:**

- Town healers
- Virtue shrines
- Most NPC healers

## Criminal Actions

### What Makes You Criminal

Actions that flag you as a criminal (gray):

**Criminal Actions:**

- Attacking innocent (blue) players
- Stealing from innocents
- Using beneficial acts on criminals
- Looting innocent corpses (old stealing rules apply)
- Using provo/discord on innocent players' pets

**Criminal Timer:**

- 2 minutes (120 seconds)
- Shown as a debuff icon
- Anyone can attack you freely
- Guards will kill you in town

### Permagray Status

Old stealing rules are enabled:

- Looting blue corpses can make you permagray
- Permagray lasts until your next death
- Can be attacked by anyone
- More severe than temporary criminal

## PvP Combat Rules

### Multi-Client Restrictions

- Cannot attack someone with multiple accounts simultaneously
- System detects and blocks multi-client PvP
- Helps maintain fair combat
- One account in dungeons for most content

### Fields and Area Damage

- Field spells (fire, poison, para) can damage anyone
- Purple potions don't stack
- Explosion potions can hit anyone
- Area effects don't discriminate targets

### Gates and Travel

- **Criminals CAN cast Gate Travel** (Patch 0.31, reverted Patch 0.29)
- Useful for escape or travel despite criminal status
- Other travel restrictions may apply

## Guard System

### Calling Guards

**NPCs can call guards if:**

- They have line of sight to the criminal
- Within **12 tiles** of the guard zone
- Actually see the criminal act

**What Guards Do:**

- Instantly kill criminals in guard zones
- Very powerful, unavoidable
- Clears criminal status through death

!!! tip "NPC Witnesses"
    NPCs need line of sight to call guards. Stay out of sight or eliminate witnesses before acting.

## Guild Wars

### War Declarations

- Guilds can declare war on each other
- War proposals and acceptances sent to Discord
- Creates structured, consequence-free PvP between guilds

**During Guild War:**

- No murder counts for killing enemy guild members
- No criminal flags
- Clean PvP between warring guilds
- Tracked and announced

## Harrower Guild Regions

When spawning a Harrower, you can create a **temporary guild region** (1 hour):

- Players not in your guild or allied appear **orange**
- Orange players are attackable without consequence
- Creates safe zone for your guild during Harrower
- Expires after 1 hour

## Town Safety

### Guard Zones

Most towns are protected by guards:

- Criminal actions result in instant death
- Guards are called by NPCs and players
- Very high damage, essentially instant kill

**Exception:** Bucs Den Inn

- Guard region removed
- Free PvP zone within the inn
- Dangerous but lawless

## Strategy & Tips

### For Murderers

- **Watch your count:** Stay under 5 long-term for reversal options
- **Use pardons strategically:** Before hitting permanent status
- **Plan dungeon trips:** 15-minute ban applies on death
- **Know resurrection spots:** Chaos shrine is your friend
- **Accept the risk:** Murder has consequences

### For Innocents

- **Report murders:** Make killers face consequences
- **Travel in groups:** Harder to target
- **Stay aware:** Watch for reds in dangerous areas
- **Use guards:** Stay near town protection when possible
- **Learn to fight back:** Best defense is a good offense

### For Everyone

- **Understand flags:** Know when you're criminal
- **Guild politics matter:** Wars provide clean PvP
- **Account linking:** Remember bans affect all accounts
- **Communication:** Coordinate with guild for safety

## Related Systems

- [Combat System](../combat.md) - Combat mechanics for PvP
- [Capture the Flag](../../custom-systems/capture-the-flag.md) - Structured PvP
- [Conquest of Virtues](../../custom-systems/conquest-of-virtues.md) - Guild PvP
- [Guilds](../../community/index.md) - Guild system and wars

## Patch History

The murder system has evolved significantly:

- **0.08:** Old stealing rules enabled, permagray system
- **0.29:** Mounts combat restrictions
- **0.29:** Resurrection limitations for reds
- **0.31:** Major murder system overhaul
  - Long-term vs short-term murders
  - Forged pardons introduced
  - Dungeon bans (15 min for 5+ murders)
  - Decay times (24-48 logged hours)
  - Stat loss scaling (20-40%)
  - Permanent status at 5 long-term
- **0.31:** Gate travel enabled for criminals
- **0.36:** Harrower guild region option
- **0.41:** Self-kill reporting fixed

For complete history, see the [patch notes](../../patchnotes.md).
