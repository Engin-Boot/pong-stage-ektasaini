# update the score of the players

## Feature

This module will be responsible for updating the score of the players.

## Acceptance Criteria

### Scenario: ball hits the wall

  Given the user is playing the pong game and
  ball coming towards the player hits the wall
  instead of the paddle

  When the received collision type is bad

  Then this module will increment the score of the opponent by 1.
