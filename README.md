## Macros
- [Ranged Attack](###ranged-attack)
- [Weapon Swap](###weapon-swap)
- [Mouseover Use Helm](###mouseover-use-helm)
- [Toggle Cleave](###toggle-cleave)
- [Toggle Heroic Strike](###toggle-heroic-strike)
- [Mouseover Interrupt](###mouseover-interrupt)
- [Mouseover Intimidating Shout](###mouseover-intimidating-shout)
- [Taunt](###taunt)
- [Mocking Blow](###mocking-blow)
- [Charge](#charge)
- [Intercept](###intercept)
- [Rend](###rend)
- [Hamstring](###hamstring)
- [Disarm](###disarm)
- [Execute](###execute)
- [Overpower + Revenge](###overpower-+-revenge)
- [Shield Block](###shield-block)
- [Recklessness](###recklessness)
- [Shield Wall](###shield-wall)
- [Retaliation](###retaliation)
- [Berserker Rage](###berserker-rage)
- [Whirlwind](###whirlwind)
- [Sweeping Strikes](###sweeping-strikes)

### Ranged Attack

Uses the appropriate spell to attack with your equipped ranged weapon.

```
/cast [equipped:Bow] Shoot Bow; [equipped:Crossbow] Shoot Crossbow; [equipped:Gun] Shoot Gun; [equipped:Thrown] Throw;
/startattack
```

### Weapon Swap

Switches between two sets of weapons.

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

### Mouseover Use Helm

Use your equipped helm on your target or mouseover target. Prioritizes the mouseover target. Nice for Goblin Rocket Helmet.

```
#showtooltip 1
/use [@mouseover, harm, nodead][] 1
```

### Toggle Cleave

Turn Cleave on or off for the next main-hand swing.

```
#show Cleave
/cast Cleave
/startattack
/stopcasting
```

### Toggle Heroic Strike

Turn Heroic Strike on or off for the next main-hand swing.

```
#show Heroic Strike
/cast Heroic Strike
/startattack
/stopcasting
```

### Mouseover Interrupt

Casts Pummel on the target or mouseover target if you are in Berserker Stance. If a shield is not equipped, casts Berserker Stance. Otherwise, casts Shield Bash instead. Prioritizes the mouseover target.

```
#showtooltip
/stopcasting
/use [@mouseover, harm, nodead, stance:3][stance:3] Pummel; [noequipped:Shields] Berserker Stance; [@mouseover, harm, nodead][] Shield Bash
/startattack
```

### Mouseover Intimidating Shout

Use your Intimidating Shout on your target or mouseover target. Prioritizes the mouseover target. This is useful if there is a target close to your main target so you can catch your main target in a fear that will not break on damage. For example, you can mouseover a shaman totem near a shaman so the shaman is caught in a fear for 8 seconds and you can DPS them the whole time.

```
#show Intimidating Shout
/cast [@mouseover, exists, nodead][] Intimidating Shout
```

### Taunt

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Taunt.

```
#show Taunt
/cast [nostance:2] Defensive Stance; Taunt
```

### Mocking Blow

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Mocking Blow.

```
#show Mocking Blow
/cast [nostance:1] Battle Stance; Mocking Blow
```

### Charge

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Charge.

```
#show Charge
/cast [nostance:1] Battle Stance; Charge
```

### Rend

Casts Battle Stance if you are in Berserker Stance. Otherwise, casts Rend.

```
#show Rend
/cast [stance:3] Battle Stance; Rend
```

### Hamstring

Casts Battle Stance if you are in Defensive Stance. Otherwise, casts Hamstring.

```
#show Hamstring
/cast [stance:2] Battle Stance; Hamstring
```

### Disarm

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Disarm.

```
#show Disarm
/cast [nostance:2] Defensive Stance; Disarm
```

### Execute

Casts Battle Stance if you are in Defensive Stance. Otherwise, casts Execute.

```
#show Execute
/cast [stance:2] Battle Stance; Execute
```

### Overpower + Revenge

Casts Overpower if you are in Battle Stance or Revenge if you are in Defensive Stance.

```
/cast [stance:1] Overpower; [stance:2] Revenge
```

### Shield Block

Equips a one-handed weapon and shield. Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Shield Block.

```
#show Shield Block
/equip [noequipped:Shields] <1H NAME>
/equip [noequipped:Shields] <SHIELD NAME>
/cast [nostance:2] Defensive Stance; Shield Block
/startattack
```

### Recklessness

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Recklessness.

```
#show Recklessness
/cast [nostance:3] Berserker Stance; Recklessness
/startattack
```

### Shield Wall

Casts Defensive Stance if you are not in Defensive Stance. Otherwise, casts Shield Wall.

```
#show Shield Wall
/cast [nostance:2] Defensive Stance; Shield Wall
/startattack
```

### Retaliation

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Retaliation.

```
#show Retaliation
/cast [nostance:1] Battle Stance; Retaliation
/startattack
```

### Intercept

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Intercept.

```
#show Intercept
/cast [nostance:3] Berserker Stance; Intercept
```

### Berserker Rage

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Berserker Rage.

```
#show Berserker Rage
/cast [nostance:3] Berserker Stance; Berserker Rage
```

### Whirlwind

Casts Berserker Stance if you are not in Berserker Stance. Otherwise, casts Whirlwind.

```
#show Whirlwind
/cast [nostance:3] Berserker Stance; Whirlwind
/startattack
```

### Sweeping Strikes

Casts Battle Stance if you are not in Battle Stance. Otherwise, casts Sweeping Strikes.

```
#show Sweeping Strikes
/cast [nostance:1] Battle Stance; Sweeping Strikes
/startattack
```
