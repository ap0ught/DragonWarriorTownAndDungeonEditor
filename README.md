# Dragon Warrior Town & Dungeon Editor

A map editor for the NES version of Dragon Warrior. This utility allows you to edit dungeon, castle, and town map data for all maps in the game.

![Dragon Warrior Town & Dungeon Editor](reference/DragonWarriorTownAndDungeonEditor.png)

## Features

- Edit all town, castle, and dungeon maps in Dragon Warrior (NES)
- Visual map editor with tile-by-tile editing
- Support for all map types (towns, castles, caves, shrines)
- Direct ROM editing capabilities
- User-friendly Windows Forms interface

## Requirements

- Windows operating system
- .NET Framework 3.5 or higher
- Dragon Warrior (U) (PRG0) [!].nes or Dragon Warrior (U) (PRG1) [!].nes ROM file (headered)

## Installation

1. Download the latest release from the [Releases](https://github.com/ap0ught/DragonWarriorTownAndDungeonEditor/releases) page
2. Extract the archive to a folder of your choice
3. Ensure you have .NET Framework 3.5 or higher installed
4. Run `DragonWarriorTownAndDungeonEditor.exe`

## Usage

1. Launch the application
2. Load your Dragon Warrior ROM file
3. Select the map you want to edit from the available locations
4. Click on tiles in the map to select them
5. Choose the tile type you want to place from the toolbar
6. Click on the map to place the selected tile
7. Click "Write ROM" to save your changes to the ROM file

**Important:** Always backup your ROM file before making any changes!

## Supported Locations

### Towns
- Brecconary
- Garinham
- Kol
- Rimuldar
- Cantlin

### Castles
- Tantegel Castle (Throne Room, Main Castle, Basement)
- Charlock Castle (F1, B1-B7)

### Dungeons & Caves
- Garinham's Grave (B1-B4)
- Erdrick's Cave (B1-B2)
- Rock Mountain Cave (B1-B2)
- Swamp Cave

### Shrines
- Rain Shrine
- Rainbow Shrine

## Important Notes

- **Visual Changes Only:** This utility currently supports visual changes only. For example, if a chest or stairs is added, the chest will not have any contents and stairs will not go anywhere. Game logic and scripting are not modified.

- **Special Tiles:** Tiles with a yellow border and cross have more than one purpose. When changing these tiles, it is recommended to use another tile with a yellow border and cross. These tiles correspond to roof placement and possibly other data/data pointers. Changing these tiles to regular tiles (and vice versa) could have unexpected results.

- **No Overworld Editing:** Overworld editing is not currently supported.

- **Loading Times:** Loading of some larger maps (30x30 grids) may take some time. On an Intel i7 first generation processor, loading time was approximately 8 seconds for a 30x30 map.

- **Backup Your ROM:** Always backup your existing ROM file before making changes in case something breaks.

## Building from Source

### Requirements
- Visual Studio 2013 or later
- .NET Framework 3.5 SDK

### Build Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/ap0ught/DragonWarriorTownAndDungeonEditor.git
   ```
2. Open `DragonWarriorTownAndDungeonEditor.sln` in Visual Studio
3. Build the solution (F6 or Build → Build Solution)
4. The compiled executable will be in the `bin/Debug` or `bin/Release` folder

## Tile Types

### Town/Castle Tiles
- Grass, Desert, Water
- Treasure Chest
- Solid Stone Wall
- Stairs (Up/Down)
- Red Brick Floor
- Forest, Poisonous Swamp
- Barrier, Locked Door
- Weapon Shop Sign, Inn Sign
- Bridge, Desk

### Cave/Dungeon Tiles
- Cracked Stone Wall
- Stairs (Up/Down)
- Red Brick Floor
- Treasure Chest
- Locked Door
- Princess Gwaelin
- Black Wall

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## Bug Reports

If you encounter any bugs or issues, please report them to the [Issues](https://github.com/ap0ught/DragonWarriorTownAndDungeonEditor/issues) page.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

- **Coded by:** Shawn M. Crawford [sleepy9090]
- **Original Release:** January 8, 2018
- **Version:** 1.0.0.28734

## Disclaimer

Dragon Warrior is a trademark of Square Enix. This tool is not affiliated with, endorsed by, or associated with Square Enix or any of its affiliates. This is a fan-made utility for educational and modding purposes only. Users must own a legal copy of Dragon Warrior to use this editor.
