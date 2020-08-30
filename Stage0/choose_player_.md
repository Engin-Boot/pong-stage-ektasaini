# Choose player

## Feature

This module will be responsible for helping the user choose his player for the game.

## Acceptance Criteria

### Scenario: play with a friend

  Given the user wants to play the game with one of his friend
  and sends him the game code

  When the friend will join the game by entering the code in his device

  Then this module will set the friend as the second player.

### Scenario: play with a random person

  Given the pong game is open and user wants to play but does not have any partner

  When the user presses "play with random person" button

  Then this module will automatically choose a player from all the available
  online people who are also searching for a second player.
