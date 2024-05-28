# Restaurant Code Test

## Criteria Evaluation

1.	Object Oriented Programming - (Wikipedia](https://en.wikipedia.org/wiki/Object-oriented_programming)
2.	Respect SOLID Principles - [Wikipedia](https://en.wikipedia.org/wiki/SOLID)
3.	Testability - [Wikipedia](https://en.wikipedia.org/wiki/Unit_testing)

## Test Requirements

1.	This application should runo commands via terminal (console)
2.	must have unit tests (evidence the sample input/output).	
3.	Push your code to GitHub repo, and create a simple github action to build and test

## App Rules

1.	You must enter time of day as `morning` or `night`
2.	You must enter a comma delimited list of dish types with at least one selection
3.	The output must print food in the following order: entrée, side, drink, dessert
4.	There is no dessert for `morning` meals
5.	Input is not case sensitive
6.	If invalid selection is encountered, display valid selections up to the error, then print error
7.	In the `morning`, you can order multiple cups of coffee
8.	At `night`, you can have multiple orders of potatoes
9.	Except for the above rules, you can only order 1 of each dish type

## Dishes Table

| Dish Type   | morning          | night  |
| ----------- | ---------------- | ------ |
| 1 (entrée)  | eggs             | steak  |
| 2 (side)    | Toast            | potato |
| 3 (drink)   | coffee           | wine   |
| 4 (dessert) | _Not Applicable_ | cake   |

## Input and Output samples:

- Input: morning, 1, 2, 3    	Output: eggs, toast, coffee
- Input: morning, 2, 1, 3 	Output: eggs, toast, coffee
- Input: morning, 1, 2, 3, 4	Output: eggs, toast, coffee, error
- Input: morning, 1, 2, 3, 3, 3	Output: eggs, toast, coffee(x3)
- Input: night, 1, 2, 3, 4	Output:  steak, potato, wine, cake
- Input: night, 1, 2, 2, 4	Output steak, potato(x2), cake
- Input: night, 1, 2, 3, 5	Output:  steak, potato, wine, error
- Input: night, 1, 1, 2, 3, 5	Output:  steak, error
