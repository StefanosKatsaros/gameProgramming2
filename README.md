Game Programming Second Project

Stefanos Katsaros

youtube link: https://www.youtube.com/watch?v=Cj3CxJIoXvc

The game: The Monkey Slot Machine is a game that uses the logic of a slot machine, but is presented visually in a different more exciting manner. A simple slot machine is usually
comprised of 3 slots that rotate and stop at a certain time. If the images on the slot machine match there is a reward, otherwise the player has lost. My game contains
the same logic, but takes place in a stunning environment with monkeys taking the place of the "slots", and colored lights and monkeys taking the place of the images, and the magic white orb replacing the lever.
In this game, you (the player) plays the role of a moving ball that destroys a magic white orb, triggering the 3 monkey slots to start rotating. After 15 second the orb will reapper and the user may strike down the
orb in order to reinitialise the rotation of the monkey slots. There are four colors that take the place of slot images, and at a random time variable of 10 to 12 seconds 3 monkeys which have a color of their own will one another.
If their colors match the player will be victorious and will earn a point. The player can follow this process  for as long as he would like, thus adding up his score. 
Additional game content has been added to fulfil the requirements of the project and therefore there is a starting animation, where the magical orb is first covered by a huge rock, which slowly flies up to the sky and unravelling
the magic white orb. Furthermore a short metagame has been added so the player can play another game while waiting for the slot spins to be completed. When the monkey slots start rotating a large gold monkey head appears rotating around the
game environment, and if the player manages to strike it down before the slot spins are complete he will gain 3 extra points. Finally it is worth mentioning that additional
to the score points the player earns, he also earns small gold monkey head statues that fall from the sky near tha magic white orb area. There is a text on the top
left of the screen describing the game activity the player may follow, while there is also text on the top center of the screen showing the current score.

Behind the scene: I will now present a short description of the methodology I followed along with a description of my code logic. The game is written in unity and all code is in C#.
It works with unity physics and collisions determine the game. We use the rotating ball which is based on simple movement and the camera attached to it follows it using its offset which forbits it from rotating along with the ball.
The magic white orb checks for collisions and if one occurs it is destroyed and initialises the monkeys to rotate. The orn is initisialised in the same position 15 seconds
after. The monkey orbs are also based on collisions. There is an invisible cube that stops the monkey heads at a position that will allow 3 of them to look at one another. This box trigger loses its box collider when the magic
white orb is destroyed and after 10-22 seconds regains its box collider feature and collides with the monkey at its given location. All monkeys have a certain color attached to them, and depending on which one collapses with the
box trigger a different light appears. Therefore if the purple monkey collides, then a purple light will appear. If all 3 monkeys have the same light color then the player earns
a point. When he earns a point a score point is added and a gold monkey head medallion falls from the sky to the center of the game. For the extras of the project, the starting rock that floats up in the sky has an animation attached to it
which is initialised automatically when the game starts and is shortly after destroyed. For the metagame, the giant gold monkey that appears is dependant on the rotating monkey slots. While they are all true the giant monkey is visible, when they are
false it is not. When an object (which will be the player) collides with it, it is destroyed and the player earns 3 points and 3 gold medallions drop from the sky. The giant monkey head moves fast and is therefore tricky to destroy.

Environment: There is not much to say about the environment, but the terrain was built in unity, models were created in blender and the atmoshpere and water in the game were created using unity's recourses.
As for the monkey slots, which are 3 large rocks and 4 monkeys rotating around each one, it has been coded in a way that the large rock is the center that the colored monkey heads rotate around in the air.
A small particle system was created to give the magic white orb a more mysterious and cool look, while lighting used up simple coloured point lights under the 3 large rocks. 
