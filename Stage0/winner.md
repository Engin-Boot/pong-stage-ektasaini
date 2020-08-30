# check winner

## Feature

This module will check for the winner after every score update.

## Acceptance Criteria

### Scenario: check winner

  Given the user is playing the pong game.

  When there is an update in the score of any player

  Then this module will check if any player's score
  is equal to 10 and if so it will return the
  winning player's name.
