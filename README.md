# Snake-Command
A game in which you control the movements of three different snakes.

class Snake {
  constructor(snakeType) {
    this.firstSquare = 0;
    this.pattern = snakeType;
  }
  move(moveNumber) {
    if(moveNumber > this.firstSquare) console.log(this.pattern, "should move up", moveNumber, "spaces");
    else if(moveNumber < this.firstSquare) console.log(this.pattern, "should move back", Math.abs(moveNumber), "spaces");
    else console.log(this.pattern, "is stuck");  
  }
  turn(turnNumber) {
    if(turnNumber > this.firstSquare) console.log("and then turn to the back.");
    else if(turnNumber < this.firstSquare) console.log("and then turn to the front.");
    else console.log("and should just face backwards.");
  }
    get () {
    return console.log(Snake.turn, Snake.move); 
  }
} 
let dots = new Snake("Boa");
let diamonds = new Snake("Python");
let stripes = new Snake("Viper");
console.log(dots.move(86), dots.turn(86));
console.log(diamonds.move(-43), diamonds.turn(-43));
console.log(stripes.move(0), stripes.turn(0));
