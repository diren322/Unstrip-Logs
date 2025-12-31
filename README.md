Unstrip Logs Mod

A Fabric QoL mod for Minecraft 1.21.11 that lets you revert stripped logs and wood back to their normal variants using an axe.

✨ Features

Right-click stripped logs or stripped wood with an axe to convert them back to normal logs

Fully vanilla-compatible behavior

✅ Client-side returns PASS → copper waxing and other vanilla axe actions still work

✅ Server-side returns SUCCESS only for stripped blocks

Custom animation system

Instant hand swing (client-side)

Two-stage sound effects (server-side):

First sound: deep axe hit (low pitch) for impact

Second sound: light wood sound (high pitch) for bark restoration

~150ms (3 ticks) delay for natural feedback

Block axis (X / Y / Z) is preserved

Axe takes 1 durability damage

No sneak (Shift) required

Designed to feel natural while still being a unique interaction

🪵 Supported Blocks
Stripped Logs → Normal Logs

Oak, Spruce, Birch, Jungle, Acacia, Dark Oak

Mangrove, Cherry, Pale Oak

Crimson Stem, Warped Stem

Stripped Wood → Normal Wood

All wood variants

Crimson Hyphae, Warped Hyphae

🎮 In-Game Experience

Player right-clicks a stripped log with an axe

Immediately:

Hand swing animation

Deep axe sound

~150ms delay for visual feedback

After 3 ticks:

Block converts back to normal

Light wood sound plays

Axe durability decreases by 1

This creates a non-magical, tactile restoration feeling instead of an instant toggle.

⚙️ Configuration

The mod can be enabled or disabled via Mod Menu

Config file:

config/unstrip-logs.json


Changes apply without restarting the game

📦 Installation

Install Fabric Loader

Install Fabric API

Download:

unstrip-logs-1.0.0.jar


Place it into:

.minecraft/mods

🛠 Technical Details

Minecraft Version: 1.21.11

Loader: Fabric

Java: 21

API: UseBlockCallback

Client/Server logic split

Axis-safe block replacement

Custom animation & sound handling

📜 License

© 2025 direnis. All Rights Reserved.

This project and its source code may not be used, modified, or distributed without explicit permission from the author.
