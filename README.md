# Hi, I'm Guilherme! VR Unity programmer
[LinkedIn](https://www.linkedin.com/in/guilherme-freire-ba8b7717a)

## Software Development in studios:
[Venturion VR](https://en.venturion.com.br/) 2018 - current

[Tapps Games](https://tappsgames.com/) 2015 - 2018

## Project Hightlights (Work in Progress):

### Slink & Snatch
<a href="http://www.youtube.com/watch?feature=player_embedded&v=55Qd2ugDzRI
" target="_blank"><img src="http://img.youtube.com/vi/55Qd2ugDzRI/0.jpg" 
alt="Slink & Snatch Demo" width="240" height="180" border="10" /></a>

**Slink & Snatch: Tales of Thievery** is a cartoonish VR Stealth Game, with a Collectathon core loop, targeting Meta Quest 2. This project is the biggest of the company yet, bringing many challenges, from general architecture to optimization. It started in 2022 as a prototype and is currently in development, with a released Demo.

I integrated the programming team with 2 more devs, creating the architecture from the ground up and implementing countless features, such as items, potions, key and locks, powerups, UI.

#### Contribution highlights:
- **Implemented asset streaming to enable a full city to run at 72 fps on Meta Quest 2**. The project was PC targeted from the beginning, but at a given point we decided to port it to the Meta Quest. There was a huge effort to optimize performance, including basic mesh culling to logic culling, simplifying complex models, mesh colliders and nav-meshes. But the biggest challenge was to have a entire open and interconnected city running at 72 fps without visible loadings. I was leading this task and this is achieved dividing the city in many sections, focusing on a limited tri count on each one, and using a neighbour loader strategy. When the Player is in a given Section, only its neighbours are loaded. When changing sections, the new neighbours got loaded and the old one unloaded. It was also needed to use portals to define when the Player was moving between sections, as each area had complex interconnections, and could be inside one another.

- **Implemented Enemy AI** The enemy is a complex structure, it has a state cycle, sensors to find the Player, a Nav Mesh Agent. I implemented a Finite State Machine to deal with its many patroling states, changing between Patrol, Investigate, Chase, Shooting, Searching. I achictecture an interface to deal with its sensors, inclusing Vision, Hearing and Touch, to deliver the complex design interactions needed in the feature.   


### Dino Quest 2:

<a href="http://www.youtube.com/watch?feature=player_embedded&v=gn_dYnYUzTI
" target="_blank"><img src="http://img.youtube.com/vi/gn_dYnYUzTI/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

2020-2022
Dino Quest 2 is a exploration/management mobile game with two main mechanics, going on expeditions to find fossils, and managing the fossils in the Museum. This was my first commercial Unity mobile game, I worked as the lead game programmer from day 1 to 1.0 release, initially with another programmer, but mostly alone. After release, the team increased to 4 programmers.

#### My most notable contributions
- I've made all the logic in the exploration sites:
 - 3D grid where the fossils are placed
 - The logical structure of the entity Fossil, including informations such as size, body part, rarity, 3D bounds
 - The structure of each exploration site, such as size, dinos included, fossil number range, dificulty, terrain block tiles included
 - The placement logic and configuration, from fossils to terrain blocks
- I've made all the logic in the Museum:
 - 2D grid where objects could be placed
 - All the actions included in object placement, such as: movementation, rotation, placement, placement check, remotion
 - Storage logic
 - Dinossaurs blocks, showing only fossil parts that the player had found
 - NPC visitors lifecycle, with navigation inside the museum and animations

### Laser Storm Arena
<a href="http://www.youtube.com/watch?feature=player_embedded&v=2vE8beTRD-I
" target="_blank"><img src="http://img.youtube.com/vi/2vE8beTRD-I/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>

#### Project Description: VR Multiplayer Shooting Arcade
- 1 year project
- Team of 4 to 6 people
- 2019-2020 (8 months)
- Multiplayer
- Location-based

#### Feature highlights:



### Bid Wars: Pawn Empire:
An auction game with a city management side loop

#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=a4yDEPUWVrs
" target="_blank"><img src="http://img.youtube.com/vi/a4yDEPUWVrs/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


### Mine Quest 2
<a href="http://www.youtube.com/watch?feature=player_embedded&v=S9E4GazGXVM
" target="_blank"><img src="http://img.youtube.com/vi/S9E4GazGXVM/0.jpg" 
alt="Slink & Snatch Demo" width="240" height="180" border="10" /></a>

Mine Quest 2 is a Mining Exploration RPG mobile game, made in a custom engine. My contribution:

#### Performance

- After a change of components, the mine scene was running very poorly, with frame rate dipping below 1 fps. I was in charge of optimizing this scene
- My investigation showed that this scene had an average of 600 draw calls, and more than 1400 at its worse.
- My main steps to improve it:
 - I've put all background tiles in a unique atlas tileset
 - I've put all interactable mine objects in another altas
 - I've changed the draw order to avoid breaking batches
 - The battle occurs in a overlay over the mine scene. I've taken a snapshot of the scene, add it behind the battle overlay and hid the mine during battle
- After these changes, I could reduce the draw call count to an average of 50, and enable the game to be played at 60 fps in most targeted devices 


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
