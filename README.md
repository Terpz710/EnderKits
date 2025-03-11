<p align="center">
    <a href="https://github.com/Terpz710/EnderKits"><img src="https://github.com/Terpz710/EnderKits/blob/main/icon.PNG"></img></a><br>

# Description

A simple kits plugin for Pocketmine-MP. This plugin will allow you to create unlimited kits with easy to use permission and cool down sytsem. Very easy configurable kits.yml.

- Custom permission support

- Added bank notes to the kit(MUST USE MY BANK NOTES PLUGIN CALLED "BankNotesPlus")

- Configurable messages

- BankNotesPlus: [BankNotesPlus](https://poggit.pmmp.io/p/BankNotesPlus/1.0.5)
  
# Permissions

```
permissions:
  enderkits.kit:
    description: "Enderkits Perm"
    default: tru
```

# CONFIG

**kits.yml**

```php
# Made by Terpz710 :p

# To create a kit follow the preset kit down below!
# Name, enchantment and banknotes are optional!

# You may use '&' for color coding in the 'name' key

kits:
  test:
    kit_name: "Test"
    permissions: "enderkits.kit.test"
    armor:
      helmet:
        item: "diamond_helmet"
        name: "Test Helmet"
        enchantments:
          protection: 2
      chestplate:
        item: "diamond_chestplate"
        name: "Test Chestplate"
        enchantments:
          protection: 2
      leggings:
        item: "diamond_leggings"
        name: "Test Leggings"
        enchantments:
          protection: 2
      boots:
        item: "diamond_boots"
        name: "Test Boots"
        enchantments:
          protection: 2
    items:
      - item: "diamond_sword"
        name: "&4Test Sword"
        enchantments:
          sharpness: 2
        quantity: 1
      - item: "diamond_pickaxe"
        name: "Test Pickaxe"
        enchantments:
          efficiency: 5
        quantity: 1
      - item: "golden_apple"
        quantity: 5
      - item: "steak"
        quantity: 32
    cooldown: 60
    banknotes:
      - 1000
      - 5000
      - 20000

  starter:
    kit_name: "Starter"
    permissions: "enderkits.kit.starter"
    armor:
      helmet:
        item: "iron_helmet"
        enchantments:
          protection: 1
      chestplate:
        item: "iron_chestplate"
        enchantments:
          protection: 1
      leggings:
        item: "iron_leggings"
        enchantments:
          protection: 1
      boots:
        item: "iron_boots"
        enchantments:
          protection: 1
    items:
      - item: "stone_sword"
        enchantments:
          sharpness: 1
        quantity: 1
      - item: "stone_pickaxe"
        quantity: 1
      - item: "bread"
        quantity: 32
      - item: "apple"
        quantity: 10
    cooldown: 10

  vip:
    kit_name: "VIP"
    permissions: "enderkits.kit.vip"
    armor:
      helmet:
        item: "chainmail_helmet"
        enchantments:
          protection: 3
      chestplate:
        item: "chainmail_chestplate"
        enchantments:
          protection: 3
      leggings:
        item: "chainmail_leggings"
        enchantments:
          protection: 3
      boots:
        item: "chainmail_boots"
        enchantments:
          protection: 3
    items:
      - item: "iron_sword"
        enchantments:
          sharpness: 3
        quantity: 1
      - item: "carrot"
        quantity: 8
      - item: "cooked_chicken"
        quantity: 16
      - item: "potion"
        name: "Swiftness Potion"
        quantity: 2
    cooldown: 10
```

# TODO

- [x] Make a messages.yml to handle messages
- [ ] Add an ecomony system
- [x] Add UI support(Will make it an off/on)
