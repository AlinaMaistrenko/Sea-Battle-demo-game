# Sea-Battle-demo-game
A demo game in python
<img src="https://github.com/AlinaMaistrenko/Sea-Battle-demo-game/blob/main/screenshots/main.jpg">

More screenshots [here](https://github.com/AlinaMaistrenko/Sea-Battle-demo-game/tree/main/screenshots).

## Requirements: 
  1. Python 3.+.
  2. PNG viewing in the GUI: Python Imaging Library (**PIL**) *ImageTk*. 
    Can be installed using command `sudo apt-get install python-imaging-tk` for linux. 
    It is optional. If you don't want the cool image background as shown above, you can skip this.

## Setup instructions:
  1. Download or import the project.
  2. Open `main.py` file (if you don't have installed **PIL** you should open `main_without_image.py`).
  3. Run and enjoy the game.
  
## Creating a custom bot:
  If someone wants to create own bot and play agains it, it is possible to create and integrate a custom bot.
  Sees the instruction how to do that, below.
      
### Bot class requirements:
  1. It must be a class
  2. It must have a function `say(value: str)` that returns *tuple* of Integers, 
  coordinates of the field where the bot wants to shoot `(x, y)`.
  There, `value` is a string which can be only one of these three values:
      * "**shoot**" - means, the player missed, and bot's turn.
      * "**hit**" - means, bot's previous shoot was successful, but didn't destroy the player's ship complataly.
      * "**destroyed**" - means, bot's previous shoot was successful, and destroyed the player's ship complataly.
  As an example open `bots.py` file, and see the bot ***Fati***.
  
  


