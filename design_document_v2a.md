# TF2: Invasion – Design Canvas (Recreation Mod)

---

## Gameplay Overview
***TF2: Invasion*** is a team‑based objective shooter with deep resource management, base building, vehicle combat, technology progression and a tactical commander overlay.  
Two asymmetrical factions — **Humans** and **Aliens** — fight over Control Zones, Resource Zones and map‑specific objectives.  
Resources (Jojirium) are harvested from Resource Zones, destroyed buildings and fallen enemies; they are spent by players and commanders on Buildings, Vehicles, Technologies and resupply.

Human structures require **external power** from PowerPacks, but enjoy a **20% build discount**. Alien structures operate **self‑powered** but are balanced around cost and exclusivity.

A unique **Commander Mode** allows any player to enter an orthographic Tactical View, issue orders, mark tech desires and manage the team’s resource economy.

---

## Controls
| Action | PC (default) | Gamepad |
|--------|--------------|---------|
| Move | WASD | Left Stick |
| Sprint | Shift | LS Click |
| Jump / Double Jump / Wall Stick | Space | Ⓐ |
| Crouch (affects spread & fire rate) | Ctrl | RS Click |
| Primary Fire | Left Mouse | RT |
| Secondary Fire / Alt‑Fire | Right Mouse | LT |
| Throw Grenade 1 | F | LB |
| Throw Grenade 2 / Special | G | RB |
| Reload | R | Ⓧ |
| Scroll Weapons | Mouse Wheel | Ⓨ |
| Use / Build / Interact | E | Ⓑ |
| Voice Chat (Team) | V | — |
| Text Chat | Y | — |
| Team Text Chat | U | — |
| Commander Mode / Tactical View | M (or click minimap) | — |
| Place Building (commander) / Mark Tech | Click in Tactical View | — |
| Call Vote (Tech, surrender, etc.) | , (in Tactical View) | — |
| Change Class / Loadout | . | — |
| Taunt | H | — |

*Building placement, vehicle mounting and special abilities (e.g. Shield tracking toggle, Harpoon pull, EMP Generator) are all bound to context‑sensitive use and fire modes.*

---

## Factions & Asymmetry

### Humans
- Use **external PowerPacks** to run Sentries, Manned weapons, Shields, Buff Stations.
- Get a **20% cost reduction** on buildings.
- **Classes:** Commando, Defender, Medic, Pyro, Support, Sniper. (??)

### Aliens
- Buildings are **self‑powered** (no PowerPacks needed).
- Respawn originally used a **wave reinforcement system** (disabled per map preference in leak; we make it a server option).
- **Classes:** Recon, Sapper, Escort, Infiltrator. (??)

---

## Classes

### Human Classes

| Class | HP | Speed (hu/s) | Equipment | Abilities | Buildings |
|-------|----|---------------|-----------|-----------|-----------|
| **Recon** | 125 | 400 | Dual semi‑auto Laser Pistols, Shoulder‑mounted Stickybombs, Combat Knife | Double jump, wall stick (short duration) | Resource Pump, Respawn Station |
| **Sapper** | 150 | 310 | Drainbeam (drains health → energy), Shotgun (alt‑fire energy shot), EMP Grenades, EMP Generator | Boost (speed + damage resist), EMP effect on drained enemies, can steal Support’s deployed Mortar (cut – may be re‑added) | Respawn Station, Powerpack, Resource Pump, Manned Plasma Gun, Dragon’s Teeth, Tower, Sandbag Bunker |
| **Escort** | 250 | 260 | Laser Minigun, Personal Shield (tracks Projectiles or Hitscan), Shield Grenades | Shield tracking modes toggled by right‑click; blocks chosen category | Respawn Station, Powerpack, Resource Pump, Projected Shield (Shield Wall), Manned Shield, Sandbag Bunker, Bunker |
| **Infiltrator** | 125 | 320 | Laser Shotgun, Limpet Mines (detonated via Laser Designator), Knife (auto‑backstab) | Disguise as enemy (E), loot corpses (+20 resources), eavesdrop on enemy voice/team chat, thermal vision (short sight range). | Camera |
| **Commando** | 200 | 250 | Laser‑Designated Rocket Launcher, Plasma Rifle (parry to charge), Combat Shield, Plasma Grenades | Shield can be used any time; charge shot tech upgrades | Respawn Station, Powerpack, Resource Pump, Manned Missile Launcher, Dragon’s Teeth, Sandbag Bunker, Vehicle Boost upgrade |
| **Defender** | 125 | 300 | Laser Shotgun, Limpet Mines (laser‑detonate), Arc Welder (weld doors shut), Combat Shield | Build multiple Sentries (tech upgrades); repair buildings | Respawn Station, Powerpack, Plasma Sentry Gun, Manned Missile Launcher, Barbed Wire, Bunker, Sandbag Bunker, Tower, Dragon’s Teeth, Driver Machinegun upgrade |
| **Medic** | 150 | 320 | Repair Gun (heal + repair, disarms grenades on target), Burst Rifle, Anti‑Personnel Grenades, Combat Shield | Overheal; techs: Selfheal, Resupply Station | Respawn Station, Powerpack, Resource Pump, Buff Station, Manned Plasma Gun, Resupply Station (tech), Selfheal upgrade |
| **Pyro** | 150 | 290 | Flamethrower (primary), Gas Can (secondary pours gasoline, ignites longer-lasting flames), Shotgun | Flames stick to surfaces; gasoline traps chain‑ignite. Immune to afterburn. | None (last class added) |
| **Support** | 200 | 270 | Plasma Grenade Launcher, Harpoon (pull enemies, secondary slap: 2‑hit kill), Deployable Mortar (aim like Wii Bowling) | Mortar can fire Smoke, Starburst (flash), MIRV rounds (tech). Tallest class (~12 ft). | Respawn Station, Powerpack, Resource Pump, Mortar (building), Sandbag Bunker, Bunker, Explosives upgrade |
| **Sniper** | 125 | 290 | Sniper Rifle (hitscan), Laser Rifle, Combat Knife, Indicator Grenade (design target) | Stealth Deploy tech: invisible while prone (head visible). Can mark respawn locations via tech. | None |


---

## Weapons (Selected)

| Weapon | Type | Base Damage | Ammo (carried/reserve) | Attack Interval (s) | Special |
|--------|------|-------------|------------------------|---------------------|---------|
| Dual Laser Pistols | Projectile (laser) | 25 | 16 / 48 | 0.3 | Dual‑wield |
| Stickybombs | Projectile (grenade) | 100 (max falloff) | 3 | — | Stick to surfaces, detonate manually |
| Rocket Launcher | Projectile (rocket) | 100 (max falloff) | 1 / 20 | 0.8 | Rockets follow laser designator; no rocket jump |
| Plasma Rifle | Projectile (plasma) | 30 (uncharged) / 60 (charged) | 27 / 81 | 0.2 | Parry charges next shot (green indicator); tech: auto‑lock charge |
| Drainbeam | Beam (constant) | 15 / sec | Infinite (energy) | Continuous | Drains health into Sapper energy; applies EMP to target |
| Shotgun | Hitscan (grid) | 10 × pellet | 6 / 30 | 0.8 | TF2 shotgun |
| Limpet Mines | Projectile (mine) | 120 | 2 | — | Toss, detonate via Laser Designator in order of placement |
| Arc Welder | Beam (short range) | 5 / sec to buildings | Infinite | Continuous | Repairs buildings, welds doors shut |
| Repair Gun | Projectile (bolt) | 50 / sec (heal/repair) | 1 / 38 | 0.7 | Heals players, repairs buildings, disarms grenades on healed target |
| Flamethrower | Particle (fire) | 6‑12 / particle | 200 fuel | Continuous | Flames stick to world; ignition propagates along gasoline trails |
| Gas Can | projectile (gasoline) | 0 | 5 cans | — | Pours gasoline; when ignited by flame, creates lasting fire trap |
| Harpoon | Projectile + melee | 10 (harpoon) / 75 (slap) | 1 (until respawn) | Slow pull | Pulls enemy; can be broken; secondary one‑hit kill slap |
| Plasma Grenade Launcher | Projectile (grenade) | 90 max | 4 / 12 | 0.6 | Direct impact detonation; green trails (friendly), red (enemy) |
| Laser Minigun | Projectile (laser) | 12 / bullet | 200 | 0.1 | Wind‑up; fire rate increased when crouched |
| Personal Shield | Equipment | blocks 100% tracked damage | Shield health bar | — | Toggle tracking: Projectile / Hitscan; depletes and recharges |
| EMP Grenade | Projectile (grenade) | 0 + EMP effect | 2 | — | Disables buildings, shields, certain weapons; disables ammo boxes |
| EMP Generator | Deployable building | EMP pulse | 1 | — | Seeks enemy buildings in range, constantly EMPs them |
| Mortar (Support deployable) | Projectile (mortar) | 120 (normal) | 6 | 3 | Alt‑ammo via tech: Smoke (low dmg, obscures), Starburst (blinding), MIRV (splits into two) |
| Sniper Rifle | Hitscan | 50‑150 (charged) | 5 / 20 | 1.5 | Standard scoped sniper; indicator grenade marks target for team |
| Knife (Infiltrator) | Melee (back) | instant kill | — | 0.5 | Auto‑locks onto back; disguise preserved |

*All weapons with "grenade" type are thrown and resupplied at Resupply Stations.* 

---

## Buildings & Power System

### Human Power
Human buildings that consume power must be placed within range of a **PowerPack**. Each PowerPack can power up to **4 buildings** (including other PowerPacks). Unpowered devices are inactive.

### Alien Buildings
All alien structures are self‑powered.

### General Buildings (both teams, unless noted)
| Building | Cost | Description |
|----------|------|-------------|
| Resource Pump | 100 | Placed on a Resource Zone. Harvests resources; yield shared equally among team. Only one per zone. |
| Respawn Station | 150 | Allies can choose to respawn here instead of default spawn. Replaces Teleporter. |
| PowerPack (Human only) | 80 | Powers up to 4 buildings. Chainable. |
| Buff Station (Medic) | 120 | Buffs plugged‑in players and buildings (+health, +accuracy). |
| Manned Plasma Gun | 200 | Stationary plasma turret; player‑manned. Buffable. |
| Manned Missile Launcher | 250 | Stationary rocket launcher; buffable. Can’t be rotated once placed. |
| Manned Shield (Escort) | 150 | Manned directional energy shield for cover. |
| Resupply Station (Medic tech) | 300 | Dispenses health, ammo and grenades for resources. Evolved Dispenser. |

### Defensive Structures
| Building | Cost | Notes |
|----------|------|-------|
| Sandbag Bunker | 50 | Quick low cover. |
| Bunker | 150 | Tall, ladder for roof access. |
| Tower | 100 | Elevated view, destructible. |
| Dragon’s Teeth | 30 per tooth | Anti‑vehicle barrier; must be placed in rows. |
| Barbed Wire (Defender) | 60 for two posts | Laser tripwire between two posts; huge damage on crossing. |
| Projected Shield / Shield Wall (Escort) | 200 | Rotatable energy wall blocking projectiles/hitscan depending on setting. |
| Tunnel | Map‑placed | Teleports players across map; footstep sounds play. |

### Sentries & Anti‑Personnel
| Building | Team / Class | Damage | Notes |
|----------|--------------|--------|-------|
| Plasma Sentry Gun | Defender | 25 per shot | Medium fire rate, self‑recharging ammo. Buffable. Tech: up to 3, Rocket Sentry, longer range. |
| Rocket Sentry Gun (Defender tech) | Human | 60 | Slower, high damage. |
| Mortar (building) | Support | 120 | Stationary mortar. Tech upgrades for special rounds. |

### Vehicle Upgrades (apply to friendly vehicles)
| Upgrade | Effect |
|---------|--------|
| Self‑Heal | Slow health regen for building. |
| Vehicle Boost (Commando) | Speed increase. |
| Driver Machinegun (Defender) | Mounts MG usable by driver. |
| Explosives (Support) | Building detonates on death. |

---

## Vehicles
Built at vehicle bays with team resources. Drivers and passengers can fire personal weapons.

| Vehicle | Faction | Description |
|---------|---------|-------------|
| Wagon | Both | Light transport; can carry one building. Drive‑by building possible. |
| Motorcycle | Both | Fastest vehicle, no combat capability. |
| Flatbed Truck | Both | Can hold multiple buildings; slow but sturdy. |
| Battering Ram | Both | Truck with ram; destroys buildings & players in path. |
| Siege Tower | Both | Mobile tower with ladder; great for elevated attacks. |
| Mortar Vehicle | Both | Mobile mortar; normal shells only. |
| Skirmisher (Tripod) | Alien | Dual MG, can crouch/move; halts to fire. |
| Mini Skirmisher | Alien | Faster, lighter version. |
| Tank | Alien | Heavy armour, powerful cannon; bobbing suspension. |
| Teleport Station | Both | Teleports players to marked point; can telefrag enemies. Map‑placed. |

---

## Resources & Economy
- **Resource Zones:** map‑defined areas with a finite pool that refreshes periodically. Emit sound when active. Yield resource chunks.
- **Gathering:** automatic via Resource Pump (equal team split) or manual pick‑up of chunks. Enemies drop 20 resources on death. Destroying buildings yields resources.
- **Spending:** used for buildings, vehicles, tech tree purchases, Resupply Station services (health/ammo/nades).
- **Team Bank:** resources collected by pumps go to a shared pool. Players retain personal stash from kills/loot.

---

## Technologies (Tech Tree)
Technologies are global team upgrades purchased with team bank resources via a **vote** initiated in Commander Mode. Marked desires help commanders decide.

### Techs
- **Defender:** x2 Sentries, x3 Sentries, Sensors (range), AI (faster lock), Rocket Sentry.
- **Medic:** Resupply Station, Selfheal.
- **Commando:** Target Info (enemy health/name), Rallyflag (replace grenade), AutoBoot (kick melee), Adrenaline Rush, Battle Cry, Bull Rush.
- **Sniper:** Stealth Deploy, Respawn Marker.
- **Support:** Mortar Range, Starburst Rounds, Cluster (MIRV) Rounds.
- **Global:** Charged Plasma auto‑lock, Shield Parry (shield bash melee).

- **Sapper:** EMP Recharge x2, Medium Range EMP, Longer EMP, Huge Range EMP.
- **Infiltrator:** Corpse‑Consuming (already baseline, likely boost).
- **Recon:** Radar Scanners (track enemies on minimap for team).
- **Escort:** ??.
- **Global:** Burst Plasma (plasma rifle burst when parried), etc.

*Purchased techs permanently unlock for the team until match end.*

---

## Commander Mode & Tactical View
- Accessible by **any player** at any time (default M, or click minimap).
- **Orthographic RTS‑style view** (not top‑down).
- **Orders system**: Heal, Build Sentry, Build Shield Wall, Kill Mortar Guy, Shell Enemy/Mortar Attack, Repair Building, Build Resource Pump, Build Resupply Station.
- Players on the ground see glowing HUD hints and waypoints.
- **Tech voting** and **marking desired technologies**.
- **Wave Reinforcement** (Alien only): dead Aliens spectate in Tactical View, can still issue orders until all aliens die; then wave respawns simultaneously.

---

## Map Hazards & NPCs
### Bugs (Third Faction)
- **Bug Hole:** spawns up to 4 Bugs; can be sapped. Emits smoke on entry/exit; tips over on death.
- **Bug Warrior:** 150 HP, half player height. Slash attack (20 dmg). Aggressive against Sentries. If hole dies, seeks new hole.
- **Bug Builder:** disabled, would have constructed defenses.

### Meteors
- Spawn in sky, transition into play area.
- Deal **200 damage** on direct hit. Drop resource chunks on impact.

### Falling Rocks
- Purely cosmetic, infinite, from cliffside maps.

---

## Hints System
- Dynamic tutorial overlay that highlights HUD elements and explains mechanics (e.g., “Build a Resource Pump here”).
- Triggered contextually; draws from the chunk of code preserved in both Invasion and early TF2 leaks. Fully functional in the mod.

---

## Narrative Design
**Backstory**:
???

---

## Art & Audio Direction
- Faithful to the leaked assets and concept art.
- Alien buildings: organic / chitinous, Humans: industrial / scrap.
- Distinct soundscape for Resource Zone activation, Bug Hole emissions, shield depletion, EMP pulses, etc.

---

## Technical Notes
- Based on Source Engine (TF2 branch).
- Netcode must handle up to 32 players, vehicles, hundreds of buildings.
- Commander mode uses ortho camera with fog‑of‑war (team vision only).

---
