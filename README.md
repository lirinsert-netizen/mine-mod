# mine-mod

## Анализ урона заклинаний Iron's Spells (1.21.1 NeoForge)

Источник анализа: `@iron431/irons-spells-n-spellbooks`, путь `src/main/java/io/redspace/ironsspellbooks/spells`, тег `v1.21.1-3.15.5`.

> Сортировка: от большего к меньшему по **базовому урону** (при `spellPower = 0`).

| Заклинание | Формула урона | Базовый урон | Файл |
|---|---|---:|---|
| Sacrifice | `(10 + spellPower) * summonDamageAttr` (+ взрыв от HP) | 10* | `spells/blood/SacrificeSpell.java` |
| Magma Bomb | `baseSpellPower * entityPowerMultiplier` | 8* | `spells/fire/MagmaBombSpell.java` |
| Sculk Tentacles | `baseSpellPower * entityPowerMultiplier` | 8* | `spells/eldritch/SculkTentaclesSpell.java` |
| Burning Dash | `5 + spellPower` | 5 | `spells/fire/BurningDashSpell.java` |
| Fireball | `5 + 5*spellPower` | 5 | `spells/fire/FireballSpell.java` |
| Volt Strike | `5 + spellPower` | 5 | `spells/lightning/VoltStrikeSpell.java` |
| Shockwave | `4 + 0.75*spellPower` | 4 | `spells/lightning/ShockwaveSpell.java` |
| Ray of Frost | `3 + 1.5*spellPower` | 3 | `spells/ice/RayOfFrostSpell.java` |
| Acupuncture | `1 + spellPower` | 1 | `spells/blood/AcupunctureSpell.java` |
| Cone of Cold | `1 + 0.75*spellPower` | 1 | `spells/ice/ConeOfColdSpell.java` |
| Dragon Breath | `1 + 0.75*spellPower` | 1 | `spells/ender/DragonBreathSpell.java` |
| Electrocute | `1 + 0.75*spellPower` | 1 | `spells/lightning/ElectrocuteSpell.java` |
| Fire Breath | `1 + 0.75*spellPower` | 1 | `spells/fire/FireBreathSpell.java` |
| Poison Breath | `1 + 0.75*spellPower` | 1 | `spells/nature/PoisonBreathSpell.java` |
| Divine Smite | `spellPower + weaponDamage(+smite)` | 0* | `spells/holy/DivineSmiteSpell.java` |
| Flaming Strike | `spellPower + weaponDamage(+fire aspect)` | 0* | `spells/fire/FlamingStrikeSpell.java` |
| Raise Hell | `spellPower + weaponDamage` | 0* | `spells/fire/RaiseHellSpell.java` |
| Shadow Slash | `spellPower + weaponDamage` | 0* | `spells/ender/ShadowSlashSpell.java` |
| Throw | `spellPower + weaponDamage` | 0* | `spells/evocation/ThrowSpell.java` |
| Arrow Volley | `0.25*spellPower` | 0 | `spells/evocation/ArrowVolleySpell.java` |
| Ascension | `int(spellPower)` (есть спад по дистанции) | 0 | `spells/lightning/AscensionSpell.java` |
| Ball Lightning | `0.5*spellPower` | 0 | `spells/lightning/BallLightningSpell.java` |
| Black Hole | `2*spellPower` | 0 | `spells/ender/BlackHoleSpell.java` |
| Blood Needles | `0.25*spellPower` | 0 | `spells/blood/BloodNeedlesSpell.java` |
| Blood Slash | `spellPower` | 0 | `spells/blood/BloodSlashSpell.java` |
| Chain Creeper | `spellPower` | 0 | `spells/evocation/ChainCreeperSpell.java` |
| Chain Lightning | `spellPower` | 0 | `spells/lightning/ChainLightningSpell.java` |
| Devour | `spellPower` | 0 | `spells/blood/DevourSpell.java` |
| Earthquake | `0.25*spellPower` | 0 | `spells/nature/EarthquakeSpell.java` |
| Eldritch Blast | `spellPower` | 0 | `spells/eldritch/EldritchBlastSpell.java` |
| Fang Strike | `spellPower` | 0 | `spells/evocation/FangStrikeSpell.java` |
| Fire Arrow | `spellPower` | 0 | `spells/fire/FireArrowSpell.java` |
| Firebolt | `0.5*spellPower` | 0 | `spells/fire/FireboltSpell.java` |
| Firecracker | `spellPower` | 0 | `spells/evocation/FirecrackerSpell.java` |
| Firefly Swarm | `spellPower/3` | 0 | `spells/nature/FireflySwarmSpell.java` |
| Flaming Barrage | `spellPower` | 0 | `spells/fire/FlamingBarrageSpell.java` |
| Guiding Bolt | `0.5*spellPower` | 0 | `spells/holy/GuidingBoltSpell.java` |
| Ice Block | `spellPower` | 0 | `spells/ice/IceBlockSpell.java` |
| Ice Spikes | `spellPower` (часть шипов `0.5x`) | 0 | `spells/ice/IceSpikesSpell.java` |
| Icicle | `0.5*spellPower` | 0 | `spells/ice/IcicleSpell.java` |
| Lightning Lance | `spellPower` | 0 | `spells/lightning/LightningLanceSpell.java` |
| Lob Creeper | `0.5*spellPower` | 0 | `spells/evocation/LobCreeperSpell.java` |
| Magic Arrow | `spellPower` | 0 | `spells/ender/MagicArrowSpell.java` |
| Magic Missile | `0.5*spellPower` | 0 | `spells/ender/MagicMissileSpell.java` |
| Poison Arrow | `arrow: spellPower; aoe: 0.185*spellPower` | 0 | `spells/nature/PoisonArrowSpell.java` |
| Poison Splash | `spellPower` | 0 | `spells/nature/PoisonSplashSpell.java` |
| Ray of Siphoning | `0.25*spellPower` (за тик) | 0 | `spells/blood/RayOfSiphoningSpell.java` |
| Scorch | `spellPower` | 0 | `spells/fire/ScorchSpell.java` |
| Sonic Boom | `spellPower` | 0 | `spells/eldritch/SonicBoomSpell.java` |
| Starfall | `0.5*spellPower` (на метеор) | 0 | `spells/ender/StarfallSpell.java` |
| Stomp | `spellPower` | 0 | `spells/nature/StompSpell.java` |
| Sunbeam | `0.5*spellPower` | 0 | `spells/holy/SunbeamSpell.java` |
| Thunder Step | `spellPower` | 0 | `spells/lightning/ThunderStepSpell.java` |
| Wall of Fire | `spellPower` | 0 | `spells/fire/WallOfFireSpell.java` |
| Wither Skull | `0.5*spellPower` | 0 | `spells/blood/WitherSkullSpell.java` |
| Wisp | `spellPower` | 0 | `spells/holy/WispSpell.java` |

\* зависит от доп. факторов (оружие/атрибуты/контекст), поэтому базовое значение условное.
