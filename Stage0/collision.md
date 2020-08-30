# Collision

## Feature

This module will be responsible for checking collision
between the four walls, ball and the paddle and thus
returning the type of collision.

## Acceptance Criteria

### Scenario: collision of ball and the paddle

  Given the user is playing the game

  When the ball collides with his paddle

  Then this module will return a "good" collision type.

### Scenario: collision of ball and one of the four walls

  Given the user is playing the game

  When the ball collides with the wall

  Then this module will return a "bad" collision type.
