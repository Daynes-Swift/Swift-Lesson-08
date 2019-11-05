# Lesson 08 - Constants and Variables

# Exercise: Making a Shopping List
The constants below represent some of the things you might want to add to a shopping list:

```swift
let eggs = "Eggs"
let milk = "Milk"
let cheese = "Cheese"
let bread = "Bread"
let rice = "Rice"
let newLine = "\n"
```

## Exercise
Create a string variable with an initial value of "". Add each constant item above to the list, one at a time. Add a newLine in between each item. Remember you can join two strings using the + operator.

```swift
var shoppingList = ""
shoppingList += eggs
shoppingList += newLine
shoppingList += milk
shoppingList += newLine
shoppingList += cheese
shoppingList += newLine
shoppingList += bread
shoppingList += newLine
shoppingList += rice
```
# Exercise: 501

You may know the popular darts game called 501. Players start with a score of 501, and have to work down to zero. Here are the rules:
* Each player plays a “round” where they throw three darts at a board.
* Each throw can score between 1 and 20 points, which may be doubled or tripled depending where it hits on the board.
* It is also possible to score 25 for the outer bulls-eye or 50 for the inner bulls-eye.

House rule: At the end of three rounds, whoever is closest to zero without going below zero is the winner.

## Exercises
Imagine you’re a game shark. You want to fool people into thinking you’re terrible at this game, but then come back and beat them in one swoop at the end. Model your game progress using variables.

 Start with a variable set to ```501``` to hold your overall score.
 Create another variable set to ```0``` to hold the score for each round.
 For each throw, update the value of the round score by adding points from the throw.
 At the end of each round, calculate your current overall score by subtracting the round score from it. Assign the new value to your overall score, and re-set the round score to zero.

How slowly can you “improve” your performance without arousing suspicion? 
 
After each round, print some statements that your opponents might make. If you can, use the value of your current score in their statements.

```swift
var overallScore = 501
var roundScore = 0
roundScore += 1
roundScore += 5
roundScore += 10
overallScore -= roundScore
print("Pretty bad round; you're still at \(overallScore)! Haha!")

// Output: Pretty bad round; you're still at 485! Haha!

roundScore = 0
roundScore += 10
roundScore += 20 * 3
roundScore += 25
overallScore -= roundScore
print("You lucked out on that triple. You're catching up with a score of \(overallScore).")

// Output: You lucked out on that triple. You're catching up with a score of 390.

roundScore = 0
roundScore += 20 * 3
roundScore += 20 * 3
roundScore += 20 * 3
overallScore -= roundScore
print("How could you possible get the highest score of \(roundScore) in a single round?! Now you're at \(overallScore).")

// Output: How could you possible get the highest score of 180 in a single round?! Now you're at 210.

roundScore = 0
```
