# Litter-Monster-Game
<h3>Initial thoughts</h3>
<p>
Create a cute interactive game, which is like flappy bird and use distance sensor to control it. The character of the game is a monster, and players will use sensor to control its position to avoid bombs and eating planets.
</p>
<h3>Modification</h3>
<p>After research we found there were already lots of sensor-control games online, so we change our idea a little bit. The monster will be able to shoot fireballs to eliminate the planets. If the monster is hit by the planet, game will be over. Instead of using distance sensor, we used makey makey to control the monster’s position and shoot fireballs.  We made a gamepad and put makey makey board inside, selected soft sweets as buttons to control position.
</P>
<h3>Coding</h3>
<p>We are using Creative JS library:ZIM to create game interface.
</p>
<h3>Material</h3>
<p>Makey makey board, carton, tape, soft sweets, paper, water color pen.
</P>

<h3>Game(Coding part)</h3>
<ol>
<li>Create a scrolling background</li>
<li>Put the monster on the stage</li>
<li>Add keyboard functions to control the monster’s position by press left, up, right, down
</li>
<li>Put planets on the stage, use setTimeout and move function to make the planet move from right side and use zim.rand to randomly change the planets
</li>
<li>Add fireball and use move function to let the monster shoot the fireballs
</li>
<li>Add keyboard function to the fireball so that users can press space to shoot the ball
</li>
<li>Make two hitTest, one for removing planets when they are hit by the ball, and another for game over when the monster is hit by the planet
</li>
<li>Add a score panel and link it to hitTest, when monster eliminate a planet the score will add up
</li>
<li>Add music to the game and link the game to the game over page.
</li>
</ol>
<h3>Stumbles
Keyboard function</h3>
<p>When we add keyboard function to control the monster, we ran into a problem which is if the user hold the key the monster should constantly move but it turns out it will always pause a second after the first move and then continually move. So something went wrong with the addEventListener. We googled it and solve this problem by set the keyboard function false at first and make it true after the user press the key. The function is always on, but it will only be active when the key is being pressed. So it won’t take extra time to start the function over and over again.
</P>
<h3>controller</h3>
<p>After finishing the coding part, we discussed about what kind of materials should we use to connect to the Makey makey board. We finally decided to use soft sweets.

Firstly, we find a suitable box to as a container, and we made a shape like a small paw control the monster’s position by press left, up, right, down, a fireball shape control the monster shoot the fireballs.

Then, we made it attached to the box surface, and drill holes in the box surfaces so that wires can get through, and in the end we put soft sweets fixed on the top. 

When we put the candy and board together, no matter how hard we press the soft sweets, it does not work, and little monster did not move on the screen. 

Then, we found the problem, which is we forget to connect the ground wire to the player. So we drilled another hole, let the ground wire connected to the candy in the right position. Player can press the soft sweets when they hold the controller. 

Finally, we put the makey makey board into the box and finish the controller.</P>
