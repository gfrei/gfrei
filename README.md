# Hi, I'm Guilherme! Software Engineer | VR Unity Programmer
[LinkedIn](https://www.linkedin.com/in/freire-guilherme)

[CV](https://drive.google.com/file/d/1g2Pe8FSXlSC_umqzyZNWOg19g8SlP5iy/view?usp=sharing)

## Software Development Studios:
[Venturion VR](https://en.venturion.com.br/) (2018 - 2025)

[Tapps Games](https://tappsgames.com/) (2015 - 2018)

## Project Highlights:

### Slink & Snatch: Tales of Thievery
#### Trailer:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=55Qd2ugDzRI
" target="_blank"><img src="http://img.youtube.com/vi/55Qd2ugDzRI/0.jpg" 
alt="Slink & Snatch Demo" width="240" height="180" border="10" /></a>

[Meta](https://www.meta.com/experiences/8424782484259699/?require_login=true&utm_source=developer.oculus.com&utm_medium=oculusredirect)

**Tech**: Unity / C# / HurricaneVR / SECTR / VR

**Duration**: 3 years (2021-2024)

**Team**: 2 to 6 members, 1 to 3 programmers

#### Description:

**Slink & Snatch** is a cartoonish VR stealth game with a collectathon core loop, similar to Sly Cooper and Banjo-Kazooie. This was the most challenging project for the company due to its scale and ambition, featuring a large sandbox city to explore. It started in 2021 as a PCVR prototype and is currently in development, with a [Demo released on Meta](https://www.meta.com/experiences/8424782484259699/?require_login=true&utm_source=developer.oculus.com&utm_medium=oculusredirect).

#### Contribution highlights:
- **Enemy AI:** The enemy AI has a complex structure, with a state cycle, sensors to detect the player, and a NavMesh Agent. I implemented a Finite State Machine to handle its various states, switching between Patrol, Investigate, Chase, Shooting, and Searching. I also designed an interface to handle its sensors, including Vision, Hearing, and Touch, supporting the complex interactions required by the feature.
- **Sectorizing the city to enable asset streaming:** The city was huge and couldn't run on Quest 2. We needed to divide the terrain, streets, and rooms into smaller chunks that could be loaded and unloaded as the player moved through the city, using SECTR. I took on this task, dividing the city into multiple sections and focusing on keeping the triangle count within a limit for each one, using a neighbor-loading strategy. When the player is in a given section, only its neighboring sections are loaded. When changing sections, the new neighbors are loaded and the old ones are unloaded. We also needed to use portals to define when the player was moving between sections, as each area had complex interconnections and could overlap with others.
- **In-game book menu:** The player has a book that displays quest progress, a currency counter, and collectible progress with hints.
- **Dominant hand switching for left-handed players:** This feature was particularly challenging because it was added late in development, and the player's hands had not been designed with this change in mind.
- **Torch of Disillusion:** An item that reveals hidden objects on the map.
- **Health Potion:** A potion that restores all health when the player opens the bottle and turns it upside down near their head.
- **Lock and Key:** A feature that allows players to lock doors and chests and open them with a key.
- **Player and Game Configuration:** Implemented using ScriptableObjects.

---

### Dino Quest 2:
#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=gn_dYnYUzTI
" target="_blank"><img src="http://img.youtube.com/vi/gn_dYnYUzTI/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

[Android](https://play.google.com/store/apps/details?id=com.tapps.games.dig.dinoquest2&hl=en)

[iOS](https://apps.apple.com/br/app/dino-quest-2-museu-jur%C3%A1ssico/id1580107903)

**Tech**: Unity / C# / Firebase / Mobile

**Duration**: 1.5 years (2021-2022)

**Team**: 3 to 10 members, 1 to 4 programmers

#### Description:

**Dino Quest 2** is an exploration/management mobile game with two main mechanics: going on expeditions to find fossils and managing those fossils in the Museum. This was my first commercial Unity mobile game. I worked as the lead game programmer from day one until the 1.0 release, initially alongside another programmer, but mostly on my own. After release, the team grew to 4 programmers.

#### Contribution highlights

I implemented all the logic for the **exploration sites**:
- 3D grid where the fossils are placed
- The logical structure of the Fossil entity, including information such as size, body part, rarity, and 3D bounds
- The structure of each exploration site, including size, dinosaurs, fossil number range, difficulty, and terrain block tiles
- Placement logic and configuration, from fossils to terrain blocks

I implemented all the logic for the **Museum**:
- 2D grid where objects could be placed
- All actions related to object placement, such as movement, rotation, placement, placement validation, and removal
- Storage logic
- Dinosaur displays, showing only the fossil parts that the player had found
- NPC visitor lifecycle, including navigation inside the museum and animations

**Museum Upgrades**
- Expanding the museum through levels and currency
- Changing the grid space and transferring item data from one grid to another
- Updating visuals and NavMesh in each room
- Loading and unloading rooms as the player moves between them

**Expedition Selection Screen**
- Handling multiple UI elements on this screen, along with their logic
- A horizontal scroll list of expedition sites
- Free scrolling of the map to display each expedition's location
- Logic for displaying data about each site and its states (Locked, Purchase, and Open)

---

### BOSCH - Desafio de Eficiência

**Tech**: Unity / C# / DialogueSystem / PC

**Duration**: 4 months (2024-2025)

**Team**: 8 members, 2 programmers

#### Description:

Corporate training game inspired by Disco Elysium, in which I acted as the lead programmer, designing the architecture and implementing the main features. I also managed the other team members, delegating tasks and reviewing their work.

#### Contribution highlights
- Broke down the main features during pre-production and provided realistic time estimates
- Researched and implemented third-party libraries to speed up development
- Created a guide to help the team use those third-party libraries
- Implemented the core features
- Managed and delegated tasks to other team members

#### Feature highlights
- Dialogue System
- Save/Load
- Progression management
- Scoring system
- Interactable objects and NPCs
- 3D movement using the mouse or WASD keys

---

### LVSIM

[Video](https://drive.google.com/file/d/1xo6MqUfXaP9YXKHXBhJHaPWYLVtsZfMZ/preview)

**Tech**: Unity / C# / Photon / PlayFab / PC / Mobile

**Duration**: 1.5 years (2022-2023)

**Team**: 3 to 8 members, 1 to 2 programmers

#### Description:

LVSIM is a multiplayer hospital room simulator for educational purposes. The professor logs in, creates a room, and sets up a patient using the control panel. Students then enter the room and participate in an interactive medical class. I was the sole programmer from the start until the 1.0 launch, and worked with a junior developer on version 1.1.

#### Contribution highlights
I worked as the sole programmer until the 1.0 release, so I implemented all the application logic:
- Online entitlement logic using PlayFab, including login and permissions
- Real-time multiplayer logic with Photon, including rooms, roles, and players in each room
- Patient state synchronization between everyone in each room
- Text and voice chat between players
- Logic for each patient state option in the Control Panel

---

### Mine Quest 2
#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=S9E4GazGXVM
" target="_blank"><img src="http://img.youtube.com/vi/S9E4GazGXVM/0.jpg" 
alt="Slink & Snatch Demo" width="240" height="180" border="10" /></a>

[Android](https://play.google.com/store/search?q=mine%20quest%202&c=apps&hl=en)

[iOS](https://apps.apple.com/us/app/mine-quest-2-idle-mining-rpg/id1105121264)

#### Description:

Mine Quest 2 is a mobile mining exploration RPG.

**Tech**: Custom Engine based on Love2D / Lua / Firebase

**Duration**: 1 month (2017)

**Team**: Solo

**Contribution**: Performance

After a change in components, the mine scene was running very poorly, with the frame rate dropping below 1 FPS. I was responsible for optimizing this scene:
- My investigation showed that the scene had an average of 600 draw calls, reaching more than 1,400 at its worst.
- My main steps to improve performance:
  - Combined all background tiles into a single atlas tileset
  - Combined all interactable mine objects into another atlas
  - Changed the draw order to avoid breaking batches
  - Since battles take place in an overlay on top of the mine scene, I took a snapshot of the scene, displayed it behind the battle overlay, and hid the mine scene during battles
- After these changes, I reduced the average draw call count to 50 and enabled the game to run at 60 FPS on most target devices.

---

### Laser Storm Arena
#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=2vE8beTRD-I
" target="_blank"><img src="http://img.youtube.com/vi/2vE8beTRD-I/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

**Tech**: Unity VR / C# / Photon / VR

**Duration**: 1 year (2019-2020)

**Team**: 3 to 6 members, 2 to 3 programmers

#### Description:

Laser Storm Arena is a VR shooting arena game played in arcade venues, with 4 players playing together in person. Each session is timed, and the teams aim for the highest score by shooting enemies and avoiding damage. The game is played using 4 Quest headsets and a PC running the local server.

#### Contribution highlights
- **Shooting:** Synchronizing shooting states, enemy hits, and damage in a multiplayer environment
- **Basic Enemy AI:** Developing the decision-making, movement, shooting intervals, and waiting times of the basic enemy
- **Grabber enemy:** An enemy that remains static until a player looks at it. It then grabs that player, and the other players must shoot it.
- **Score and Leaderboard:** Scores are tracked individually during the session and summed at the end to determine the team score, which is saved on the host PC.
- **Player Avatar:** Each player has an animated avatar using IK.

<!--

---

### Bid Wars: Pawn Empire:

#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=a4yDEPUWVrs
" target="_blank"><img src="http://img.youtube.com/vi/a4yDEPUWVrs/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

**Tech**: Custom Engine based on Love2D / Lua / Firebase

**Duration**: 2 years (2017-2018)

**Team**: 8 to 10 members, 3 to 4 programmers

#### Description:
An auction game with a city management side loop.

#### Contribution highlights

---

<!--
**gfrei/gfrei** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
