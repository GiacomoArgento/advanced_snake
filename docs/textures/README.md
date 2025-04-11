# 🎨 Textures docs
Make your snake stand out. Reskin the apples. Redefine the walls.
__Advanced Snake__ supports full texture customization for every game element — all configured through easy-to-edit files.

## 📁 Where Textures Are Stored
Textures are organized into folders based on what they represent:
```
textures/
├── snakes/    ← Textures for each snake
├── food/      ← Textures for apples
├── walls/     ← Textures for walls
└── backgrund/ ← Textures for the bacground
```
Each folder contains `.png` files that can be referenced dynamically at runtime.

## 🧠 How the Game Loads Textures
Texture names are pulled directly from the main config file 📄`config.toml` and `.yml` files for players

These are the default texture settings:
- `config.toml`
    ```toml
    [apples]
    textures = "apple.png"

    [walls]
    textures = "default.png"

    [background]
    textures = "default.png"
    ```
- `.yml` files
    ```toml
    textures: 'default.png'
    ```

## 📌 Texture Assignment by Type
| Type | Source of Texture Info | Location |
| ------- | ------- | ------- |
| Snake | Set per-player in `players/*.yml` | `textures/snakes/` |
| Food | Set in `config.toml` | `textures/food/` |
| Walls | Set in `config.toml` | `textures/walls/` |
| Background | Set in `config.toml` | `textures/background/` |

<br>

Each section has its own detailed guide:
- 🐍[`Snakes`](./snakes.md) – How to design full snake spritesheets
- 🍎[`Food`](./food.md) – How to add custom apples or bonus items
- 🧱[`Walls`](./walls.md) – How to reskin map walls
- 🎑[`Background`](./background.md) – How to reskin background tiles