# mine-mod

## Все заклинания Iron's Spells 'n Spellbooks (1.21.1 NeoForge)

> Источник: [`@iron431/irons-spells-n-spellbooks`](https://github.com/iron431/irons-spells-n-spellbooks), тег `v1.21.1-3.15.5`  
> Базовый урон указан при **уровне 1, без бонусов к spell power**.  
> `*` — дополнительные факторы (атрибуты существа, оружие, призывные существа).

---

### Заклинания с уроном (от большего к меньшему)

| # | Заклинание | Школа | Формула урона | Урон (Lv1) | Откат |
|---|---|---|---|---:|---|
| 1 | **Sacrifice** | Кровь | `(10 + spellPower) × attrMult` + взрыв при жертве | ~20* | 120 с |
| 2 | **Fireball** | Огонь | `5 + 5 × spellPower` | 10 | 25 с |
| 3 | **Lightning Bolt** | Молния | `spellPower` (radial falloff) | 10 | 25 с |
| 4 | **Fang Ward** | Вызов | `spellPower` (кольца клыков вокруг) | 8 | 15 с |
| 5 | **Magma Bomb** | Огонь | `spellPower × powerMult` | 8* | 30 с |
| 6 | **Sculk Tentacles** | Эльдрич | `spellPower × powerMult` | 8* | — |
| 7 | **Burning Dash** | Огонь | `5 + spellPower` | 6 | — |
| 8 | **Volt Strike** | Молния | `5 + spellPower` | 6 | — |
| 9 | **Shockwave** | Молния | `4 + 0.75 × spellPower` | ~4.75 | — |
| 10 | **Ray of Frost** | Лёд | `3 + 1.5 × spellPower` | 4.5 | — |
| 11 | **Frost Step** | Лёд | `spellPower` (урон при рассеивании льда) | 4 | 12 с |
| 12 | **Acupuncture** | Кровь | `1 + spellPower` | 2 | — |
| 13 | **Blaze Storm** | Огонь | `0.4 × spellPower` за снаряд | 2/выстрел | 20 с |
| 14 | **Cone of Cold** | Лёд | `1 + 0.75 × spellPower` | ~1.75 | — |
| 15 | **Dragon Breath** | Эндер | `1 + 0.75 × spellPower` | ~1.75 | — |
| 16 | **Electrocute** | Молния | `1 + 0.75 × spellPower` | ~1.75 | — |
| 17 | **Fire Breath** | Огонь | `1 + 0.75 × spellPower` | ~1.75 | — |
| 18 | **Poison Breath** | Природа | `1 + 0.75 × spellPower` | ~1.75 | — |
| 19 | **Divine Smite** | Святость | `spellPower + урон_оружия` (+Smite) | 0+оружие* | — |
| 20 | **Flaming Strike** | Огонь | `spellPower + урон_оружия` (+Fire Aspect) | 0+оружие* | — |
| 21 | **Raise Hell** | Огонь | `spellPower + урон_оружия` | 0+оружие* | — |
| 22 | **Shadow Slash** | Эндер | `spellPower + урон_оружия` | 0+оружие* | — |
| 23 | **Throw** | Вызов | `spellPower + урон_оружия` (бросок врага) | 0+оружие* | — |
| 24 | **Black Hole** | Эндер | `2 × spellPower` | ~scales | — |
| 25 | **Blood Slash** | Кровь | `spellPower` | ~scales | — |
| 26 | **Chain Creeper** | Вызов | `spellPower` (цепная волна криперов) | ~scales | — |
| 27 | **Chain Lightning** | Молния | `spellPower` (прыжки молнии) | ~scales | — |
| 28 | **Devour** | Кровь | `spellPower` (пожирает ХП противника) | ~scales | — |
| 29 | **Eldritch Blast** | Эльдрич | `spellPower` | ~scales | — |
| 30 | **Fang Strike** | Вызов | `spellPower` | ~scales | — |
| 31 | **Fire Arrow** | Огонь | `spellPower` | ~scales | — |
| 32 | **Firecracker** | Вызов | `spellPower` | ~scales | — |
| 33 | **Flaming Barrage** | Огонь | `spellPower` | ~scales | — |
| 34 | **Ice Block** | Лёд | `spellPower` | ~scales | — |
| 35 | **Ice Spikes** | Лёд | `spellPower` (конечные шипы), `0.5×` промежут. | ~scales | — |
| 36 | **Lightning Lance** | Молния | `spellPower` | ~scales | — |
| 37 | **Magic Arrow** | Эндер | `spellPower` | ~scales | — |
| 38 | **Poison Arrow** | Природа | `spellPower` (стрела) + `0.185×spellPower` AoE | ~scales | — |
| 39 | **Poison Splash** | Природа | `spellPower` | ~scales | — |
| 40 | **Scorch** | Огонь | `spellPower` | ~scales | — |
| 41 | **Sonic Boom** | Эльдрич | `spellPower` | ~scales | — |
| 42 | **Stomp** | Природа | `spellPower` | ~scales | — |
| 43 | **Thunder Step** | Молния | `spellPower` | ~scales | — |
| 44 | **Wall of Fire** | Огонь | `spellPower` | ~scales | — |
| 45 | **Ascension** | Молния | `int(spellPower)` (спад по дистанции) | ~scales | — |
| 46 | **Ball Lightning** | Молния | `0.5 × spellPower` | ~scales | — |
| 47 | **Blood Needles** | Кровь | `0.25 × spellPower` (x3 иглы) | ~scales | — |
| 48 | **Earthquake** | Природа | `0.25 × spellPower` | ~scales | — |
| 49 | **Firebolt** | Огонь | `0.5 × spellPower` | ~scales | — |
| 50 | **Firefly Swarm** | Природа | `spellPower / 3` за светлячка | ~scales | — |
| 51 | **Guiding Bolt** | Святость | `0.5 × spellPower` (+ бонус след. удару) | ~scales | — |
| 52 | **Icicle** | Лёд | `0.5 × spellPower` | ~scales | — |
| 53 | **Lob Creeper** | Вызов | `0.5 × spellPower` | ~scales | — |
| 54 | **Magic Missile** | Эндер | `0.5 × spellPower` | ~scales | — |
| 55 | **Ray of Siphoning** | Кровь | `0.25 × spellPower` за тик | ~scales | — |
| 56 | **Starfall** | Эндер | `0.5 × spellPower` за метеор | ~scales | — |
| 57 | **Sunbeam** | Святость | `0.5 × spellPower` | ~scales | — |
| 58 | **Wisp** | Святость | `spellPower` (светлячок-союзник) | ~scales | — |
| 59 | **Wither Skull** | Кровь | `0.5 × spellPower` | ~scales | — |

> «~scales» означает, что базовый урон напрямую равен `baseSpellPower`, конкретное значение зависит от конфигурации предмета.

---

### Заклинания без прямого урона (утилитарные, лечебные, призывные)

| Заклинание | Школа | Описание | Длительность эффекта | Откат |
|---|---|---|---|---|
| **Abyssal Shroud** | Эльдрич | Накладывает эффект Abyssal Shroud на себя (снижает видимость для врагов) | 6 с (base) | 200 с |
| **Angel Wings** | Святость | Даёт эффект Angel Wings — полёт/планирование | 10 с (base) | 120 с |
| **Blight** | Природа | Накладывает дебафф на цель: снижает лечение и урон | 30 с (base) | 90 с |
| **Blessing of Life** | Святость | Лечит союзника дальнего боя на `spellPower` ХП | Мгновенно | 10 с |
| **Blood Step** | Кровь | Телепорт (кровавый рывок с кратковременной невидимостью) | Мгновенно | 12 с |
| **Charge** | Молния | Баф: скорость + урон ближнего боя + spell power | 30 с (base) | 40 с |
| **Cleanse** | Святость | Снимает все вредные эффекты с союзников в радиусе 3 блоков | Мгновенно | 60 с |
| **Cloud of Regeneration** *(устарело)* | Святость | Поток лечения (`0.5×spellPower`) в радиусе 5 блоков | Непрерывно | 35 с |
| **Counterspell** | Эндер | Прерывает заклинание врага, снимает магические эффекты | Мгновенно | 10 с |
| **Echoing Strikes** | Эндер | Баф Echoing Strikes: удары в ближнем бою бьют AoE в радиусе 2 блоков | 20 с (base) | 60 с |
| **Evasion** | Эндер | Уклонение от `spellPower+1` ударов в течение 60 с | 60 с (фикс.) | 180 с |
| **Fortify** | Святость | Absorption-баф для союзников в радиусе 8 блоков | 120 с (фикс.) | 180 с |
| **Frostbite** | Лёд | Баф на себя: следующие удары оружием замораживают цель (shatter damage по окончании) | 30 с (base) | 60 с |
| **Frostwave** | Лёд | Волна холода — замедляет всех врагов в радиусе вокруг вас | 10 с (base) | 45 с |
| **Gluttony** | Природа | Баф: восстановление маны при употреблении пищи | 30 с (base) | 90 с |
| **Greater Heal** | Святость | Полностью восстанавливает своё ХП | Мгновенно | 45 с |
| **Heal** | Святость | Лечит себя на `spellPower` ХП | Мгновенно | 30 с |
| **Healing Circle** | Святость | Зона АОЕ-лечения (`0.25×spellPower`/тик) радиусом 5 блоков | 10 с (фикс.) | 25 с |
| **Heartstop** | Кровь | Накладывает эффект Heartstop на себя (временная «смерть» для вражеских атак) | 10 с (base) | 120 с |
| **Ice Tomb** | Лёд | Заключает себя в ледяном коконе, регенерируя ХП | 4–12 с (по уровню) | 30 с |
| **Invisibility** | Вызов | Полная невидимость (True Invisibility) | 10 с (base) | 45 с |
| **Oakskin** | Природа | Уменьшает получаемый урон, но замедляет движение | 20 с (base) | 90 с |
| **Planar Sight** | Эльдрич | Видит сквозь блоки (Planar Sight) | 40 с (base) | 200 с |
| **Pocket Dimension** | Эльдрич | Переносит в личное карманное измерение | — | 60 с |
| **Portal** | Эндер | Создаёт два портала для быстрого перемещения | 5 мин (base) | 180 с |
| **Raise Dead** | Кровь | Призывает зомби/скелетов; кол-во = `spellLevel + 2` | ~10 мин (призыв) | 150 с |
| **Recall** | Эндер | Телепортирует к кровати/спавну (не в бою); время каста 4 с | Мгновенно | 300 с |
| **Root** | Природа | Обездвиживает цель на месте | 5 с (base) | 35 с |
| **Shield** | Вызов | Создаёт магический щит: HP = `10 + spellPower` | До уничтожения | 8 с |
| **Slow** | Вызов | Замедляет до 5 целей в радиусе 3 блоков | 20 с (base) | 80 с |
| **Spider Aspect** | Природа | Баф: дополнительный урон по отравленным целям | 20 с (base) | 90 с |
| **Summon Ender Chest** | Эндер | Открывает инвентарь эндер-сундука | Мгновенно | 5 с |
| **Summon Horse** | Вызов | Призывает боевого коня с масштабируемыми характеристиками | ~10 мин (призыв) | 20 с |
| **Summon Polar Bear** | Лёд | Призывает белого медведя; HP = `(20+lvl×4)×mult`, урон = `spellPower` | ~10 мин (призыв) | 180 с |
| **Summon Swords** | Эндер | Призывает 3 клинка-союзника (+5%/ур. к урону и +10%/ур. к ХП) | ~10 мин (призыв) | 150 с |
| **Summon Vex** | Вызов | Призывает вексов; кол-во = `spellLevel + 2` | ~10 мин (призыв) | 150 с |
| **Telekinesis** | Эльдрич | Удерживает и перемещает цель в воздухе (continuous) | Непрерывно | 35 с |
| **Teleport** | Эндер | Мгновенный телепорт вперёд по линии взгляда | Мгновенно | 3 с |
| **Thunderstorm** | Молния | Аура: молнии бьют всех врагов в радиусе 20 блоков | 20 с (base) | 120 с |
| **Touch Dig** | Природа | Ломает блок на расстоянии 8 блоков (harvest level от уровня) | Мгновенно | 0.5 с |
| **Wololo** | Вызов | Меняет цвет шерсти овцы на случайный | Мгновенно | 10 с |

---

> **Примечание.** Длительности указаны как `baseSpellPower × 20 ticks ÷ 20 = секунды` при уровне 1. Реальное значение растёт с уровнем и бонусами.
