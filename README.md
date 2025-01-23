# WayBackHome Game

This repository contains a Roblox game script designed as an adventure to find a way back home. Players navigate through challenges such as moving ice walls, coolable hot lava, invisible steps, and a riddle hidden within a campfire. This project is a great starting point for learning Roblox scripting concepts, including `BodyPosition`, `BodyGyro`, and interactive gameplay mechanics.

## Features

- **Moving Ice Walls:** Three ice walls move up and down between predefined points at varying speeds, maintaining their orientation with `BodyGyro`.
- **Coolable Hot Lava:** Hot lava sections that can be cooled down to create a safe path for players.
- **Invisible Steps:** Hidden steps that require players to explore and uncover their positions.
- **Campfire Riddle:** A riddle embedded within a campfire, adding an element of puzzle-solving to the adventure.
- **Script Optimization:** Tables and loops are used for clean and maintainable code, allowing easy customization and scalability.

## Getting Started

### Prerequisites

- Roblox Studio installed on your computer.
- Basic understanding of Lua scripting.

### Installation

1. Clone the repository or download the script directly.
2. Open Roblox Studio and create a new project.
3. Insert the following elements into the Workspace:
   - **Ice Walls:** Three walls, each containing:
     - A `top` part (to define the top position).
     - A `bottom` part (to define the bottom position).
     - An `iceWall` part (the moving wall).
   - **Hot Lava:** Lava parts that can transition to a cooled state.
   - **Invisible Steps:** Parts that are initially invisible but can be discovered during gameplay.
   - **Campfire:** A part with an interactive riddle.
4. Paste the script into a Script object within the Workspace.

### Script Overview

The script employs a modular approach to manage various gameplay elements, making it efficient and easy to expand. Key configurations include:

- **Ice Walls:**
  ```lua
  local walls = {
      {top = game.Workspace.Wall1.top, bottom = game.Workspace.Wall1.bottom, iceWall = game.Workspace.Wall1.iceWall, speed = 3},
      {top = game.Workspace.Wall2.top, bottom = game.Workspace.Wall2.bottom, iceWall = game.Workspace.Wall2.iceWall, speed = 5},
      {top = game.Workspace.Wall3.top, bottom = game.Workspace.Wall3.bottom, iceWall = game.Workspace.Wall3.iceWall, speed = 2},
  }
  ```

- **Coolable Hot Lava:** Transition states to enable safe passage.
- **Invisible Steps:** Detection and discovery mechanics.
- **Campfire Riddle:** Interactive logic for solving the puzzle.

This repository offers a foundation for creating engaging adventure games on Roblox, combining movement, interaction, and problem-solving to enhance gameplay.

