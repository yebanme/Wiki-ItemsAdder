---
description: Collection of basic item properties
---

# Basic

### Enabled

```yaml
enabled: true
```

With this setting you can disable an item completely.  
**Obviously if a player has it in inventory it won't be removed, he still will own it.  
Same thing for blocks, but when broken they won't drop anymore**

### Display name

```yaml
display_name: "Test"
```

This is the name user will see on the item

### Permission

```yaml
permission: myitem
```

{% page-ref page="item-permission.md" %}

### Lore

```yaml
lore:
- '&7When you mine a block'
- '&7it drops exp orbs'
- '&750% of times.'
```

Lore lines of the item

### Attribute modifiers

```yaml
attribute_modifiers:
  mainhand:
    attackDamage: 19
    attackSpeed: 1.1
    maxHealth: 1.1
    movementSpeed: -1
    armor: 1.1
    armorToughness: 1.1
    attackKnockback: 1.1
    luck: 1.1
  offhand:
    attackDamage: 19
    attackSpeed: 1.1
    maxHealth: 1.1
    movementSpeed: 1.1
    armor: 1.1
    armorToughness: 1.1
    attackKnockback: 1.1
    luck: 1.1
```

These are the vanilla attribute modifiers, you can get more info here [https://minecraft.gamepedia.com/Attribute\#Attributes\_available\_on\_all\_living\_entities](https://minecraft.gamepedia.com/Attribute#Attributes_available_on_all_living_entities)

### Durability

```yaml
durability:
  max_custom_durability: 200
  custom_durability: 32
  disappear_when_broken: false
  unbreakable: false
  usages: 5
```

There are pretty self explanatory.  
`usages` are a special propery which allows you to set a number of usages for the current item. Remember to decrement it using events \(check events tutorial\).

`custom_durability` is the durability amount which the item has on crafting \(if not specified is the same as `max_custom_durability`\)

`max_custom_durability` is the max durability the item can reach

### Item flags

```yaml
item_flags:
  - HIDE_ATTRIBUTES
  - HIDE_DESTROYS
  - HIDE_ENCHANTS
  - HIDE_PLACED_ON
  - HIDE_POTION_EFFECTS
  - HIDE_UNBREAKABLE
```

Special item flags that can hide some vanilla info of the item.  
You can find a detailed info list here: [https://hub.spigotmc.org/javadocs/spigot/org/bukkit/inventory/ItemFlag.html](https://hub.spigotmc.org/javadocs/spigot/org/bukkit/inventory/ItemFlag.html)

### blocked\_enchants

Special item property that disables enchants for this item, so your users won't be able to enchant it.

{% tabs %}
{% tab title="Disable some enchants" %}
```yaml
blocked_enchants:
      - DAMAGE_UNDEAD
      - DAMAGE_ALL
      - DAMAGE_ARTHROPODS
      - KNOCKBACK
      - DURABILITY
      - SWEEPING_EDGE
```
{% endtab %}

{% tab title="Disable all enchants" %}
```yaml
blocked_enchants:
      - ALL
```
{% endtab %}
{% endtabs %}

### events\_cooldown

Special attribute to limit spamming of events by players. It's in ticks, so 20 = 1 second.

```yaml
  healing_crystals:
    display_name: display-name-healing_crystals
    permission: healing_crystals
    resource:
      material: IRON_SWORD
      generate: true
      textures:
      - item/healing_crystals.png
    durability:
      max_custom_durability: 6
      custom_durability: 6
      disappear_when_broken: true
    item_flags:
    - HIDE_ATTRIBUTES
    events_cooldown: 1200 ########### <-- EXAMPLE 60 seconds
    events:
      interact:
        right:
          play_particle:
            name: HEART
          decrement_durability:
            amount: 1
          potion_effect:
            type: REGENERATION
            duration: 70
            amplifier: 4
```

### events\_needed\_player\_stats

Special attribute to make events work only if the player stat \(ItemsAdder player stat, which are usually shown in HUDs\) satisfies the set rule.

You can set it to `>`, `<` ad `=`

#### Example:

{% page-ref page="../../../beginners/creating-a-custom-item/magic-wand/" %}

```yaml
  magic_wand:
    display_name: "Magic wand"
    permission: magic_wand
    resource:
      material: DIAMOND_SWORD
      generate: true
      textures:
      - item/example_item.png
    durability:
      max_custom_durability: 512
    attribute_modifiers:
      mainhand:
        attackDamage: 0.1
    blocked_enchants:
    - ALL
    events_needed_player_stats:
      mana: ">0" ### <---- for example. You could also set it to <5 or =1 for example.
    events:
      interact:
        entity:
          target_potion_effect:
            type: GLOWING
            duration: 70
            amplifier: 15
          decrement_player_stat:
            name: mana
            amount: 1
```



