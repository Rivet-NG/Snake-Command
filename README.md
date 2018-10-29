# Snake-Command
A game in which you control the movements of three different snakes.

class Snake {
  constructor(snakeColor) {
    this.color_ = snakeColor;
    this.position_ = 0;
    this.direction_ = "Forward";
  }
  move(numOfSquares) {
    if (this.direction_ == "Forward") this.position_ = this.position_ + numOfSquares;
    else if (this.direction_ == "Backward") this.position_ = this.position_ - numOfSquares;
    }
  turn() { 
    if (this.direction_ == "Forward") this.direction_ = "Backward";
    else this.direction_ = "Forward";
  }
  get position() {
    return this.position_;
  }
}    

let redSnake = new Snake("red");
let yellowSnake = new Snake("yellow");
let greenSnake = new Snake("green");

redSnake.move(78);
redSnake.turn();
redSnake.move(42);
console.log(redSnake.position);

yellowSnake.move(25);
yellowSnake.turn();
yellowSnake.move(56);
console.log(yellowSnake.position);

greenSnake.move(-37);
greenSnake.turn();
greenSnake.move(61);
console.log(greenSnake.position);
