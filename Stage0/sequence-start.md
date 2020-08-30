# Interaction Sequences

## sequenceDiagram

 sequenceDiagram
 home page->> signin/login: signin or login
 signin/login->>+buy and pay: buy new board,paddle,ball
 signin/login->>+difficulty level: choose any difficulty level
 signin/login->>+board settings :change color of board, ball,paddle
 signin/login->>+choose player : choose your opponent

 choose player->>+random person: choose any random person to play with
 choose player->>+game code: share game code with friend
 random person ->>+start game : start game

loop Every 10 ms

 game code ->>+start game : start game (ball starts moving)
 start game-->> exit : exit in middle of the game
 start game ->>+paddle movement : can move paddle up and down
 paddle movement->>+collision :tells type of collision

 collision->>+ball direction: collision b/w paddle and ball
 collision->>+ball position reset : collision b/w wall and ball
 ball direction -->>-paddle movement: ball moving towards the opponent
 ball position reset ->> score calculate : increment opponent score by 1
 score calculate->+winner: check if any player won
 winner -->>-paddle movement : if noone won

end

 winner-> exit : if any player won
