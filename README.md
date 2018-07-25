Agar.io Clone
=============

**This is a clone of [huytd's agar.io server clone](https://github.com/huytd/agar.io-clone) with bug fixes and better logic:
'A simple but powerful Agar.IO clone built with socket.IO and HTML5 canvas on top of NodeJS.'

#### Game Basics
- Move your mouse around the screen to move your cell.
- Eat food and other players in order to grow your character (food respawns every time a player eats it).
- A player's **mass** is the number of food particles eaten.
- **Objective**: Try to get as big as possible and eat other players.

#### Gameplay Rules
- Players who haven't eaten yet cannot be eaten as a sort of "grace" period. This invincibility fades once they gain mass.
- Everytime a player joins the game, **3** food particles will spawn.
- Everytime a food particle is eaten by a player, **1** new food particle will respawn.
- The more food you eat, the slower you move to make the game fairer for all.

---

## Latest Changes
- Login doesn't crash on guessing incorrect password
- The game won't crash when people split

---

#### Requirements
To run / install this game, you'll need: 
- NodeJS with NPM installed.
- socket.IO.
- Express.


#### Installing & Setup
This command will automatically download and install all required files:

```
wget https://aspriddell.github.io/jel.ly/installer-src/install_server_reverseproxy.sh && sudo bash install_server_reverseproxy.sh
```

#### Running the Server
After downloading all the dependencies, you can run the server with the following command:

```
cd  && sudo startserver.sh
```

The game will then be accessible at `http://localhost:3000` or the respective server installed on. The default port is `3000`, however this can be changed in config. To kill the server, turn it off or press Ctrl+Z on the window

If you are on the terminal window, but is not the screen then run:

```screen -r #reattach the screen to the SSH console```

## License
>You can check out the full license [here](https://github.com/aspriddell/jel.ly/blob/master/LICENSE).

This project is licensed under the terms of the **MIT** license.
