# System Intelligence: Game

## Design

### Gameplay Loop

- multiplayer, with one player as the host
  - the others share the host's world
- realtime with pause/slowdown for movement & exploration
  - increase time/unpause as a vote, slow time/pause individually triggered
- turn-based on the adventuring/campaign level
  - turns pass on:
    - adventure step completion
    - hyperspace jumps
    - combat end
    - manually by the player
  - the world evolves when a turn passes

#### Core Loop (_second-to-second gameplay_)

- move spaceship within the open-world universe

#### Secondary Loops (_minute-to-minute gameplay_)

- exploration
- combat
- trading
- build & alter holdings (planets/outposts/space stations/spaceships)

#### Wider Loops (_long term goals and planning_)

- gain experience
- expand total holdings

### Game Systems

- open world galaxy
- flight
  - physics-driven
    - propulsion impulses
    - no _magical_ drag in space slowing down movement
    - inertial movement based on placement of thrusters & ship size/weight
    - gravity from solar bodies
- companion control
  - controlled by AI
  - players can design decision trees for them to utilise
- spaceship design
  - build spaceships from components (on a grid?)

## Dev

### Plugins

- **Installed:**
  - LE Extended Standard Library (installation)
- **Activated:**
  - Chaos Niagara
  - Harmonix
  - Json Blueprint Utilities
  - Modelling Tools Editor Mode
  - Niagara
  - Niagara Fluids
  - Physics Control
  - PCG Biome Cire
  - Procedural Content Generation (PCG)
  - Quixel Bridge
  - Serialization Utils
  - Soundscape
  - Static Mesh Editor Modelling
  - UMG Viewmodel
- **Removed**
  - Studio Telemetry

### Game Levels & Screens

- **levels**
  - Landing page
  - Hyperspace (between galaxies?)
  - Galaxy
- **screens**
  - Settings
  - holdings design
  - holdings management
    - empire
    - planet
    - outpost
    - space station
    - spaceship

### Data Structures

- Preconfigured
  - data (in csv and/or json) should be loaded when the game starts
- Live
  - saved normally
