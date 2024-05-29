# Hi, I'm Guilherme! VR Unity programmer
## Software Development in studios:
[Venturion VR](https://en.venturion.com.br/) 2018 - current
[Tapps Games](https://tappsgames.com/) 2015 - 2018

### Slink & Snatch
#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=55Qd2ugDzRI
" target="_blank"><img src="http://img.youtube.com/vi/55Qd2ugDzRI/0.jpg" 
alt="Slink & Snatch Demo" width="240" height="180" border="10" /></a>

**Slink & Snatch: Tales of Thievery** is a cartoonish VR Stealth Game, with a Collectathon gameplay, such as Sly Cooper and Banjo-Kazooie, targeting Meta Quest 2. This project was a huge challenge for its size and complexity, as the biggest game of the company yet. It started in 2022 as a prototype and is currently in development, with a released Demo.

I integrated the programming team with 2 more devs, creating the architecture from the ground up and implementing countless features, such as items, potions, key and locks, powerups, UI.

#### Contribution highlights:
- **Implemented asset streaming to enable a full city to run at 72 fps on Meta Quest 2**. The project was PC targeted from the beginning, but at a given point we decided to port it to the Meta Quest. There was a huge effort to optimize performance, including basic mesh culling to logic culling, simplifying complex models, mesh colliders and nav-meshes. But the biggest challenge was to have a entire open and interconnected city running at 72 fps without visible loadings. I was leading this task and this is achieved dividing the city in many sections, focusing on a limited tri count on each one, and using a neighbour loader strategy. When the Player is in a given Section, only its neighbours are loaded. When changing sections, the new neighbours got loaded and the old one unloaded. It was also needed to use portals to define when the Player was moving between sections, as each area had complex interconnections, and could be inside one another.

- **Implemented Enemy AI** The enemy is a complex structure, it has a state cycle, sensors to find the Player, a Nav Mesh Agent. I implemented a Finite State Machine to deal with its many patroling states, changing between Patrol, Investigate, Chase, Shooting, Searching. I achictecture an interface to deal with its sensors, inclusing Vision, Hearing and Touch, to deliver the complex design interactions needed in the feature.   



### Laser Storm Arena
#### Project Description: VR Multiplayer Shooting Arcade
- 1 year project
- Team of 4 to 6 people
- Multiplayer
- Location-based

#### Feature highlights:


#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=2vE8beTRD-I
" target="_blank"><img src="http://img.youtube.com/vi/2vE8beTRD-I/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


<h3>Dino Quest 2:</h3>


#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=gn_dYnYUzTI
" target="_blank"><img src="http://img.youtube.com/vi/gn_dYnYUzTI/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


<h3>Bid Wars: Pawn Empire:</h3>


#### Trailer:
<a href="http://www.youtube.com/watch?feature=player_embedded&v=a4yDEPUWVrs
" target="_blank"><img src="http://img.youtube.com/vi/a4yDEPUWVrs/0.jpg" 
alt="IMAGE ALT TEXT HERE" width="240" height="180" border="10" /></a>


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
