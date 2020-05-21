## General
- [Ranged Attack](#ranged-attack)
- [Weapon Swap](#weapon-swap)
- [Mouseover Use Helm](#mouseover-use-helm)

## Skills
- [Toggle Cleave](#toggle-cleave)
- [Toggle Heroic Strike](#toggle-heroic-strike)
- [Mouseover Interrupt](#mouseover-interrupt)
- [Mouseover Intimidating Shout](#mouseover-intimidating-shout)
- [Taunt](#taunt)
- [Mocking Blow](#mocking-blow)
- [Charge](#charge)
- [Intercept](#intercept)
- [Rend](#rend)
- [Hamstring](#hamstring)
- [Disarm](#disarm)
- [Execute](#execute)
- [Overpower + Revenge](#overpower-+-revenge)
- [Shield Block](#shield-block)
- [Recklessness](#recklessness)
- [Shield Wall](#shield-wall)
- [Retaliation](#retaliation)
- [Berserker Rage](#berserker-rage)
- [Whirlwind](#whirlwind)
- [Sweeping Strikes](#sweeping-strikes)

# Ranged Attack

### Description

Uses the appropriate spell to attack with your equipped ranged weapon.

### Macro

```
/cast [equipped:Bow] Shoot Bow; [equipped:Crossbow] Shoot Crossbow; [equipped:Gun] Shoot Gun; [equipped:Thrown] Throw;
/startattack
```

# Weapon Swap

### Description

Switches between two sets of weapons.

### Macro

```
#showtooltip 16
/equipslot 16 <MAIN>
/equipslot 17 <OFF>
/equipslot 16 <2H>
```

```
#showtooltip 16
/equipslot 16 <MAIN #1>
/equipslot 17 <OFF #1>
/equipslot 16 <MAIN #2>
/equipslot 17 <OFF #2>
```

# Mouseover Use Helm

### Description

Use your equipped helm on your target or mouseover target. Prioritizes the mouseover target. Nice for Goblin Rocket Helmet.

### Macro

```
#showtooltip 1
/use [@mouseover, harm, nodead][] 1
```

# Toggle Cleave

### Description

Turn Cleave on or off for the next main-hand swing.

### Macro

```
#show Cleave
/cast Cleave
/startattack
/stopcasting
```

# Toggle Heroic Strike

### Description

Turn Heroic Strike on or off for the next main-hand swing.

### Macro

```
#show Heroic Strike
/cast Heroic Strike
/startattack
/stopcasting
```

# Mouseover Interrupt

### Description

Casts Pummel on the target or mouseover target if you are in Berserker Stance. If a shield is not equipped, casts Berserker Stance. Otherwise, casts Shield Bash instead. Prioritizes the mouseover target.

### Macro

```
#showtooltip
/stopcasting
/use [@mouseover, harm, nodead, stance:3][stance:3] Pummel; [noequipped:Shields] Berserker Stance; [@mouseover, harm, nodead][] Shield Bash
/startattack
```

# Mouseover Intimidating Shout

### Description

Use your Intimidating Shout on your target or mouseover target. Prioritizes the mouseover target.

### Macro

```
#show Intimidating Shout
/cast [@mouseover, exists, nodead][] Intimidating Shout
```

# Taunt

### Description

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Taunt.

### Macro

```
#show Taunt
/cast [nostance:2] Defensive Stance; Taunt
```

# Mocking Blow

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Mocking Blow.

### Macro

```
#show Mocking Blow
/cast [nostance:1] Battle Stance; Mocking Blow
```

# Charge

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Charge.

### Macro

```
#show Charge
/cast [nostance:1] Battle Stance; Charge
```

# Rend

### Description

Casts Battle Stance if you are in Berserker Stance. Otherwise, casts Rend.

### Macro

```
#show Rend
/cast [stance:3] Battle Stance; Rend
```

# Hamstring

### Description

Casts Battle Stance if you are in Defensive Stance. Otherwise, casts Hamstring.

### Macro

```
#show Hamstring
/cast [stance:2] Battle Stance; Hamstring
```

# Disarm

### Description

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Disarm.

### Macro

```
#show Disarm
/cast [nostance:2] Defensive Stance; Disarm
```

# Execute

### Description

Casts Battle Stance if you are in Defensive Stance. Otherwise, casts Execute.

### Macro

```
#show Execute
/cast [stance:2] Battle Stance; Execute
```

# Overpower + Revenge

### Description

Casts Overpower if you are in Battle Stance or Revenge if you are in Defensive Stance.

### Macro

```
/cast [stance:1] Overpower; [stance:2] Revenge
```

# Shield Block

### Description

Equips a one-handed weapon and shield. Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Shield Block.

### Macro

```
#show Shield Block
/equip [noequipped:Shields] <1H NAME>
/equip [noequipped:Shields] <SHIELD NAME>
/cast [nostance:2] Defensive Stance; Shield Block
/startattack
```

# Recklessness

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Recklessness.

### Macro

```
#show Recklessness
/cast [nostance:3] Berserker Stance; Recklessness
/startattack
```

# Shield Wall

### Description

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Shield Wall.

### Macro

```
#show Shield Wall
/cast [nostance:2] Defensive Stance; Shield Wall
/startattack
```

# Retaliation

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Retaliation.

### Macro

```
#show Retaliation
/cast [nostance:1] Battle Stance; Retaliation
/startattack
```

# Intercept

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Intercept.

### Macro

```
#show Intercept
/cast [nostance:3] Berserker Stance; Intercept
```

# Berserker Rage

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Berserker Rage.

### Macro

```
#show Berserker Rage
/cast [nostance:3] Berserker Stance; Berserker Rage
```

# Whirlwind

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Whirlwind.

### Macro

```
#show Whirlwind
/cast [nostance:3] Berserker Stance; Whirlwind
/startattack
```

# Sweeping Strikes

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Sweeping Strikes.

### Macro

```
#show Sweeping Strikes
/cast [nostance:1] Battle Stance; Sweeping Strikes
/startattack
```
