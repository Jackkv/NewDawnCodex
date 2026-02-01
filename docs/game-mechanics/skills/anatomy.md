![Anatomy](../../assets/Flag_anatomy.gif){ align=right }

# Anatomy

Increases melee damage and improves bandage healing effectiveness.

## Overview

Anatomy is a versatile support skill that enhances both offensive combat and healing. It's essential for all physical combat builds and significantly improves bandage healing.

## Active Use

When you actively use the Anatomy skill on a target:

- **Target Range**: 8 tiles
- **Success**: Reveals the target's approximate Strength, Dexterity, and Stamina percentage
  - At 65.0+ skill: Also shows stamina percentage
  - Accuracy improves with higher skill (margin of error decreases from ±25 at 0 skill to ±0 at 100 skill)
- **Failure**: "You can not quite get a sense of their physical characteristics."
- **Cooldown**: 10 seconds

## Effects

### Combat Benefits

- **Bonus Damage** - Increases damage on all melee attacks
  - Formula: `anatomyBonus = value * 0.500 + (value >= 100.0 ? 5.00 : 0.0)`
  - At 100 skill: Adds 50% + 5.00 = **55% damage bonus**
  - Damage increases linearly from 0-100 skill: 0.5% per skill point, plus 5% bonus at GM
- **Combines with Tactics and Strength** - All bonuses stack multiplicatively

### Healing Benefits

- **Improved Bandage Healing** - Increases HP restored per bandage
- **Cure Poison** - Can cure poison with bandages (requires 60+ Healing and 60+ Anatomy)
- **Resurrect** - Revive dead players/pets with bandages (requires 80+ Healing and 80+ Anatomy)

## Training

### Passive Gains

Anatomy improves automatically during combat:

- Gains during any physical combat
- Trains alongside weapon skills
- No special actions needed

### Active Training

- Use Anatomy skill on creatures
- Examine corpses
- Practice during hunts

!!! tip "Natural Progression"
    Anatomy trains naturally as you fight. Just keep it locked up and it will reach 100 through normal combat.

## Damage Calculation Details

### Damage Formula

In the classic damage system:

```
damage = damage + damage * ((tactics - 50.0) / 100.0)
damage = damage + damage * modifiers
```

Where `modifiers` include:

- **Strength**: `1% per 5 strength` (e.g., 100 STR = 20% bonus)
- **Anatomy**: `1% per 5 anatomy` (e.g., 100 Anatomy = 20% bonus)
- **Lumberjacking** (axes): Additional bonus

## Bandage Healing Formula

### Healing Amount

When using bandages, the amount healed is calculated as:

**System**:
```
min = anatomy / 5.0 + healing / 5.0 + 3.0
max = anatomy / 5.0 + healing / 2.0 + 10.0
toHeal = min + random * (max - min)
```

### Example Healing at 100/100

With 100 Healing and 100 Anatomy:

- **Pre-AOS**: Heals between 43.0 and 30.0 HP

### Poison Curing

Requirements for curing poison with bandages:

- Healing skill: 60+
- Anatomy skill: 60+
- Success chance: `(healing - 30.0) / 50.0 - poisonLevel * 0.1 - slips * 0.02`
- Higher skills = better success rate

### Resurrection

Requirements for resurrection with bandages:

- Healing skill: 80+
- Anatomy skill: 80+
- Success chance: `(healing - 68.0) / 50.0 - slips * 0.02`
- Must be next to corpse

## Related Skills

**Essential Combat Pair:**

- [Tactics](tactics.md) - Damage multiplier
- Any weapon skill - Attack capability
- [Healing](healing.md) - Bandage effectiveness

**Full Combat Package:**

- Weapon Skill: 100
- Tactics: 100
- **Anatomy: 100** ⭐
- Healing: 100

## Character Templates

### Warrior

- Weapon Skill: 100
- Tactics: 100
- **Anatomy: 100** ⭐
- Healing: 100
- Parrying: 100
- Resisting Spells: 100
- Magery: 100

### Archer

- Archery: 100
- Tactics: 100
- **Anatomy: 100** ⭐
- Healing: 100
- Hiding: 100
- Tracking: 100
- Resisting Spells: 100

### Healer

- Healing: 100
- **Anatomy: 100** ⭐
- Magery: 100
- Meditation: 100
- Resisting Spells: 100
- Evaluating Intelligence: 100
- Wrestling: 100

## PvP Importance

In PvP, Anatomy is crucial:

- Maximum damage potential
- Better healing efficiency
- Cure poison in combat
- Essential for competitiveness

## Importance

⭐⭐⭐⭐⭐ (Essential for all combat builds)

---

**Related Pages:**

- [Combat Skills Overview](index.md#combat-skills)
- [Tactics](tactics.md)
- [Healing](healing.md)
- [Combat System](../combat.md)
