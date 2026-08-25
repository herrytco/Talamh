---
aliases:
  - Rules
---
Pen&Paper System heavily inspired by *Mongoose Traveler 2nd Edition*.

## 0. General Conventions
Should any calculation yield a non-integer, the result is rounded down.

## 1. Stats and Skills
Several stats and skills describe a character's capabilities. **Stats** are abstract ratings of a character's properties. **Skills** are well-defined capabilities that are combined with stats for individual checks.

### 1.1 Stats
Stats are a broad measure of a character's mental and physical abilities.

| Stat | Description |
| --- | --- |
| Strength (**STR**) | Physical strength, fitness, and forcefulness |
| Dexterity (**DEX**) | Physical coordination, agility, and reflexes |
| Endurance (**END**) | Stamina, determination, and pain resistance |
| Intellect (**INT**) | Intelligence, quickness of mind |

#### 1.1.1 Rolling on Stats
The Dice Modifier of a stat is calculated like this: **(Stat-6)/2**.

### 1.2 Skills
There is no exhaustive list of all available skills a character can obtain. Skills are a character's proficiency in that specific field. For example, a character with the skill "**Pilot**" can control an aircraft more effectively than a regular person, while "Gun Combat" describes the use and maintenance of various firearms.

### 1.3 Specialties
Certain Skills have specialties, meaning multiple skills belong to the same group. Specialties are labeled in round brackets after the primary Skill name. **Gun Combat (Explosives)** implies that a character can handle explosive weapons. However, this also means that the character can handle other weapons. If skill points in a skill with a specialty are present, all other specialties are automatically **promoted to a value of 0 instead of -3**.

## 2. Dice/Number Conventions
This system uses D6 as its default dice. Any unspecified roll refers to 3D6. The following conventions are used in game-related documents:

| Notation | Meaning |
| --- | --- |
| XD | roll X 6-sided dice and add the results together |
| DY | roll one Y-sided dice |
| XDY | roll X Y-sided dice and add the result together |
| ...+X | add X to the roll result |

## 3. Check Procedure
A check is required when a character attempts some action with an uncertain outcome and where failure would have a meaningful consequence. Each check is comprised of the following components:
- A dice roll (3D6)
- A Stats Dice Modifier (optional)
- A skill value (optional)
- A dice modifier (optional)

Examples:
- **Forcefully open a door** 3D6+STR+Athletics
- **Calm a frightened horse** 3D6+INT+Animals

The chosen combination represents how a player attempts the task. A player may propose a different approach, but the Game Master determines whether it is appropriate.

### 3.1 Untrained Checks
If a character does not possess the required Skill, a Skill Level of **-3** is used.

If a character possesses a related specialty from the same Skill group, they are considered trained and use a Skill Level of **0**.

Some tasks (forging a sword, creating a new spell, ...) are impossible without the appropriate skill. Here, each roll automatically fails, no matter how high the result.

### 3.2 Resolve the Check
After the result of the check is determined, the outcome of the check is announced by the Game Master. Checks **succeed if their roll is higher than or equal to the assigned difficulty**.

#### 3.2.1 Unopposed Checks
Unopposed Checks are situations where a character tries to overcome a passive obstacle. In these cases, the check has a hidden difficulty assigned by the Game Master.

| Difficulty | Target | Example |
| --- | --- | --- |
| Routine | Automatic Success | Saddle a calm horse |
| Easy | 8 | Follow fresh tracks |
| Standard | 11 | Climb a rough stone wall |
| Difficult | 14 | Treat a deep wound with poor supplies |
| Formidable | 17 | Track someone through a storm |
| Legendary | 20 | Forge a blade from the heart of a dying star |

#### 3.2.2 Opposed Checks
Opposed Checks are situations where 2 characters actively work against each other. Here, the difficulty of the roll is determined by the outcome of the resisting character.

Examples:
- Sneak past a guard (DEX + Stealth vs INT + Perception)
- Wrestling an opponent (STR + Combat (Unarmed) vs STR or DEX + Combat (Unarmed))

#### 3.2.3 Advantage and Disadvantage
Certain situations make the check easier/harder than it would be otherwise. In those instances, (dis)advantage can be added as a modifier to a check. This means that the roll is performed twice, and the higher/lower result is used for the final outcome.

Example situations:
- Ambushes (see below)
- Fighting while blinded

#### 3.2.4 Assistance
Certain actions can be done with multiple characters. In these cases, an Assisted Check is performed. Here, one character takes the lead and performs a dice check. Each helping character performs a standard dice check. Succeeding gives the leader an additional 1D6; failing will remove the lowest result from the roll.

#### 3.2.5 Combat Rolls
An attack is determined via two rolls: a hit roll and a damage roll. The hit roll is an opposed roll with a weapon archetype's hit roll against the roll of the defensive action. If the hit roll succeeds, a damage roll is performed and the attack resolves. This is either the damage roll of the weapon archetype or a specific one noted in the item description of the used weapon.

A character with no defensive action (either if they do not want to perform an action or are unable to perform one) is hit by a hit roll of 8 or more. Cover is added to that constant defense roll.

## 4. Combat
The attacker makes an attack check. The defender chooses Dodge, Parry, Block, or Passive Defense. The attack hits if its result exceeds the defense result. Cover and other defensive circumstances increase defense, range, and offensive circumstances modify attack. Ties favor the defender.

### 4.1 Weapon Archetypes
Melee weapons can be categorized into different archetypes. These types determine:
- Hit-Rolls
- Damage-Rolls
- Special actions (if any)

| Archetype | Hit-Roll | Damage-Roll |
| --- | --- | --- |
| Hammer | STR+Combat(Melee) | 3d5+STRMOD |
| Axe | STR+Combat(Melee) | 2+1d6+1d5+STRMOD |
| Sword | STR+Combat(Melee) OR DEX+Combat(Melee) | 4+1d4+1d3+STRMOD OR 4+1d4+1d3+DEXMOD |
| Spear | DEX+Combat(Melee) | 5+1d3+1d2+DEXMOD |
| Bow | DEX+Combat(Ranged) | 3+1d6+1d4+DEXMOD |

### 4.2 Initiative
At the start of combat, characters can roll on either **DEX** or **INT**. The higher the result of the roll, the earlier this character can act in combat. They can delay their turn as far back as they want. Initiative marks only the **first** opportunity to act.

#### 4.2.1 Ambushes
Surprising an enemy gives advantage on the attacker's initiative rolls and disadvantage on the defender's initiative rolls.

#### 4.2.2 Tactics
If no ambush situation is present, the party may choose one player to act as the leader. This player can make a **Tactics** roll, the effect of which is added to the initiative of all characters on their side.

Players with Tactics can make a call to their teammates, raising their DM by their Tactics value. The call must be rather specific, and the other player must follow the instruction for this effect to take place. There can only be one Tactics bonus applied at all times.

### 4.3 Range
Each ranged weapon has a Range-score associated with it. This denotes the effective range of this weapon in meters. Based on the actual distance to the target, the following conditions apply:

| Distance | | With Sights | Without Sights |
| --- | --- | --- | --- |
| <25% Range | Short Range | DM+2 | DM+2 |
| 25% - 100% Range | Range | DM | DM |
| 100% - 200% | Long Range | DM-2 | DM-2 |
| 200%-400% | Extreme Range | DM-4 | DM-4 |

If a weapon does not have the **Scope** trait, all distances above 100m automatically count as Extreme Range with a DM-4.

### 4.4 Taking Damage
When an attack hits, resolve it in the following order:
1. Roll for damage according to the attack's instructions
2. Apply any damage modifier (wounds, debuffs, ...)
3. Subtract armor protection (if any)
4. Apply the remaining damage to stats
5. Determine whether the character's condition changes

Physical damage is applied in this order:

> END - chosen Body Stat - remaining Body Stat

The body stats are DEX and STR.

#### 4.4.1 Conditions
| Alive and Well | Injured | Incapacitated | Dead |
| --- | --- | --- | --- |
| All body stats are >0 | END=0 | STR or DEX=0 | All body stats=0 |

Damage is first subtracted from **END**. This represents temporary damage. The character is still fit without penalties as long as their END is above 0. If END reaches 0, the character becomes **Injured**, and excess damage carries over to either STR or DEX. The character chooses one, which becomes their **Wounded Stat**.

Further damage is assigned to the wounded stat. While still conscious, the character is facing the first damage penalties:
1. DM-1 on all physical checks
2. Reduced movement to 4 squares

When the wounded stat reaches 0, excess damage is carried over to their remaining body stat, and the character becomes **Incapacitated**.

While incapacitated, the character remains conscious but can move no more than 1 square per turn. They may still use Free Actions. If the remaining body stat reaches 0, the character dies.

**Fall damage** ignores armor.

### 4.5 Evading Damage

#### 4.5.1 Passive Protection
Passive protection applies automatically without the defender needing to declare anything. They also stack; a character can be in cover and wearing armor and will get the benefits of both.

##### 4.5.1.1 Cover
If a character has applicable cover between them and the attacker, the cover modifier is added to their defense roll.

| Cover | Defence Modifier | Example |
| --- | --- | --- |
| Partial Cover | 1 | Box where upper body is visible |
| Substantial Cover | 2 | Rock where only head is visible |
| Near-total Cover | 4 | Arrow slit in wall |
| Total Cover | Cannot normally be targeted | Staying behind a wall |

##### 4.5.1.2 Armor
Armor reduces the damage dealt by its Protection value. If incoming damage is higher than 6, at least one point of damage is dealt. If incoming damage is higher than 6, the armor value is reduced by 1, which can be repaired.

#### 4.5.2 Active Protection
Characters are allowed to react to the first incoming attack with an active defensive action.

##### 4.5.2.1 Dodge [DEX + Athletics(DEX)]
Move to an adjacent square on a successful dodge. This can only be done if an adjacent, empty square is available.

##### 4.5.2.2 Dive for Cover [DEX + Athletics(DEX)]
You have advantage on the defense roll. Move up to 2 squares. If the character ends up in a suitable cover, the cover modifier is added to the result. If a character dives for cover, they only have one minor action in their next turn.

##### 4.5.2.3 Parry [DEX + Combat(Melee)] DM-4
If a character is attacked by a Melee weapon, they can use their own melee weapon to parry the attack. If the defense roll succeeds, the defender gains advantage on their next attack.

##### 4.5.2.4 Block [STR + Combat]
Block a melee or ranged attack with an equipped shield or weapon. Blocking stops the attack and provides no additional movement or offensive bonus.

### 4.6 Action Economy
Each character can perform 1 major and 1 minor action **OR** 3 minor actions in each round.

#### 4.6.1 Major Actions
Every action described on an item or a skill is a major action if not stated otherwise.

##### 4.6.1.1 Use of an Item/Skill Action

##### 4.6.1.2 Overwatch
Aim your ranged weapon towards a general area and fire at the first enemy that enters your field of view. The hit rolls for this attack suffer a DM-3.

#### 4.6.2 Minor Actions

##### 4.6.2.1 Aiming
Spend one Minor action aiming at a target (not a square) within the range of the used weapon. Gain DM+1 per spent consecutive time Aiming was used (stacks up to 6 times). If the line of sight to the target is interrupted, this bonus resets to 0.

##### 4.6.2.2 Drawing/Reloading
Reloads the current weapon.

##### 4.6.2.3 Movement
Move up to 6 squares. This distance may vary with the terrain.

#### 4.6.3 Free Actions
Free Actions can be used as often as desired (within reason).
- Push a button
- Shout a warning
- ...

### 4.7 Item/Skill Modifiers

#### 4.7.1 Auto X (Full Auto)
Some weapons can be fired in Auto mode, which means the user keeps the trigger pressed down as long as possible while aiming at the target. A hit roll with DM-X must be performed for each shot.

#### 4.7.2 Silent
The weapon is completely silent while being shot. Other means of detection (muzzle flash, ...) can still be sensed.

#### 4.7.3 Multihit X
This action can be executed up to X times in a single action.

### 4.8 Keywords

#### 4.8.1 Grappling
To grapple an enemy, a Character must win an opposed (STR or DEX) Melee (unarmed) check with their target.

The winner may do one of the following:
- Force an opponent prone on the ground.
- Disarm an opponent. If the Effect is 6+, they may take their opponent's weapon.
- Throw an opponent 1D6 meters, causing 1D6 damage. This automatically ends the grapple.
- Inflict damage using a pistol or a small blade-sized weapon.
- Escape and move away (as a normal movement action) to end the grapple.
- Drag their opponent up to three meters.
- Continue the grapple with no other effect.

#### 4.8.2 Dual Weapons
Two weapons of appropriate size can be wielded simultaneously. The user suffers DM-2 on both attack rolls. Using both weapons at once still counts as one Major Action.

#### 4.8.3 Flying
Melee attacks against flying opponents have disadvantage on their hit rolls.

#### 4.8.4 Stunned X
Reduce your action budget to 1 Minor Action for the next X rounds.

#### 4.8.5 Outpaced
Have no actions or reactions for the rest of the round until it is your turn again.

#### 4.8.6 Upkeep X Y
At the start of your turn, pay X amount of resource Y. If this is not possible, the ability ends with possible consequences stated in the ability.

#### 4.8.7 Physical
Can only be activated when touched.

#### 4.8.8 Off
Can be performed in parallel to another action. It doubles the cost for each other's active Off action.

#### 4.8.9 Focus
The action requires the user's focus. Only one "Focus" action can be performed at the same time. The action can be interrupted when the user takes damage or is distracted.

#### 4.8.10 When X
Can be used whenever X happens. Does not consume an action if not stated differently.

#### 4.8.11 Reaction
Can be used outside of your turn, past your Initiative.
