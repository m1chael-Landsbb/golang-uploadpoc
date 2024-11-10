# CascadeRealmsTheTileGame
A tile-matching puzzle game with strategic battles, cross-platform compatibility, and future support for gaming platforms and Discord Bot.

# CascadeRealmsTheTileGame

A tile-matching puzzle game with strategic battles, cross-platform compatibility, and future support for gaming platforms and Discord Bot.

---

> **All graphics and visual assets in this project are original work by the author (cascadedev) and are not taken from any existing game or resource.**
>
> **Todos los gráficos y recursos visuales de este proyecto son creaciones originales del autor (cascadedev) y no han sido tomados de ningún otro juego ni recurso existente.**
>
> *This project is inspired by the dynamic mechanics of the Avalanche slot series by Microgaming. All assets, narrative, and code in this project are original creations and not affiliated with or endorsed by Microgaming.*
>
> *Este proyecto está inspirado en las mecánicas dinámicas de la serie Avalanche de Microgaming. Todos los assets, narrativa y código de este proyecto son creaciones originales y no están afiliadas ni aprobadas por Microgaming.*

---

## Description

- Align tiles on a tile-matching grid to attack, defend, and accumulate power.
- Real-time (or turn-based) confrontations against other players, each with their own grid and Guardian.
- Four initial Guardians, each representing an element, a realm, a region of the cosmos, and a cardinal axis.
- Every alignment of 3 or more tiles creates **barrier zones** on the grid, preventing players from acquiring more tiles of the same element until they are cleared.
- Cross-platform support: Web, mobile, tablet, and future **Discord Bot**.
- Future plan to port to Unreal, Godot, or Unity.
- **Gaming platform vision:** Future integration for tournaments, competitions, and rewards.

---

## Inspiration from Avalanche (Microgaming)

Cascade Realms is also inspired by the dynamic mechanics of Avalanche series by Microgaming:

- **Expandable grid:** The play area starts compact and can expand during gameplay, activating new rows and more winning patterns, similar to Avalanche mechanics.
- **Flow mechanics:** Tiles don't simply cascade down—they can shift horizontally, enabling new alignments and strategic opportunities.
- **Progressive amplifiers:** Special symbols that reach the grid's boundaries or bottom can activate or amplify powerful multipliers for subsequent matches.
- **Surge rounds:** Periodically, the grid enters a special "surge state," with all rows and amplifiers active, for massive potential combinations and rewards.

---

## Story

The narrative of **Cascade Realms** chronicles how four Guardians, each from different corners of the Cosmos and representing the four cardinal axes and four elements, compete and cooperate in an ancient tournament where nature and strategy intertwine.

Each Guardian represents an element and a territory, united by elemental power. Their essence and element also symbolize the region of the cosmos they originate from, adding diversity, lore, and depth to the game universe.

---

## Guardians: Selection, Identity and Expansions

At the start of gameplay, each player selects a Guardian—visible beside their grid and representing a cardinal axis and an element:

- **Guardian Pyrox** (South, Fire, Crimson)
- **Sentinel Aquis** (North, Water, Azure)
- **Warden Terrax** (West, Earth, Emerald)
- **Sage Aeris** (East, Air, Amber)

Each Guardian's avatar appears next to their grid, displaying their unique appearance and elemental affiliation.

**Expansions:**  
New Guardians can be added in future updates—simply add their image to `assets/guardians/` and update the `GUARDIANS` array in `src/game/player.ts`.

---

## Game Tile Design

- Puzzle tiles are **hexagonal**, each one representing an element (essence/character).
- Each tile features a special visual design:
  - **Luminance and gradients** for a sense of depth and premium quality.
  - **Subtle textures** and graphic details to differentiate each element (frost patterns, ember sparks, stone textures, wind swirls, etc).
  - **Not flat hexagons**—they have illumination and graphic effects to stand out on any screen.
- This design works well on web, mobile, tablet, Discord Bot, and future gaming platform adaptations.

**Visual examples:**  
- Crimson (Fire): Luminous hexagon with ember particles.
- Azure (Water): Hexagon with cool luminance and frost patterns.
- Emerald (Earth): Hexagon with stone texture and golden highlights.
- Amber (Air): Hexagon with wind swirls and warm luminance.

---

## Online Confrontations & Rankings

- **Duel mode:** Two players compete in real-time, each with their own grid and Guardian. Strategic moves and combinations can send obstacles or effects to the opponent's grid.
- **Real-time multiplayer:** Built using websockets for responsive and interactive gameplay.
- **Victory & Advancement:** The winner is determined by score, efficiency, or defeating the rival Guardian. Results are transmitted to the server.
- **Rankings:** Track the top players globally, with live rankings and historical statistics.

---

## Technologies

- Frontend: PixiJS + TypeScript (Web, mobile, tablet, Discord Bot)
- Backend: Node.js (Express/Fastify) for matchmaking and multiplayer logic
- **Future:** Port to Unreal, Godot, or Unity for enhanced and gaming platform versions.

---

## Structure

```
CascadeRealmsTheTileGame/
├── src/         # Game code (frontend)
│   ├── game/
│   │   ├── player.ts
│   │   ├── grid.ts
│   │   ├── renderer.ts
│   └── network/
│       └── socket.ts
├── server/      # Backend (Node.js)
│   ├── index.js
│   └── database.js
├── assets/      # Images, audio
│   └── guardians/   # Guardian avatars
│   └── tiles/       # Tile sprites
├── docs/        # Documentation and design
│   └── guardians-expansion.md
├── public/      # Static files
└── README.md
```

---

## Roadmap

1. Playable prototype on web, mobile, and tablet
2. Matchmaking and real-time confrontations
3. Advancement and rewards system
4. Discord Bot integration
5. Support for tournaments and competitions (gaming platform)
6. Port to Unreal/Godot/Unity

---

## Quick Install (Frontend)

```bash
npm install
npm run dev
```

## Backend install (Node.js)

```bash
cd server
npm install
npm start
```

---

## Contributing & Contact

Pull requests, ideas, and collaborations are welcome!  
Author: **cascadedev**

---
