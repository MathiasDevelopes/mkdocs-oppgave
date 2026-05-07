# Enemies & Bosses

## Enemy types

Every floor introduces new enemy variants. Learning their movement patterns is the difference between a smooth run and an embarrassing death on floor 2.

| Enemy            | Floor | HP  | Behaviour                                      |
|------------------|-------|-----|------------------------------------------------|
| **Green Slime**  | 1+    | 20  | Moves slowly toward the player                 |
| **Blue Slime**   | 2+    | 35  | Splits into two small slimes on death          |
| **Spike Slime**  | 3+    | 45  | Shoots a spike projectile every 2 seconds      |
| **King Slime**   | 5+    | 80  | Charges at full speed when HP drops below 50%  |
| **Void Slime**   | 8+    | 120 | Teleports randomly; ignores walls              |

> [!WARNING] Blue Slimes
> **Always kill Blue Slimes last.** The two small slimes they split into can chain into more splits if you have bad AoE timing.

---

## Boss fights

A boss spawns at the end of floors **5** and **10**.

### Floor 5 — The Slime King

The Slime King has three phases:

1. **Phase 1 (100–60% HP):** Slow charge attacks. Dodge sideways.
2. **Phase 2 (60–30% HP):** Spawns 4 Green Slimes every 10 seconds.
3. **Phase 3 (30–0% HP):** Enrages — moves at 2× speed, spawns continuously.

```
Phase 3 damage formula:
  base_damage × 2 + (active_slimes × 0.5)
```

> [!DANGER] Don't let slimes pile up
> In phase 3, **clear the spawned slimes first** or their combined contact damage will shred even the Knight.

---

### Floor 10 — The Void Amalgamation

The final boss. It combines every slime type into one chaotic encounter.

> [!NOTE] No spoilers
> Figuring out the Void Amalgamation's pattern yourself is part of the experience. There's a reason the achievement is called *"Did you even read the docs?"*

---

## Tips for deep runs

- **Dodge roll has i-frames** — you are invincible during the animation. Use it aggressively.
- **The shop on floor 6 has a secret item** if you have exactly **0 gold** when you enter.
- Passive items **stack** — two *Iron Skins* gives double the armour bonus.
- Standing still for 3 seconds regenerates **5 HP**. This is often more useful than potions on low-HP characters.

> [!TIP] The 0-gold trick
> Spend every coin before floor 6 and the shopkeeper will respect your poverty with a **Cursed Rabbit's Foot** — arguably the best item in the game.
