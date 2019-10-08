//Functions 


**What is a function?

Wrap up shunks of code, repetitive tasks that we want to happen time and time again

Bulding blocks:

```swift
 func firstFunc(){
        }
```
"call" this function:

View load to vall the function (usually up on the programing sheet)

```swift
override func viewDidLoad() {
        super.viewDidLoad()
      
       firstFunc()
    }
```

**What are function "arguments" or "parameters?"

to write an argumnet you need an function , an argument and a string than you may print the string
(values thta canebe added into a function) eg: ```swift firstNumber: Int, secondNumber: Int ```

```swift
 func argumnet(username: String){
        print(username)
        }
```
"call" this function:

go up to view did load

```swift
 verride func viewDidLoad() {
        super.viewDidLoad()
      
       firstFunc()
    
    argumnet(username: "Joao")
    argumnet(username: "Jakub")
    argument(username: "Jane")
        }
```

write a function with multiple arguments of different types.

Use a , (coma) to seperate the, 

```swift
func add(firstNumber: Int, secondNumber: Int){
        print(firstNumber + secondNumber)
       }
 
 func subtract(firstNumbert: Int, secondNumber: Int){
      print(firstNumbert - secondNumber)
    }

func devide(firstNumber: Int, secondNumber: Int){
        print(firstNumber / secondNumber)
    }
    
    func times(firstNumber: Int, secontNumber: Int){
    print(firstNumber * secontNumber)
    }
```
"call" this function:

```swift
override func viewDidLoad() {
        super.viewDidLoad()
      
       firstFunc()
    
    argumnet(username: "Joao")
    argumnet(username: "Jakub")
    argumnet(username: "Jane")
        
    add(firstNumber: 6, secondNumber: 7)
   
    subtract(firstNumbert: 23, secondNumber: 7)
       
    devide(firstNumber: 3254364, secondNumber: 324234)
       
    times(firstNumber: 1, secontNumber: 2)
```
**What are return values?

To return a value use ->

```swift
func addNumbers(first: Int, second: Int) -> Int {
        return first + second
    }
 ```

"call" this function

```swift
override func viewDidLoad() {
        super.viewDidLoad()
        
        let result = addNumbers(first: 79, second: 23)
        print(result)
    }
```

**How do you access functions of a class? Give an example.

A calss outlines an object.
Anything in the {} is part of a class and is an object with a specific porpuse.

```swift
class ViewController: UIViewController {}
```

