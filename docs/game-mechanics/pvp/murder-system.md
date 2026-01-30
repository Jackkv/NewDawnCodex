# Player Murder System Guide

## Overview

The murder system tracks player kills and applies consequences for those who engage in player killing (PKing). This system uses both **short-term** and **long-term** murder counts to regulate PvP behavior and provide pathways for redemption.

---

## How Murder Counts Work

### Important: Reporting is Required!

**Murder counts are NOT automatic.** When you kill another player, the victim receives a gump (dialog box) asking if they want to report you as a murderer. **Only if they choose to report you** will you receive murder counts.

- The gump appears **4 seconds** after death
- Victims can choose **"Yes"** (report) or **"No"** (don't report)
- If multiple players killed the victim, they can choose to report each one individually
- **Exception**: Members of the Thieves Guild cannot report murders (guards won't take reports of a thief's death)
- Once someone reports you, they cannot report you again for the same incident for **5 minutes**

When you ARE reported, you receive **two types** of murder counts:

### 1. Short-Term Murders

- **Duration**: Decays over time based on your total count
  - **Less than 5 murders**: Each count decays after **24 hours** of in-game play time
  - **5 or more murders**: Each count decays after **48 hours** of in-game play time
- **Purpose**: Tracks recent PK activity and determines eligibility for pardons
- **Decay**: Only decays while you're **logged in** (based on game time, not real time)

### 2. Long-Term Murders (Kills)

- **Duration**: **60 hours** of in-game play time
- **Purpose**: Your permanent murder record
- **Note**: Currently, long-term murders **do not automatically decay** (this may change)
- **Visibility**: This is your "Kills" count that other players can see

---

## Murder Count Decay System

### Key Points:

- Murder counts **only decay while you are online**
- The system checks for decay every **5 minutes**
- Counts decay **one at a time** as their timers expire
- When you log out, your decay progress is saved
- When you log back in, the system resumes tracking from where it left off

### Decay Timeline Examples:

**Example 1: Player with 3 short-term murders**

- Each murder will decay after 24 hours of play time
- Total time to clear all 3: **72 hours** of being logged in

**Example 2: Player with 6 short-term murders**

- First 2 murders decay at 48 hours each (while at 6→5, then 5→4)
- Remaining 4 murders decay at 24 hours each (while below 5)
- Total time to clear all 6: **(2 × 48) + (4 × 24) = 192 hours** of being logged in

**Example 3: Player with 10 short-term murders**

- First 6 murders decay at 48 hours each (from 10 down to 4)
- Remaining 4 murders decay at 24 hours each (below 5)
- Total time to clear all 10: **(6 × 48) + (4 × 24) = 384 hours** of being logged in

---

## Stat and Skill Loss on Resurrection

### Overview

If you have **5 or more short-term murders** when you die, you will suffer **stat and skill loss** upon resurrection. This penalty is **severe** and increases with the number of murders you have accumulated.

### How the Penalty Works

When you resurrect with 5+ short-term murders:

1. **Your stats (STR, INT, DEX) are reduced**
2. **Your skills are reduced**
3. **Your short-term murder count is reset to 0** (the penalty "pays off" your short-term murders)
4. You receive a message showing the exact percentage of loss

### Loss Calculation

The percentage of stat/skill loss is calculated as follows:

| Short-Term Murders | Loss Percentage | You Keep |
|-------------------|----------------|----------|
| **5** | 20.0% | 80% |
| **6** | 21.0% | 79% |
| **7** | 22.0% | 78% |
| **8** | 23.0% | 77% |
| **9** | 24.0% | 76% |
| **10** | 25.0% | 75% |
| **15** | 30.0% | 70% |
| **20** | 35.0% | 65% |
| **25+** | 40.0% (max) | 60% |

**Formula**: Base 20% + 1% per murder above 5 (capped at 40% loss)

### What Gets Reduced

#### Stats (STR, INT, DEX)

- Each stat is multiplied by the retention percentage (what you keep)
- **Minimum floor**: Stats won't drop below 10
- Example: With 100 STR and 10 murders (25% loss), you'd have 75 STR after resurrection

#### Skills

- Each skill is multiplied by the retention percentage
- **Minimum floor**: Skills won't drop below 35.0
- Example: With 100.0 Swordsmanship and 10 murders (25% loss), you'd have 75.0 Swordsmanship

### Important Notes

⚠️ **This penalty is severe!**

- At 5 murders, you lose **20% of all stats and skills**
- At 10 murders, you lose **25% of all stats and skills**
- At 25+ murders, you lose **40% of all stats and skills** (maximum penalty)

💡 **The penalty clears your short-term murders**

- After resurrection, your short-term murder count is reset to 0
- This means you "pay off" your murders with the stat/skill loss
- Your long-term murders (kills) remain unchanged

🎯 **Avoiding the Penalty**

1. **Stay below 5 short-term murders** - No penalty at 4 or fewer
2. **Use a Forged Pardon** - Resets both murder types without penalty
3. **Wait for decay** - Let murders decay below 5 before dying
4. **Don't die** - The penalty only applies on resurrection

### Strategic Considerations

**When to Take the Penalty:**

- If you have 5-9 murders and can't afford a pardon
- If you need to clear murders quickly to avoid the 10+ lockout for pardons
- If you're confident you can regain stats/skills through training

**When to Avoid the Penalty:**

- Use a Forged Pardon if you can afford it (no stat/skill loss)
- Stay alive and let murders decay naturally if possible
- Keep murders below 5 if you engage in risky PvP

---

## The Corrupt Judge & Pardons

### Finding the Judge

Dryden the Judge can be found in the world and offers a **discreet service** for those seeking to clear their names... for a price.

### How to Request a Pardon

1. Approach Dryden the Judge
2. Say: **"I request a pardon"**
3. If eligible, the Judge will provide you with a **Forged Pardon**

### Eligibility Requirements

You can request a pardon if you meet **ALL** of the following criteria:

| Requirement | Details |
|------------|---------|
| **Minimum Murders** | Must have at least **5** short-term murders |
| **Maximum Murders** | Must have **less than 10** short-term murders |
| **Previous Pardons** | Can only receive **3 pardons maximum** from the Judge |
| **Sufficient Gold** | Must have enough gold in your bank |

### Pardon Pricing

The cost increases with each pardon you purchase:

| Pardon Number | Cost |
|---------------|------|
| **1st Pardon** | 50,000 gold |
| **2nd Pardon** | 150,000 gold |
| **3rd Pardon** | 300,000 gold |

**Note**: Gold is automatically withdrawn from your bank account.

### Judge's Responses

The Judge has different responses based on your situation:

- **Too few murders (less than 5)**: The Judge will be outraged that you'd suggest he'd engage in corruption
- **Too many murders (10+)**: "Even with the gold you offer, I cannot forge a Pardon for one so drenched in blood..."
- **Too many pardons (3+)**: "Thou hast stretched my generosity thin. Another Pardon would raise suspicions..."
- **Successful pardon**: "Our business is concluded. Let no soul know of this pardon..."

---

## Using a Forged Pardon

Once you receive a **Forged Pardon**:

1. The pardon is **blessed** (won't be lost on death)
2. It is **bound to you** - only you can use it
3. Keep it in your **backpack**
4. **Double-click** the pardon to use it
5. Upon use:
   - Your **short-term murders** are reset to **0**
   - Your **long-term murders (kills)** are reset to **0**
   - The pardon is consumed
   - You receive a message: *"Redemption is granted. Your sins are now but shadows of the past."*

---

## Important Notes

### ⚠️ Things to Remember:

- **Murder counts only decay while online** - Logging out pauses all decay timers
- **You can only get 3 pardons total** - Choose when to use the Judge's services wisely
- **Pardons get more expensive** - The first is relatively affordable, but the third is very costly
- **10+ murders locks you out** - If you accumulate 10 or more short-term murders, the Judge will not help you
- **Pardons are character-bound** - You cannot trade or give them to other players
- **The Judge keeps records** - He tracks how many pardons you've purchased

### 💡 Strategy Tips:

1. **Not all kills become counts** - Remember, victims must report you, so diplomacy matters
2. **Monitor your murder count** - Don't let it reach 10 if you want the option to buy a pardon
3. **First pardon is cheap** - Consider it an investment if you're at 5-9 murders
4. **Let murders decay naturally if possible** - Save gold by waiting, but this requires long play sessions
5. **Plan your PvP carefully** - Each kill has consequences that last many hours
6. **Thieves Guild members can't report** - They're criminals themselves, so guards won't take their reports

---

## Summary

The murder system is designed to:

- **Track** player killing behavior accurately through reportable murder counts
- **Punish** excessive PKing through severe stat/skill loss on resurrection (5+ murders)
- **Discourage** long-term murderous behavior through time-based decay consequences
- **Provide** a redemption path through the Corrupt Judge for those willing to pay
- **Balance** risk vs. reward for those who choose the darker path

Whether you're a noble hero or a notorious villain, understanding this system will help you navigate the consequences of your actions in the world.

*Remember: With great power comes great responsibility... or at least, great expense and stat loss.*
