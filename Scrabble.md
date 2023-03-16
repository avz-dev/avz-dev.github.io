---
title: Scrabble
layout: page
filename: Scrabble.md
remote_theme: pages-themes/midnight@v0.2.0
plugins:
- jekyll-remote-theme
--- 

# Scrabble
By Andrew Valdez 

## How to Run
<a href="https://github.com/avz-dev/scrabble/raw/main/scrabble.jar">Scrabble</a> 
`java -jar scrabble.jar`


## How to Play

The player starts the game by either selecting a starting square or selecting `Play` to end their turn.
<img src="https://avz-dev.github.io/resources/starting-tile.png" width="800" height="800">
  
The player may also selet `Shuffle` at any time to randomly rearrange the order of their unplayed tiles.
<img src="https://avz-dev.github.io/resources/shuffle.png" width="800" height="800">

Once a tile is selected, the player must select a direction in which to build the word.
<img src="https://avz-dev.github.io/resources/direction.png" width="800" height="800">

Once a direction is selected, the player may select tiles to add to the board or reset their turn.
<img src="https://avz-dev.github.io/resources/tile-select.png" width="800" height="800">

If at least one tile has been placed, the player may select "Play" to submit the word. 
<img src="https://avz-dev.github.io/resources/first-word.png" width="800" height="800">

If a word is valid, it is played and the computer then plays a word.
<img src="https://avz-dev.github.io/resources/comp-first.png" width="800" height="800">

Invalid words will not be played and the player can either continue adding to the word or reset their turn.
<img src="https://avz-dev.github.io/resources/invalid-word.png" width="800" height="800">

Each word is scored and each word score is added to the total score.
The participant with the highest score is declared the winner at the end of the game.

The game ends when the both solver and player have no valid plays. (Note: player must end their turn)
<img src="https://avz-dev.github.io/resources/end.png" width="800" height="800">


## Classes

### Trie Data Structure
Reads in dictionary and builds trie data structure
### Display
Handles all GUI elements and feeds player input into Player. Alternates turns between players.
### Board
Holds square objects with multiplier information, stores tiles placed on board.
### Tiles
Holds tile data such as letter, points, and blank status.
### Square
Holds board space data such as multipliers, anchor status, and tile.
### Player:
Ability to play word, check word validity, return tiles to rack if invalid. 
Keeps track of overall score and current word score.
### Solver
Plays word with the highest possible score using recursive backtracking.
### Main
Initializes Display and starts game.
