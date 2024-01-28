# Global Game Jam 2024 Project

Diversifiers:
Mouthing Off
Full Steam Ahead


## Team
- Vi Prime      @vprime             Art / Programming
- Tyler Shauger @Tyler-Shauger      Programming / UI / Level Design
- Will Kostecki @WillKostecki       Art / Programming
- Isaac Pahona  @CheftoTheLeft      artificial intelligence / Art / Programming
- Valarie Adams @deviantdear        Sounds
- Tutu                              Moral Support

---

# Game Design
A third person action game of Cat and Mouse with physics in Unreal Engine.

### Theme: Make Me Laugh
The game will be funny though the use of physics

## Mechanics
Overdone physics
Third person
Chase a mouse
Claws out will grab some objects
Claws can get stuck in things
Human/Cat animations
Ragdoll when knocked down
"Self righting"
Target platform: WebGL


## Story

### Characters
- Cat
- Mouse 
  - Steamboat willie
  - Or computer mouse
  - Flys
  - Birds
  - Chuaua
  - Another cat

### Setting
Bookstore setting

### Game
- Object loading
- User pause
- Opening animation
- Menu screen
  - Start Game
  - Settings
  - Exit
- Settings
  - UI Interface for changing any settings we make available.
  - Sound controls
- Start Game
- Setup game
- Game Entrypoint animation
- Game start
- Game loop
- Game end
- Failure mode animation
- Win mode animation
- Game cleanup
- Failure Menu screen
- Win mode Menu screen

#### Game Loop
- Chase mouse
- Traps
- Mice spawn
- Tackle mouse
- Time limit?
- Mouse overrun limit?
- Protected object

### User Interface
Respawn button
Maybe a way to quit

### Technical
Sticky objects
Oily / Gross
Liquids
Springs or force

Stink physics


#### Requirements
- [x] Vi: Player input   
- [x] Vi: Player model (Cat)
- [x] Vi: Animation controller
- [ ] Isaac: NPC controller (Mice, Dogs, Birds, People)
- [ ] Isaac: NPC spawner
- [x] Trap controller 
- [ ] Vi: Hazards (Mousetraps, Exploding barrels, Water, Catbox, Sleeping dogs, Glue traps, Sticks to you)
- [ ] Will: Primary game mode (Capture rodents)
- [x] Vi: Grab and Hold Rodents
- [ ] Will: Win handler (Rodent capture count)
- [ ] Tyler: Loose handler (Time limit or a rodent target)
- [x] Tyler: Game main menu
- [x] Tyler: Pause menu
- [ ] End game
- [ ] Reset game
- [x] Will & Tyler: Scene static layout
- [x] Will & Tyler: Scene dynamic layout
- [x] Will & Tyler: Scene static lighting
- [x] Will & Tyler: Scene dynamic lighting
- [ ] :akko-shrug: Game Story
- [ ] Opening Storyboard
- [x] Tyler: Opening graphics
- [ ] Opening sequence programming
- [x] Tyler: Win graphics
- [x] Tyler: Loose graphics
- [ ] Settings


## Progress


### Monday 1-22
Planning
Learning Unreal
Will is starting on Environment
Vi is starting on Cat
Tutu is playing pokemon

### Tuesday


### Wednesday
Merged in Cat with walk, run, jump, and bap

### Thursday 
merged in UI from tyler
merged in tackle from Vi

### Friday


### Saturday


### Sunday 1-28 
Release day


### Cat Animations 30fps
- [x] Rig
- [x] Walk in place (30fps 82frames 6 steps Start from Left foot)
- [x] Walk forward (30fps 56frames 6 steps Start from Left foot, about 12 frames a step)
- [x] Run Forward (30fps 57frames 6 steps Start from Left food, about 7 frames a step)
- [x] Land (26 frames)
- [x] Jump (26 frames)
- [x] Fall loop (90 frames)
- [x] Idle (227 frames)
- [x] T Pose
- [x] Grab right arm
- [x] Grab left arm
- [x] Sleeping
- [x] Cleaning

Cat walking
front right up and forward
rear left up and forward just before last foot starts going down


Cat Running

### Hazards
- Glue spill (Grabs objects, makes it hard to move until broken free)
- Explosion (Impulse effect)
- Sticky objects (Sticks to whatever touches it, hard to remove)
- Spawn hazard actors
- Knockout (Temp Ragdoll effect on animated bodies)

#### Glue spill hazard
In the simplest form, this would be an object that will stick to other physical objects when they touch.
If we want to get fancy, I think a parent object could allow the glue to flow around.
A spawner could pour out a bunch of these physical glue balls, then when a dynamic body touches it the actual glue would trigger and hold.

Current issues
- Cat don't stick, probably because it's non physical
- Need to dial in the stickyness, but that will depend on the cat.

