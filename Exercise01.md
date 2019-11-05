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