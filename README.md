# Snake-Command
A game in which you control the movements of three different snakes.

class Snake {
  constructor(snakeType) {
    this.pattern = snakeType;
  }
  move(numOfSquares) {
    if(numOfSquares > 0 || numOfSquares < 0) totalDistance = numOfSquares;    
  }
  turn(totalDistance) {  
    if(totalDistance >= 1) console.log(this.pattern, "should go up", totalDistance, "spaces and turn to the back.");
    else if(totalDistance <= -1) console.log(this.pattern, "should go back", Math.abs(totalDistance), "spaces and turn to the front.");
    else console.log(this.pattern, "is stuck.");   
  }
  get numOfSquares() {
    return totalDistance;
  }
} 
let dots = new Snake("Boa");
let diamonds = new Snake("Python");
let stripes = new Snake("Viper");
dots.turn(86);
diamonds.turn(-43);
stripes.turn(0);
