# Charge

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Charge.

```
if stance is not battle stance:
    cast battle stance
else:
    cast charge
```

### Macro

```
#show Charge
/cast [nostance:1] Battle Stance; Charge
```

# Taunt

### Description

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Taunt.

```
if stance is not defensive stance:
    cast defensive stance
else:
    cast taunt
```

### Macro

```
#show Taunt
/cast [nostance:2] Defensive Stance; Taunt
```

# Rend

### Description

Casts Battle Stance if you are in Berserker Stance. Otherwise, casts Rend.

```
if stance is berserker:
    cast battle stance
else:
    cast rend
```

### Macro

```
#show Rend
/cast [stance:3] Battle Stance; Rend
```

# Mocking Blow

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Mocking Blow.

```
if stance is not battle:
    cast battle stance
else:
    cast mocking blow
```

### Macro

```
#show Mocking Blow
/cast [nostance:1] Battle Stance; Mocking Blow
```

# Hamstring

### Description

Casts Battle Stance if you are in Defensive Stance. Otherwise, casts Hamstring.

```
if stance is defensive:
    cast battle stance
else:
    cast hamstring
```

### Macro

```
#show Hamstring
/cast [stance:2] Battle Stance; Hamstring
```

# Disarm

### Description

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Disarm.

```
if stance is not defensive:
    cast defensive stance
else:
    cast disarm
```

### Macro

```
#show Disarm
/cast [nostance:2] Defensive Stance; Disarm
```

# Execute

### Description

Casts Battle Stance if you are in Defensive Stance. Otherwise, casts Execute.

```
if stance is defensive:
    cast battle stance
else:
    cast execute
```

### Macro

```
#show Execute
/cast [stance:2] Battle Stance; Execute
```

# Overpower + Revenge

### Description

Casts Overpower if you are in Battle Stance or Revenge if you are in Defensive Stance.

```
if stance is battle:
    cast overpower

if stance is defensive:
    cast revenge
```

### Macro

```
/cast [stance:1] Overpower; [stance:2] Revenge
```

# Shield Block

### Description

Equips a one-handed weapon and shield. Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Shield Block.

```
if shield is not equipped:
    equip 1h

if shield is not equipped:
    equip shield

if stance is not defensive:
    cast defensive stance

cast shield block
```

### Macro

```
#show Shield Block
/equip [noequipped:Shields] <1H NAME>
/equip [noequipped:Shields] <SHIELD NAME>
/cast [nostance:2] Defensive Stance; Shield Block
/startattack
```

# Interrupt

### Description

Casts Pummel. If a shield is equipped and you are not in Berserker Stance, casts Shield Bash instead.

```
if shield is equipped and stance is not berserker:
    cast shield bash
else:
    cast pummel
```

### Macro

```
#showtooltip
/cast [equipped:Shield, nostance:3] Shield Bash; Pummel
```


# Recklessness

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Recklessness.

```
if stance is not berserker:
    cast berserker stance

cast recklessness
```

### Macro

```
#show Recklessness
/cast [nostance:3] Berserker Stance; Recklessness
/startattack
```

# Shield Wall

### Description

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Shield Wall.

```
if stance is not defensive:
    cast defensive stance

cast shield wall
```

### Macro

```
#show Shield Wall
/cast [nostance:2] Defensive Stance; Shield Wall
/startattack
```

# Retaliation

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Retaliation.

```
if stance is not battle:
    cast battle stance
else:
    cast retaliation
```

### Macro

```
#show Retaliation
/cast [nostance:1] Battle Stance; Retaliation
/startattack
```

# Intercept

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Intercept.

```
if stance is not berserker:
    cast berserker stance

cast intercept
```

### Macro

```
#show Intercept
/cast [nostance:3] Berserker Stance; Intercept
```

# Berserker Rage

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Berserker Rage.

```
if stance is not berserker:
    cast berserker stance

cast berserker rage
```

### Macro

```
#show Berserker Rage
/cast [nostance:3] Berserker Stance; Berserker Rage
```

# Whirlwind

### Description

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Whirlwind.

```
if stance is not berserker:
    cast berserker stance

cast whirlwind
```

### Macro

```
#show Whirlwind
/cast [nostance:3] Berserker Stance; Whirlwind
/startattack
```

# Sweeping Strikes

### Description

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Sweeping Strikes.

```
if stance is not battle:
    cast battle stance

cast sweeping strikes
```

### Macro

```
#show Sweeping Strikes
/cast [nostance:1] Battle Stance; Sweeping Strikes
/startattack
```

# Ranged Attack

### Description

Uses the appropriate spell to attack with your equipped ranged weapon.

### Macro

```
/cast [equipped:Bow] Shoot Bow; [equipped:Crossbow] Shoot Crossbow; [equipped:Gun] Shoot Gun; [equipped:Thrown] Throw;
/startattack
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

# Mouse-Over Use Helm

### Description

Use your equipped helm on your target or mouse-over target. Prioritizes the mouse-over target.

### Macro

```
#showtooltip 1
/tar [@target, harm, nodead] [@mouseover, harm, nodead]
/stopmacro [@target, dead] [@target, noexists]
/use [@mouseover, harm, nodead] [ ] 1
```

# Mouse-Over Intimidating Shout

### Description

Use your Intimidating Shout on your target or mouse-over target. Prioritizes the mouse-over target.

### Macro

```
#show Intimidating Shout
/cast [@mouseover, exists, nodead][] Intimidating Shout
```

# Toggle Weapons

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
