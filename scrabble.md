---
title: Scrabble
name: Andrew Valdez
description: By Andrew Valdez
layout: default
filename: scrabble.md
--- 
## Desctiption
A game of Scrabble against an algorithm that utilizes a trie data structure to generate the highest possible scoring word given a set of tiles and a configuration of tiles on the board.

## How to Play

The player starts the game by either selecting a starting square or selecting `Play` to end their turn.
<img src="https://avz-dev.github.io/resources/starting-tile.png">
  
The player may also selet `Shuffle` at any time to randomly rearrange the order of their unplayed tiles.
<img src="https://avz-dev.github.io/resources/shuffle.png">

Once a tile is selected, the player must select a direction in which to build the word.
<img src="https://avz-dev.github.io/resources/direction.png">

Once a direction is selected, the player may select tiles to add to the board or reset their turn.
<img src="https://avz-dev.github.io/resources/tile-select.png">

If at least one tile has been placed, the player may select "Play" to submit the word. 
<img src="https://avz-dev.github.io/resources/first-word.png">

If a word is valid, it is played and the computer then plays a word.
<img src="https://avz-dev.github.io/resources/comp-first.png">

Invalid words will not be played and the player can either continue adding to the word or reset their turn.
<img src="https://avz-dev.github.io/resources/invalid-word.png">

Each word is scored and each word score is added to the total score.
The participant with the highest score is declared the winner at the end of the game.

The game ends when the both solver and player have no valid plays. (Note: player must end their turn)
<img src="https://avz-dev.github.io/resources/end.png">

<a href="https://github.com/avz-dev/scrabble">GitHub Repository.</a> 
