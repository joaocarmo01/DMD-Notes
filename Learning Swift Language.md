//Learning Swift Language



let is a constant 
string may only be used with phrares 
int may only be used with numbers
else (or) works like a var (check condition)
if (condition)
else if ( used to check other comnditions)

**Playground 1**

```swift
import UIKit

var str:String = "Hello, playgroundy"

print (str)

var a:Int = 2
var b:Int = 1


a = b

str = String(29)

var c:Float = 2.3
var d:Double = 13.9
var e:Bool = true

print(Int(c))
print(Int(d))
print(Int(round(d)))


var myNumberOfApple = 19


print (a + b)
print (a - b)
print (a * b)
print (a / b)

let f = 10


```


**Playground 2**

```swift
var str = "Hello, playground"

let a = 10
let b = 5
let c = 2
let d = 20

if a < 23 && c > 20 {
    
    print("branch 1")
}

else if !(b > 4) && c > 1 {
    
    print("barnch 2")
}

else if !(c > 13 || a > 5) && b < 10 {
    
    print("branch 3")
}

else if d > 18 {
    
    print("branch 4")
    print("branch 1")
}

else {
    
    print("nothing was true")
}

```
**Playground 3**

```swift

//switch statement

import UIKit

var someCharacter:Character = "c"

switch someCharacter {

case "a":
    print("is an A")

case "b","c":
    print("is a B or C")
        
default:
    print("some fallback")
}

```
Minute: 44.52
https://www.youtube.com/watch?v=Ulp1Kimblg0
