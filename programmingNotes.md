Dictionaries// 
Create and Store 
Keys in dictioanries are used to look up associated values. 

Bsic Structure 
var dictionaryName: [KeyType: ValueType]
var studentGrades: [String: Int]
String = key (student name)
Int = value (grade)
Empty Dictionary 
var scores: [String: Int] = [:]
Optional Binding 
if let score = scores["Peter"] {
    print(score)
}
Adding Values 
scores["Mike"] = 88

to add to dictionary 

travelMiles["Daryl"] = 700
retrieve from dictionary 
if let tracellermiles = travelMiles["Peter"]
how to remove an item if let deletedItem = trabvelMiles.removeValus()




Using different types with arrays

you can create a new array by adding to arrays of the same type 

arrays by default are set to handle specific types 

var aArray:[Int] = [1,2,3]
var bArray:[Int] = [4,5,6]

var cArray:[Int] = aArray + bArray

print(cArray)


array with mixed types 

var anArray: [Any] = [59]
anArray.append(3.33)
anArray.append("orange") 

TUPLES 

var vegArray: [Any] = ["carrot", 3, true] 
NOT IDEAL ^^^ 

var vegetable = ("carrot", 3, true)
func getUser() -> (name: String, age: Int) {
    return ("Peter", 39)
}

Tuples are used to store mulitple values of different data types.  

Arrayss-->  stores an ordered list value of the same type 
var array: [String]  = []

when creating an array you hav to specify the type. type inference doesnt work with empty array 

Array index 

var train1 = ["wheat", "barley", "wheels"]

edit array 

train1[1] = "barley"

counting in array 

print(train1.count) --> will return 3 items
append() --> to add item to end of an array 
train1.append("")

insert() --> adds to specific location

remove() --> removes item 

train1.remove(at: 4) 

 ​These values are ordered in a sequence and must be of the same data type. ​Each array item can be accessed through its index number. ​And you can use array methods to add and delete items from an array. 

What are optionals? means this variable might have a value..or might be nil (nothing) 
Ex: 
var username: String? = "Joe" String? --> could be a string or could be nil
var username: String? = nil 

Why swift yses optionals.. User didnt ener their name. API didnt return data. image failed to load. database is empty. 

Force Unwrapping (!) means: I promise this is not nill - just give me the value. 
Ex: 
var username: String? = "Joe" 
print(username!) --> Joe 
!DANGER! 
var username: String? = nil 
print(username!) --> App crashes | only use ! when you are 100% sure its not nill. 

Optional binding: If there is a value =, unwrpa it. if not, skip. 

var username: String? = "Peter"

if let unwrappedName = username {
    print("Hello \(unwrappedName)")
}

if its nil 
var username: String? = nil

if let unwrappedName = username {
    print("Hello \(unwrappedName)")
}
!!! Nothings happens no crash!!! 

When to use what
Situation	Use
You are 100% sure value exists	! (rare)
Value might be nil	if let   







Nested Loops ( when they is a loop present inside the body of another loop) 
Break is the keyword to break the flow of a loop immediately 
 purpose of a nested loop is to include a seperate loop inside the body of another loop. 




Using Conditions in loops; 


Basic loops in Swift; 
for in loop 
while loop 
repeat while loop 

For in loop --> repeats for a definite number of times. 
While loop --> repeats while a condition is true. 
Repeat while loop --> Executes loop first before evaluating the condition. 

example syntax: 

For-in loop over a range 

for value in 1...5 
{
print("this is item \(value)")
}

examples of for loops in swift. 

For in loops execute a block of code a given number of times. This type of loop is useful when you know the number of iterations beforehand.

While and repeat while loops execute a block of code while a certain condition is true.

for dice in 1...6 {
    print("Roll a \(dice).")
}

Nested Loops; 
 


Booleans and logial operators: 

== equal to 5==5 
> gretater than 3>2 
< less than 3 < 2 
>= greater than or equal to 4>=3 
<= less than or equal to  4<=3 
!= not equal to 6!= 7 

Logical operators 

&& AND  
|| OR
!  NOT 
^ Exclusive or 5^10 (anything can be used netween 5 and 10 
difference between comparison operators and logical operators; One let’s you compare two values, while the other can evaluate more than one condition to determine if it’s true or false.  

if, if/else and else/if statements: 
Conditional are used to check wether a condition is met 
if statement checks is a condition and runs code if condition is true 

if statement 

let water = 0 
if waterTemp == 0 {
print("The water is freezing")
}

else statement 

let waterTemp = 92 
if waterTemp >= 100 {
print("water boiling")
} 
else {
print("not boiling")
}


Else/if statement lets you nest multiple if statements to test many conditions that depends on each other. 
Strings in Swift: An ordered collection of characters surrounded by double quotes



Switch Statements are conditionals that compare the value of a constant or varibe with a fixed set of values. 

switch statements advantages over else if statements; 

var stringA = "Hello there" unicode 

String literals: 
let myString = "Hello World" <--String literal 

String mutability 
Assign to constant <-- the string is immutable can't be modified. 

Combining Strings: 

let stringA = "Hi"
let stringB = "there"
let newString = stringA = stringB --> returns "Hi there" 

let quote = "hello world" 

Comparing Strings 
quote.hasPrefix("H") returns boolean value true 

quote.hasSuffix("rld") returns true 

convert strings 

let aString = "hi there" 

let upper = aString.uppercased() --> "HI THERE"
let lower = aString.lowerCased() --> "hi there"

counting number of characters: 

let aString = "Hi there"
let theCount = stringA.count --> returns 8

create  multi-line string literals: 

let mlString = """ coffee 
latte
more and more wysiwyg

intro to programming and its history.
0 = off 
1 = One 
Transistor = CPU 

programming is a set of instructions that a computer uses to perform a specific function. 

Constants, variables and data types in swift. 
variables store different types of information. 
Constant is a value that cannot be changed. 

Declare a constant: 

let name <-- Constant

Let name = <--- Assignment operator 

let name = 10 <--- cannot change 

Declare a Variable : 

var exampleA <--- A varaible 

var exampleA = 20 <--- Type of variable 

Data Types: 

Integers = whole numbers 
Floating point = decimal numbers 

floating point = 15.25 (32-bit floating-point)
Double  = 10.233444444 (64-bit floating-point)

Boolean data type 

//Swift is type safe language 

Using operators in Swift; 

Arithmetic (integer and floating points (Double)) 

+*-/ 

Multiplication basic math 

var firstValue = 3 * 10 <--- value if 30 will be stored in firstvalue 

compound operators: work out the answer and store it.
compound operators are best used for combining the equal with another operator to perform two task at once 

floating point numbers: 

var firstValue = 3.3 (double) 

firstValue = firstValue + 1.5 returns --> 4.8 

Division: 
firstValue = 20/6 returns 3.33333

Modulos operator returns the remainder: 

var basket = 10 % 2 <-- returns value of remainder 0 

BIDMAS
 Brackets <-- Highest priority 
Indices 
Division 
Multiplication 
Addition 
Subtraction <-- Lowest priority

Unary minus operator: Toggle the sign of a numeric value by prefixing (-) 

let one = 1 
let negativeValue = -one <-- returns negativeValue = -1 

different types cant be added together. need to covert 

let x = 5 
let y = 0.33 
let z = Double(x) + y <-- prefixed with correct type <-- returns x is inferred double with a value of 5.0 

 
 


