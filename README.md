# Control Flow Lab

## Instructions for lab submission

1. Fork the assignment repo
1. Clone your Fork to your machine
1. Complete the lab
1. Push your changes to your Fork
1. Submit a Pull Request back to the assignment repo
1. Paste a link to of your Fork on Canvas and submit

## Question 1

What will be printed when the code below is run?  Select all that apply.

```swift
let conditionOne = !(4 < 5) || !(3 > 8)
let conditionTwo = !(!true)

if conditionOne {
 print("A")
} else if conditionTwo {
 print("B")
}
if conditionTwo {
 print("C")
}
print("D")

            ///// Answer: A, C, D
            
```

***
## Question 2

What will the code block below print?  Select all that apply:

```swift
let appInfo = (name: "myCoolApp", version: 0.4)
switch appInfo {
 case (_, 0.0..<1.0):
 print("\(appInfo.0) hasn't released yet")
 case ("myCoolApp", _):
 print("Thanks for looking at myCoolApp!")
 default:
 print("I'm not quite sure what you are looking at")
}

            ///// Answer: myCoolApp hasn't released yet 
                          Thanks for looking at myCoolApp  
```
***
## Question 3

What will be printed to the console when the code below is run?  Select all that apply.

```swift
let x: Int = 4
switch x {
case 0..<4:
 print("A")
case 5..<10:
 print("B")
case is Double:
 print("C")
default:
 print("D")
}
            ///// Answer: D
```
***
## Question 4

What are the errors in the code below for the switch statement? Select all that apply.

```swift
let candyType : String = "skittles"

switch candyType {
case "mAndM":
 print("Melts in your mouth, not in your hand")
case "skittles":
 print("Taste the rainbow")
case "snickers":
 print("Hungry? Grab a Snickers")
}

            ///// Answer: No parentheses around                     the conditions
                          No default case in the switch statement
```
***
## Question 5

Given the current weather conditions (rain, sunny, snow), use a switch statement to print an appropriate message to the user

```swift
let currentWeather = "rain"

            ////Answer:
switch currentWeather {
case: "Rain"
print(" Make Sure You Have Your Umbrella!")
}
default: 
print(" This weather is unpredictable sometimes")

```

***
## Question 6

Given the first name and last name of a Fellow, declare `fullName` variable and use string interpolation to concatenate the Fellow's full name and print to the console e.g The Fellow's full name is John Appleseed

```swift
let firstName = "John"
let lastName = "Appleseed"

            /////Answer:
let fullName = firstName + " " + lastName
print("The Fellow's full name is \(fullName)")



```

***

## Question 7

Convert the if/else statement below into a switch statement.

```swift


if temperatureInFahrenheit <= 40 {
 print("It's cold out.")
} else if temperatureInFahrenheit >= 85 {
 print("It's really warm.")
} else {
 print("Weather is moderate.")
}

var temperatureInFahrenheit = 60
            
            /////Answer:
switch temperatureInFahrenheit {
case (0...41):
    print("It's Cold out")
case (85...1000):
    print("It's really warm")
default:
    print("Weather is Modedrate")
}

//Re-written statement here

```

***

## Question 8

Complete the following code so that "You win!" is printed.

```swift

var chances = 22
if chances % 2 == 0  {
 print("You win!")
}
else {
 print("You lose!")
}

var chances2 = 23

if chances2 % 2 == 1 {
 print("You win!")
}
else {
 print("You lose!")
}

```
***

## Question 9

Given a variable called numberOfSides, write code using a switch so that it prints out the name of the shape. Account for shapes with 3 to 10 sides and print an error message if out of range.

var numberOfSides = 6

```swift
var numberOfSides = 9

switch numberOfSides {
case (3):
    print("Triangle")
case (4):
    print("Square")
case (5):
    print("Pentagon")
case (6):
    print("Hexagon")
case (7):
    print("Heptagon")
case (8):
    print("Octogon")
case (9):
    print("Nonagon")
case(10):
    print("Decagon")
default:
    print("ERROR")
    
}

```
***

## Question 10

Create a switch statement that will convert a number grade into a letter grade as shown below:

```swift
let grade = 60

switch grade {
    
case 100:
    print("A+")
case 90..<100:
    print("A")
case 80..<90:
    print("B")
case 70..<80:
    print("C")
case 65..<70:
    print("D")
case 0..<65:
    print("F")
default:
    print("Your Grade is so special that there is no letter to represent it")
}```
***
```
## Question 11

What is wrong with the block of code below?  Correct it so it behaves as expected.

```swift
/////Answer:
let firstName = "Peter"
var lastName: String = ""
if firstName == "Peter" {
 lastName = "Gabriel"
} else if firstName == "Phil" {
lastName = "Collins"
}
let fullName = firstName + " " + lastName


```
***

## Question 12

Write an if statement that prints out what decade of life someone is in (e.g "You are in your twenties). Then, write it as a switch statement.

```swift
            /////Answer:
let nameAndBirthYear = ("Ant" , 1978)

if 1960..<1970 ~= nameAndBirthYear.1 {
    print("\(nameAndBirthYear.0) is in his 50's")
} else if 1970..<1980 ~= nameAndBirthYear.1 {
        print("\(nameAndBirthYear.0) is in his 40's")
} else if 1980..<1990 ~= nameAndBirthYear.1 {
    print("\(nameAndBirthYear.0) is in his 30's")
} else if 1990..<2000 ~= nameAndBirthYear.1 {
    print("\(nameAndBirthYear.0) in in his 20's")
} else {
print("sorry")
}

let nameAndBirthYear = ("Ant" , 1978)

switch nameAndBirthYear.1 {
case 1960..<1970:
    print("\(nameAndBirthYear.0) is in is 50's")
case 1970..<1980:
    print("\(nameAndBirthYear.0) is in his 40's")
    case 1980..<1990:
    print("\(nameAndBirthYear.0) is in his 30's")
    case 1980..<1990:
    print("\(nameAndBirthYear.0) is in his 20's")
default:
        print("")
}
```
***


## Question 13

Consider the below switch statement. What should your system currently print?

```swift
let number = 42

switch number {
case 365:
 print("Days in year")
case 1024:
 print("Bytes in a Kilobyte")
case 0:
 print("Where arrays start")
case 42:
 print("The answer to life, the universe and everything")
default:
 print("Some uninteresting number")
 
 ////Answer: The answer to life, the universe and everything
```
What happens when you change number to:

-a. 365? - Days in Year

-b. 1024? - Bytes in a Kilobyte

-c. 65? - Some uninteresting number


What happens when you remove the default clause?

the code will not compile. it needs the default. 

***


## Question 14

Consider the variable below called population and the if-condition.

a. Add an else-if-condition that states if population is less than 10000 but greater than 5000, then message changes to say it's "a medium size town".

b. Add an else-condition where message changes to say it's a mid-size town.

c. Convert your final if-else statement to a switch statement.

```swift
var population: Int = 100000
var message = String()

if population > 10000 {
 message = "\(population) is a large town"
 } 
 
        ////Answer:
var population: Int = 70000
var message = String()

        if population > 100000 {
            message = "\(population) is a large town"
        } else if population < 100000 && population > 50000 {
           message = "\(population) is a medium size town"
        } else {
           message = "\(population) is a small - size town"
        }
        print(message)
        ...................................................
        switch population {
        case 100000...:
            message = "\(population) is a large town"
        case 50000..<100000:
            message = "\(population) is a medium size town"
        case 1..<50000:
            message = "\(population) is a small size town"
        default:
            print("Ya too big or too small.. sorry")
        }
        
```
***

## Question 15

Complete the code below so that it prints out and tells the user if the sum of the two numbers in the tuple is at least 15.

a. Using a conditional

            ////Answer:
let myTuple: (Int, Int) = (5, 10)

if myTuple.0 + myTuple.1 == 15 {
    print("Yup! It's 15!")
}else {
    print("Nope sorry! try again")
}

b. Using a switch statement

```swift
let myTuple: (Int, Int) = (5, 10)


```
***
