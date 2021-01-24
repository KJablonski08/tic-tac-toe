# Tic Tac Toe in Ruby

## Overview

A two-player CLI version of Tic-Tac-Toe

## Objectives

1.  Build and use helper methods within the Tic Tac Toe application
2.  Write a method that is responsible for the game loop in Tic Tac Toe
3.  Code the main executable file that will run the game in the CLI

#### Gemfile

This file sets up gems for the project and can mostly be ignored. Make sure to run `bundle` before starting this project so that you have all the required gems.

#### `bin/tictactoe`

This is our main executable and will be how we run our game.

#### `lib/tic_tac_toe.rb`

All of our game methods will be coded here.

### Game Conventions

A Tic Tac Toe board is represented using an array of `" "` strings.
This board is passed to every method as an argument so the helper methods can interact with or introspect on the board.

The game gets the user input via `gets` and a player will choose a position on the board by entering 1-9. The program will fill out the appropriate
position on the board with the player's token. The term 'position' will refer to the spot on the board as the player sees it (1-9).

At every turn, the application will check to see if there is a winner. If there is a winner, the game will congratulate them. If there is a tie, the game will inform the players.

## Instructions

#### `#display_board`

A method that prints the current board representation based on the
`board` argument passed to the method.

An empty board would be:

```ruby
board = [" "," "," "," "," "," "," "," "," "]
display_board(board)
```

Outputting:

```
   |   |
-----------
   |   |
-----------
   |   |
```

A board with an "X" in the middle:

```ruby
board = [" ", " ", " ", " ", "X", " ", " ", " ", " "]
display_board(board)
```

Outputting:

```
   |   |
-----------
   | X |
-----------
   |   |
```

### The CLI: `bin/tictactoe`

1.  Greet the players with "Welcome to Tic Tac Toe!"
2.  Define a `board` array.
3.  Display the starting board.
4.  Begin the game by calling `#play`.

## Play Your Game

Once you get all the tests to pass, play your game!

```
$ bin/tictactoe
```
