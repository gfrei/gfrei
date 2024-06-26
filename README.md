# Hi, I'm Guilherme! VR Unity programmer
[LinkedIn](https://www.linkedin.com/in/freire-guilherme)

[CV](https://drive.google.com/file/d/1lIoYRoXxsfjYGYJAGqcF4RzOvYoVYOUt/view?usp=sharing)

## Software Development in studios:
[Venturion VR](https://en.venturion.com.br/) (2018 - current)

[Tapps Games](https://tappsgames.com/) (2015 - 2018)

## Project Hightlights:

### Slink & Snatch: Tales of Thievery

<a href="http://www.youtube.com/watch?feature=player_embedded&v=55Qd2ugDzRI
" target="_blank"><img src="http://img.youtube.com/vi/55Qd2ugDzRI/0.jpg" 
alt="Slink & Snatch Demo" width="240" height="180" border="10" /></a>


**Tech**: Unity / C# / HurricaneVR / SECTR / VR

**Duration**: 3 years (2021-2024)

**Team**: 2 to 6 members, 1 to 3 programmers

#### Description:

**Slink & Snatch** is a cartoonish VR Stealth Game with a Collectathon core loop, something like Sly Cooper and Banjo & Kazooie. This was the most challenging project for the company due to its scale and ambition, with a big sandbox city to explore. It started in 2021 as a prototype for PCVR and is currently in development, with a released [Demo on Meta](https://www.meta.com/experiences/8424782484259699/?require_login=true&utm_source=developer.oculus.com&utm_medium=oculusredirect). 



#### Contribution highlights:
- **Enemy AI:** The enemy is a complex structure, it has a state cycle, sensors to find the Player, a Nav Mesh Agent. I implemented a Finite State Machine to deal with its many patroling states, changing between Patrol, Investigate, Chase, Shooting, Searching. I achictecture an interface to deal with its sensors, inclusing Vision, Hearing and Touch, to deliver the complex design interactions needed in the feature.
- **Sectorize the city to enable asset streaming:** The city was huge and couldn't run on Quest 2. We needed to divide the terrain, streets and rooms into small chunks to load/unload them while the player was traversing, using SECTR. I took this task, divided the city in many sections, focusing on a limited tri count on each one, and using a neighbour loader strategy. When the Player is in a given Section, only its neighbours are loaded. When changing sections, the new neighbours got loaded and the old one unloaded. It was also needed to use portals to define when the Player was moving between sections, as each area had complex interconnections, and could be inside one another.
-  **In-game book menu:** The Player has a book that shows quests progress, currency counter, collectables progress with hints
-  **Dominant Hand Changing por left-handed players:** This feature was actually very challenging, because it was a late addition, the Player's hands were not developed with this change in mind
-  **Torch of Disillusion:** This item reveals hidden objects on the map
-  **Health Potion:** A potion has heals all health when the Player open the bottle and turns it close the head
-  **Lock and Key:** A feature of locking doors and chests, and opening it with a key
-  **Player and Game Config:** using with SciptableObjects

---

### Dino Quest 2:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=gn_dYnYUzTI
" target="_blank"><img src="http://img.youtube.com/vi/gn_dYnYUzTI/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

**Tech**: Unity / C# / Firebase / Mobile

**Duration**: 1.5 years (2021-2022)

**Team**: 3 to 10 members, 1 to 4 programmers

#### Description:

**Dino Quest 2** is a exploration/management mobile game with two main mechanics, going on expeditions to find fossils, and managing the fossils in the Museum. This was my first commercial Unity mobile game, I worked as the lead game programmer from day 1 to 1.0 release, initially with another programmer, but mostly alone. After release, the team increased to 4 programmers.

#### Contribution highlights
I've made all the logic in the **exploration sites**:
 - 3D grid where the fossils are placed
 - The logical structure of the entity Fossil, including informations such as size, body part, rarity, 3D bounds
 - The structure of each exploration site, such as size, dinos included, fossil number range, dificulty, terrain block tiles included
    The placement logic and configuration, from fossils to terrain blocks
   
I've made all the logic in the **Museum**:
 - 2D grid where objects could be placed
 - All the actions included in object placement, such as: movementation, rotation, placement, placement check, remotion
 - Storage logic
 - Dinossaurs blocks, showing only fossil parts that the player had found
 - NPC visitors lifecycle, with navigation inside the museum and animations

**Museum Upgrades**
 - Expanding the museum with level and currency
 - Changing the grid space and transfering item data from one to another
 - Changing the visuals and navmesh in each room
 - Loading/unloading rooms as you change between them

**Expedition Selection Screen**
 - Handle many UI elements on this screen, along with logic
 - A horizontal scroll list of the expedition sites
 - A free scroll of the map to show each expedition's location
 - Logic of showing data on each site, and its states (Locked, Purchase and Open) 

---

### LVSIM

[Video](https://drive.google.com/file/d/1xo6MqUfXaP9YXKHXBhJHaPWYLVtsZfMZ/preview)

**Tech**: Unity / C# / Photon / PlayFab / PC / Mobile

**Duration**: 1.5 years (2022-2023)

**Team**: 3 to 8 members, 1 to 2 programmers

#### Description:

LVSIM is a multiplayer Hospital Room simulator for educational purposes. The professor logs in, creates a room and set up a patient, using the control panel. Then the students enter the room and have a interactive medicine class in this room. I was the sole programmer from start to 1.0 launch, and worked with a junior dev on the 1.1 version. 


#### Contribution highlights
I worked as the sole programmer until 1.0 release, so I've made all the logic in the aplication:
- Online entitlement logic using PlayFab, including login and permissions
- Realtime multiplayer logic with Photon, including rooms, roles and players in each room
- Patient state sync between everyone in each room
- Message and voice chat between the players
- Each patient state option in the Control Panel

---

### Mine Quest 2
#### Media:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=S9E4GazGXVM
" target="_blank"><img src="http://img.youtube.com/vi/S9E4GazGXVM/0.jpg" 
alt="Slink & Snatch Demo" width="240" height="180" border="10" /></a>


#### Description:

Mine Quest 2 is a Mining Exploration RPG mobile game

**Tech**: Custom Engine based on Love2D / Lua / Firebase

**Duration**: 1 month (2017)

**Team**: Alone

**Contribution**: Performance

After a change of components, the mine scene was running very poorly, with frame rate dipping below 1 fps. I was in charge of optimizing this scene:
- My investigation showed that this scene had an average of 600 draw calls, and more than 1400 at its worse.
- My main steps to improve it:
 - I've put all background tiles in a unique atlas tileset
 - I've put all interactable mine objects in another altas
 - I've changed the draw order to avoid breaking batches
 - The battle occurs in a overlay over the mine scene. I've taken a snapshot of the scene, add it behind the battle overlay and hid the mine during battle
- After these changes, I could reduce the draw call count to an average of 50, and enable the game to be played at 60 fps in most targeted devices 

---

### Laser Storm Arena
<a href="http://www.youtube.com/watch?feature=player_embedded&v=2vE8beTRD-I
" target="_blank"><img src="http://img.youtube.com/vi/2vE8beTRD-I/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

**Tech**: Unity VR / C# / Photon / VR

**Duration**: 1 year (2019-2020)

**Team**: 3 to 6 members, 2 to 3 programmers

#### Description:

Laser Storm Arena is a VR Shooting Arena game  

#### Contribution highlights

---

### Bid Wars: Pawn Empire:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=a4yDEPUWVrs
" target="_blank"><img src="http://img.youtube.com/vi/a4yDEPUWVrs/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

**Tech**: Custom Engine based on Love2D / Lua / Firebase

**Duration**: 2 year (2017-2018)

**Team**: 8 to 10 members, 3 to 4 programmers

#### Description:
An auction game with a city management side loop

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
