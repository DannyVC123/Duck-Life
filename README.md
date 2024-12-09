# Duck Life

## Aesthetic Goals:
### Goal 1: Simplicity
**Definition:** The player should feel that the game is easy to pick up and play, with intuitive controls and clear objectives, allowing them to quickly understand how to progress without feeling overwhelmed.

#### Success:
- Players quickly understand what to do and can start engaging with the game immediately.
- The game mechanics are intuitive, allowing players to learn through gameplay rather than relying on lengthy tutorials or detailed instructions.
- Players of all skill levels can enjoy the game without feeling frustrated or overwhelmed.

#### Failure:
- Players express confusion or frequently ask for clarification about how to play.
- Tutorials or instructions feel overly detailed and are skipped or ignored because players struggle to understand how they affect gameplay.
- The game has a steep learning curve that deters casual players.

### Goal 2: Competition
**Definition:** The player should feel a sense of excitement and motivation to outperform other players, making each competition thrilling and engaging.

#### Success:
- Players experience a rush of excitement during competitive moments, such as races or challenges.
- Players are motivated to replay sections to improve their performance and achieve better results.
- Players feel a sense of accomplishment and pride when they surpass their opponents.

#### Failure:
- The competition feels too easy or too hard, leading to boredom or frustration.
- Players feel unmotivated to compete, showing little interest in winning or losing.
- The competition lacks excitement, making races feel repetitive and dull.

## Core Loop:
### Running
- Obstacles spawn and move toward the player.
- The player jumps to avoid the obstacles.
- If successful, another obstacle spawns, increasing in speed or frequency.
- If the player fails to avoid an obstacle, the training ends. The player can then choose to try again for a higher score or move on to the next training event.

### Flying
- Rocks spawn randomly in the top or bottom half of the screen and move toward the player.
- The player flies up or down to avoid the rocks.
- If successful, a new rock spawns with a faster speed.
- If the player fails to avoid a rock, the training ends. The player can then choose to try again for a higher score or move on to the next training event.

### Swimming
- Obstacles spawn and move toward the player.
- The player jumps over or dives down into the water to avoid the obstacles.
- If successful, another obstacle spawns, with a faster speed.
- If an obstacle pushes the player offscreen, the training ends. The player can then choose to try again for a higher score or move on to the next training event.

## Devlog
### Running Training - Nov. 25, 2024
I implemented the basics of the running training section. An obstacle spawns on the right side of the screen and rolls toward the player on the left. The player must press the up arrow key to jump over the obstacle. If successful, a new obstacle spawns on the right with a faster speed. The training continues until the player hits an obstacle.

### Moving Clouds - Nov. 25, 2024
In each training section, the player remains stationary while the objects on screen scroll left, creating the illusion that the player is moving forward. To enhance realism, I added clouds moving left to further emphasize the player's motion.

### Flying Training - Nov. 26, 2024
I implemented the basics of the flying training section. The player uses the up and down arrow keys to control the duck's movement in the air. A large rock spawns on the right side of the screen, either in the top or bottom half. The player must maneuver the duck to avoid the rock. If successful, a new rock spawns with a faster speed. The training continues until the player hits a rock or the water below.

### Flying Training Ramp Animation - Nov. 27, 2024
In the original game, the flying training begins with the duck sliding down a ramp and being launched into the air. I recreated this animation in Unity using rigid bodies and Unity's built-in physics. This took longer than expected due to the duck frequently rolling into the wrong position, but it now behaves as intended.

### Starting and Game Over UIs - Nov. 27, 2024
I added two UIs for each training section: the starting UI and the game over UI. The starting UI states the controls for the training section, and the player presses the space bar to begin. The game over UI appears when the player loses, based on the training section's loss condition. It then gives players the option to replay the section for a higher score or continue to the next training section.

### Swimming Training - Dec. 05, 2024
I implemented the basics of the swimming training section. The player uses the up arrow to jump and the down arrow to dive underwater. Various obstacles, such as sailboats, icebergs, and rock pillars, spawn on the right side of the screen and move toward the player. Since the obstacles are larger than the other two sections, the player can touch obstacles but loses if they are pushed offscreen. If the player successfully stays onscreen after the obstacle moves offscreen, a new obstacle spawns at a faster speed. The training continues until the player is pushed offscreen.

### Game Over Screen - Dec. 08, 2024
I originally planned to implement a short race at the end of the three training sessions, where the player would compete against NPC ducks. The race would incorporate different sections that test the three skills—running, flying, and swimming—offering a fun and competitive payoff that showcases the results of their training. However, due to time constraints, I chose to create a simple game over screen instead which displays the player's score from each training session.

## Gameplay Instructions
There are three training sections: running, flying, and swimming. In each section, avoid obstacles and survive as long as possible to earn a higher score. If you hit an obstacle or go offscreen, you can either retry the section for a higher score or move on to the next one. The game concludes by displaying your scores from each training section.



