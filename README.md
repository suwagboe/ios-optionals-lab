# Optionals lab

Fork and clone this repo. On your fork, answer and commit the follow questions. When you are finished, submit the link to your repo on Canvas.


## Question 1

a. Given the variable `userNameOne` below, print *"The username is Test User"*.  Use *Optional Binding* (`if let`) to print the name.

```swift
var userNameOne: String? = "Test User"
```

```
if let newName = userNameOne {
print("The userName is \(newName)")}
else{
print("The username is Test User")
}


```

b. Given the variable `userNameTwo` below, print *"The username is undefined"*.  Use the *nil coalescing operator* (`??`).

```swift
var userNameTwo: String? = nil
```

```
var userNameTwo: String?? "The username is undefined"
print("userNameTwo")
```

## Question 2

a. Given the variables `rectOneWidth` and `rectOneHeight` below, print "The area of rectOne is 50".  Use *Optional Binding* (`if let`) to print the area.

```swift
var rectOneWidth: Double? = 5
var rectOneHeight: Double? = 10


var rectOneWidth: Double? = 5
// this is initializing it to be an optional double
var rectOneHeight: Double? = 10

if let area = Double?((rectOneWidth ?? 2.2) + (rectOneHeight ?? 5.5)){
print("The area of rectOne is \(area)")
} else {
print("The area is not valid")
}

```

b. Given the variables `rectTwoWidth` and `rectTwoHeight` below, print "The are of rectTwo is not able to be calculated".  Use *Optional Binding* (`if let`) to print this message.

```swift
var rectTwoWidth: Double? = nil
var rectTwoHeight: Double? = nil
```
```
if let unwrappedrect2width = rectTwoWidth, let unwrappedrect2height = rectTwoHeight {
   let areaTwo = unwrappedrect2width * unwrappedrect2height
   print("The area of rectTwo is \(areaTwo)")
   }else {
print("The area of rectTwo is not able to be calculated.")
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
print ("Hello \(userOneName) !  You are \(userOneAge) years old and (\(userOneHeight)/ 12)! feet tall")
```
b. Given the variables `userTwoName`, `userTwoAge` and `userTwoHeight` below, write code that prints "Hello user!  You are 15 years old and I don't know how tall you are".  Use optional binding

```swift
var userTwoName: String? = nil
var userTwoAge: Int? = 15
var userTwoHeight: Double? = nil
```


## Question 4

Give the variable `favoriteNumber`, write code that either prints "Your favorite number is " followed by the number, or "I don't know what your favorite number is"

`favoriteNumber` is of type Int? and will either be `nil` or a random number between 0 and 10.  It will change each time you run your Playground.

```swift
var favoriteNumber = Bool.random() ? Int.random(in: 0...10) : nil
```
```
if let newNum = favoriteNum {
print("Your favorite number is \(newNum)")
}
else {
print("I do not know what your favrotie color is...")
}
```


## Question 5

Given the variables `numOne`, `numTwo` and `numThree`, write code that prints "The sum of all the numbers is " followed by their sum.  If a number is `nil`, don't add it to the sum.  If all numbers are `nil`, the sum is zero.

```swift
var numOne = Bool.random() ? Int.random(in: 0...10) : nil
var numTwo = Bool.random() ? Int.random(in: 0...10) : nil
var numThree = Bool.random() ? Int.random(in: 0...10) : nil
```
```
if let firstNum = numOne, let secondNum = numTwo, let thirdNum = numThree{
var sum = firstnum + secondNum + thirdNum 
print("The sum is /(sum)")
}else {
print ("The sum is zero")
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

```
??

```


b. Using the same variable, find the average of all non-nil values.

## Extra Questions

https://github.com/joinpursuit/Pursuit-Core-iOS-Extra-Optionals-Questions/blob/master/README.md
