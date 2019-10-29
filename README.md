# Optionals lab

Fork and clone this repo. On your fork, answer and commit the follow questions. When you are finished, submit the link to your repo on Canvas.


## Question 1

a. Given the variable `userNameOne` below, print *"The username is Test User"*.  Use *Optional Binding* (`if let`) to print the name.

```swift
var userNameOne: String? = "Test User"
if let userNameOne = userNameOne {
print("The username is \(validUsername)")
} else {
print("no username")
}
```

b. Given the variable `userNameTwo` below, print *"The username is undefined"*.  Use the *nil coalescing operator* (`??`).

```swift
var userNameTwo: String? = nil

```
```
let validUserNameTwo = userNameTwo ?? "Undefined"
print("the username is \(validUserNameTwo)")

```
## Question 2

a. Given the variables `rectOneWidth` and `rectOneHeight` below, print "The area of rectOne is 50".  Use *Optional Binding* (`if let`) to print the area.

```swift
var rectOneWidth: Double? = 5
var rectOneHeight: Double? = 10
```
```
if let rectOneWidth = rectOneWidth,
    let rectOneHeight = rectOneHeight {
    print(" The area of rectOne is \(rectOneWidth * rectOneHeight)")
} else {
    print("no such value")
}


```

b. Given the variables `rectTwoWidth` and `rectTwoHeight` below, print "The are of rectTwo is not able to be calculated".  Use *Optional Binding* (`if let`) to print this message.

```swift
var rectTwoWidth: Double? = nil
var rectTwoHeight: Double? = nil
```
```
if let rectTwoWidth = rectTwoWidth,
    let rectTwoHeight = rectTwoHeight {
    print("the value of rectTwo is \(rectTwoWidth * rectTwoHeight )")
} else {
    print("The are of rectTwo is not able to be calculated")
}

```

## Question 3

a. Given the variables `userOneName`, `userOneAge`, and `userOneHeight` below, write code that prints "Hello Anne!  You are 15 years old and 5.8 feet tall" (1 foot = 12 inches).  Use optional binding.


```swift
var userOneName: String? = "Anne"
var userOneAge: Int? = 15
var userOneHeight: Double? = 70

```
```
if let bindedName = userOneName,
    let bindedAge = userOneAge,
    let bindedHeight = userOneHeight {
print("Hello \(bindedName)!, You are \(bindedAge) years old and \(bindedHeight / 12) feet tall")
} else {
    print("no info is available")


```

b. Given the variables `userTwoName`, `userTwoAge` and `userTwoHeight` below, write code that prints "Hello user!  You are 15 years old and I don't know how tall you are".  Use optional binding

```swift
var userTwoName: String? = nil
var userTwoAge: Int? = 15
var userTwoHeight: Double? = nil
```
```
if let userTwoName = userTwoName,
let userTwoAge = userTwoAge,
    let userTwoHeight = userTwoHeight {
    print("Hello \(userTwoName), you are \(userTwoAge) years old and \(userTwoHeight) feet tall")
} else {
    print("Hello user you are \(userTwoAge ?? 0) years old and I dont know how tall you are")
}



```


## Question 4

Give the variable `favoriteNumber`, write code that either prints "Your favorite number is " followed by the number, or "I don't know what your favorite number is"

`favoriteNumber` is of type Int? and will either be `nil` or a random number between 0 and 10.  It will change each time you run your Playground.

```swift
var favoriteNumber = Bool.random() ? Int.random(in: 0...10) : nil
print(favoriteNumber ?? "I dont know what your favorite number is")
```



## Question 5

Given the variables `numOne`, `numTwo` and `numThree`, write code that prints "The sum of all the numbers is " followed by their sum.  If a number is `nil`, don't add it to the sum.  If all numbers are `nil`, the sum is zero.

```swift
var numOne = Bool.random() ? Int.random(in: 0...10) : nil
var numTwo = Bool.random() ? Int.random(in: 0...10) : nil
var numThree = Bool.random() ? Int.random(in: 0...10) : nil
```
```
if let numOne = numOne,
let numTwo = numTwo,
    let numThree = numThree {
    print("the sum of all the numbers is \(numOne + numTwo + numThree)")
} else {
    print("the sum is zero")
}


```

## Question 6

a. Given the variable `numbers` below, write code that prints "The sum of all the numbers is " followed by their sum.  If a number is `nil`, don't add it to the sum.  If all numbers are `nil`, the sum is zero.

```swift
var numbers = [Int?]()

for _ in 0..<10 {
    numbers.append(Bool.random() ? Int.random(in: 0...100) : nil)
}
```

b. Using the same variable, find the average of all non-nil values.

## Extra Questions

https://github.com/joinpursuit/Pursuit-Core-iOS-Extra-Optionals-Questions/blob/master/README.md
