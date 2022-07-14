**This is the game of Dominoes written by Todd Sipe for CS 351 UNM.**

Console game information is first, then GUI information at the bottom.

To start playing, run the program from the main method in
ConsoleGame.DominoGame.java.

**RULES:** Each player in this game gets a hand of seven dominoes initially
dealt to them from the common stack of dominoes henceforth referred to
as the Boneyard.

Each player may only play one domino to the battlefield per turn.
In order to do so, the player must match a number on a domino in hand to one
of the numbers on the left or right edge of the Battlefield. The domino may be
flipped, and the blanks (or zeroes) are wild and can be matched to any
number. If the player cannot play a domino, then the player must take one
from the Boneyard one at a time until a domino can be played. When one player
plays a domino to the Battlefield the turn is passed to another player.

**VICTORY CONDITIONS:** Once a player plays the last domino in hand, if the
Boneyard is empty, this player wins the game.

**HOW TO PLAY:** There will be a series of questions proposed to the user in the
terminal.
The first question determines which action the user will take from:

- [p] Play
- [t] Take
- [q] Quit.

If the player decides to Quit, the program terminates. If the player decides to
Take, the user takes a domino from the Boneyard, and then the player is
presented with these three options again, until Play is selected. Once Play is
selected, the player is then prompted with the next question.
The second question determines which domino from the player's hand will
be played to the Battlefield. Every turn the hand is shown to the user, and
the user selects one by typing in a number corresponding to the proper
domino, starting from 0 on the left, ascending to the right.

0, 1, 2, 3, ...

The third question determines whether the user would like to flip the
selected domino before it gets played to the battlefield or not.
(y/n)

The fourth and final question determines whether the player wants to play
the selected domino on the left or right side of the Battlefield.
(l/r)

The turn is then passed to the computer, which takes similar actions as the player,
and then passed back again to the player. This process repeats until there is a victor,
at which time the program terminates.

**TO PLAY THE GUI GAME:**
The gui plays very similarly to the console version. Player must select a domino to play by filling in the correct index number into the text field. Then the player can play left, play right, or flip this domino.

To draw a bone from the boneyard, the player hits the button to "Take One From Boneyard".

I used an extra day for this project, it was a struggle to convert the console to gui. I ran through multiple different iterations of how to approach this, and settled on a very messy way to do so. Most of my logic is within buttons, and I dislike this greatly, but felt the pressure to get something that worked done, so that I could turn a functional program in.

The error handling is not great, yet another thing I would have liked to spend time on had I not spent so much time working out kinks and figuring out how to approach refactoring so much.