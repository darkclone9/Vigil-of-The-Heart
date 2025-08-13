Vigil of the Heart (Fabric)
A techno-mystic Minecraft mod about guarding a dying god-heart on the fog-locked island of Tol. Build the Heart. Keep it alive. Hold the line.

Status: Concept → Prototype (planning & scaffolding). Contributions welcome.

🔮 Premise
On Tol—an island sealed by a living fog—an ancient Mechanical Heart is wired into a portal that once fed higher beings. Corporations want its power. Cults want its silence. You are the Vigil: a sworn protector keeping the Heart alive long enough to learn why it beats… and whether it should.

This mod blends medieval ritual with industrial tech: offerings, wards, and runes meet gears, conduits, and field emitters. Expect base defense, expedition raids, and long-form progression anchored to a single, very needy, very temperamental Heart.

🧰 Core Features (planned)
The Mechanical Heart (Multiblock)

Assemble a late-game multiblock “Heart” with valve rings, conduit arms, and a portal core.

Fuel it with Offerings (crafted items/fluids) to maintain Pulse, Heat, and Integrity.

Starve it, and the island wakes up angry.

Fog Barrier

Tol is a distinct dimension/region with a creeping fog wall. Venture too far without proper beacons → disorientation, decay, and teleport “snaps” back to sanctuary.

The Vigil Class

Lightweight class system with talents in Bulwark (defense/wards), Binder (rituals/offerings), and Breaker (saboteur/raid utility).

Unlock perks via Heart milestones (not XP grind).

Factions & Encounters

Corporate Saboteurs (ranged squads, signal jammers).

Worshipful Remnants (melee zealots, ritual disruptors).

Aetheric Wraiths (spawn on Heart instability).

Nightly/weekly Incursions scale with your Heart’s output.

Structures & Techno-Rituals

Pulse Beacons (push back fog, mark safe corridors).

Warding Anchors (AOE debuffs for invaders).

Offering Vats (item→essence processing).

Glyph Loom (inscribe runes onto gear).

Progression Loop

Stabilize the Heart (basic offerings).

Scout fog-thick ruins for fragments/blueprints.

Fortify (beacons, anchors, traps).

Withstand incursions and unlock new tiers.

Decide the endgame: feed, free, or extinguish.

Multiplayer Co-op

Shared Heart state; roles shine in coordinated defense.

Optional “Vigil Oaths” for team buffs/penalties.

Stretch ideas: REI/EMI integration, Trinkets/CCA hooks, data-driven raids, in-world codex.

📦 Compatibility
Loader: Fabric / Quilt (targeting 1.21.x)

Java: 21+

Gradle/Loom: Latest stable Loom (see gradle.properties)

Optional hooks (planned): REI/EMI, Trinkets, Cardinal Components API

If an integration is listed, it’ll be behind a soft dependency.

🗺️ World/Content
Dimension/Region: tol:vigil_island (custom noise + fog mechanics)

Loot/Blocks: conduit arms, valve rings, wardstone, offering vats, glyph loom

Items: heart keys, glyph plates, aether vials, signal scramblers

Mobs: saboteur scout, zealot binder, aetheric wraith, ruptured husk

Sound/FX: heartbeat intensity maps to Heart stability; fog chorus at boundaries

🧪 Building & Running
bash
Copy
Edit
# Clone
git clone https://github.com/yourname/vigil-of-the-heart.git
cd vigil-of-the-heart

# Build (dev)
./gradlew build

# Run client
./gradlew runClient

# Run server
./gradlew runServer
Import into IntelliJ IDEA or VS Code with Gradle.

Yarn mappings + Loom handle sources; no manual deobf needed.

⚙️ Config (WIP example)
toml
Copy
Edit
# config/vigil-heart.toml
[heart]
base_pulse=40            # ticks per beat
decay_per_minute=1.5
max_integrity=1000

[fog]
thickness=0.85
snap_back_distance=96    # blocks
beacon_push=32           # safe radius per tier

[incursions]
min_night=3
scale_per_milestone=0.2
🗂️ Repo Structure
bash
Copy
Edit
/src/main/java/com/tol/vigil/   # code
/src/main/resources/            # assets, datapacks
/datapack/                      # dev datapack examples
/docs/                          # design notes, diagrams
🧭 Roadmap
 Minimal Heart multiblock & UI (Pulse/Heat/Integrity)

 Offering pipeline (items → essence → upkeep)

 Fog boundary + beacon pushback

 First incursion (saboteur squad)

 Vigil talents (Bulwark/Binder/Breaker)

 Dimension polish, ruins, codex

 Balance pass + MP sync

 Content pack hooks & API

🤝 Contributing
PRs welcome. If you open an issue, include:

Game version, loader, logs

Repro steps and expected vs. actual

Screenshots for structure/visual bugs

Style: standard Fabric patterns, Yarn names, no hard singletons, prefer data-driven JSON where sane.

📝 License
TBD (MIT recommended). All art & audio must be yours or licensed appropriately.

🙏 Credits & Inspiration
Concept & lore inspired by the Tol setting (Vigil, the Heart, the fog barrier, corporate interference).
Dev stack: Fabric, Loom, Yarn. Thanks to the modding community for docs, tools, and brain cells.
