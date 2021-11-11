# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## To run the app

```
git clone git@github.com:sayandip18/2048.git
cd 2048
npm install
npm run start
```
## To play

The player can play along by pressing the arrow keys

## Logic

The functions used in the project are explained below

1. Initializing the grid with zeros and two randomly placed numbers which are either 2 or 4.
2. Swiping left, right, up and down which takes all the contents of the grid and move them in the respective directions.
3. Checking if the game is over or not. If all the squares are filled and no move can be made, then the game is over
4. Reset function to start the game again.


### Swipe function

Let us dive deep into the swipe left function. Let us imagine a single row for the operation. The same operation is repeated
for all the rows.

We take two pointers, `slow` and `fast` initialized to 0 and 1 positions respectively. We perform
a series of checks while iterating to implement the algorithm.

### 8x8 board

In order to make a 8x8 game, we need to modify `data`, `addNumber()` and all the `swipe*()` functions accordingly.
