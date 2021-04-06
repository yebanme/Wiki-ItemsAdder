# 在游戏中转换旧物品/方块

{% hint style="danger" %}
**It's recommended to start a fresh new world and don't use the old one as converters work but are experimental.**
{% endhint %}

{% hint style="danger" %}
These features MAY be laggy, leave them enabled only for some days and then disable them to avoid useless lag.
{% endhint %}

## 如何自动转换世界中的旧物品

当您从ItemsAdder 1.0更新到2.0时，您注意大多数物品都发生了更改，因此，它们与更新前的旧物品不同。
这就是为什么我要编写一个自动用新物品替换旧物品的功能。每当玩家在世界上打开一个库存时，都会运行这个过程 \(箱子、容器.. 但不是他们自己的库存\).

要启用此功能，必须在**ItemsAdder 2.0**`converter.yml`中将此属性设置为true

#### 确保设置为 inventory-open: true

```text
items-auto-update:
  debug: false
  inventory-open: true
```

## 如何自动转换世界中放置的旧方块

你必须打开`converter.yml`并将你旧方块的**model\_id**与IA 2.0的新方块**命名空间**进行映射。例如，我已经添加了旧的ItemsAdder 1.0方块映射，将它们转换为2.0命名空间方块。

#### 确保设置为 enabled: true

```text
blocks:
  enabled: true
  debug: false
  conversion-map:
    "1": "itemsadder:ruby_block"
    "2": "itemsadder:crystal_block"
    "3": "itemsadder:spinel_block"
    "4": "itemsadder:turquoise_block"
    "5": "itemsadder:aqua_aura_block"
    "6": "itemsadder:amethyst_block"
    "7": "itemsadder:amethyst_prism_block"
    "8": "itemsadder:crying_obsidian"
    "9": "itemsadder:nice_stone"
    "10": "itemsadder:nice_wood"
    "11": "itemsadder:modern_stone"
    "12": "itemsadder:modern_sandstone"
    "13": "itemsadder:modern_quartz"
    "14": "itemsadder:ruby_ore"
    "15": "itemsadder:spinel_ore"
    "16": "itemsadder:turquoise_ore"
    "17": "itemsadder:aqua_aura_ore"
    "18": "itemsadder:amethyst_ore"
    "19": "itemsadder:bronze_ore"
    "20": "itemsadder:mysterious_ore"
    "21": "itemsadder:end_ore"
    "22": "itemsadder:restoration_table"
    "23": "itemsadder:customization_table"
    "24": "itemsadder:iron_dirt_ore"
    "25": "itemsadder:gold_dirt_ore"
    "26": "itemsadder:coal_dirt_ore"
    "27": "itemsadder:blaze_powder_ore"
    "28": "itemsadder:nether_alchemy_ore"
```

