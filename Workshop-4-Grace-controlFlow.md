## Workshop 04 - Control Flow
  
**What is countrol flow?**

The order of a project, how functions, variables, call's are arranged.

**Why is countrol flow important?**

Control flow helps the computer to understand the task that its set to do better, provideing for a more efficient and esier work flow

**What is an array?**

An array is an area of data storage, is acollection of variables of the same type

**What is an if statement?**

A function that allows for the comparison of values and whatnis expected of them

```swift

func checkNumber(){
        if number == 10 {
            print ("yes it is")
        }
        
```

**What is a guard statement?**

Guard statemnets work like an if statemnt, however they only run/work wehn the set conditions are not met
Much safer than else satemnet andesier to use
Dont do piramid of doom (DONT)

```swift
func validateMobileNo(mobileNo: String){
            guard mobileNo.count == 10
                else {return}
        }
```

**What is else used for and what is the notation for it?**

else is used to contradict teh if satement

```swift
 func checkNumber(){
        if number == 10 {
            print ("yes it is")
        } else {
            print("no it does not")
        }
```

**Why do you have to use else in a gaurd statemnt?**

The else statemnt is always included in the gurad statemnt, it is teh condition that runs if the conditions in the guard statemnt are not met 

**Describe a loop statement?**

1. tehre is alist of items
2. an outcome is filtered after the comand
3.
Uses an array (list) of items. The command then filters through the list and the outcome is a value from that list. The list can be of any type for example: dictionaries, strings, intagers etc.

**Which statement does 'for in' most commonly use?**


**Workshop 4**

```swift
//
//  ViewController.swift
//  Workshop 4
//
//  Created by Joao Carmo (s5215505) on 10/10/2019.
//  Copyright © 2019 Joao Carmo (s5215505). All rights reserved.
//

import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var usernameField: UITextField!
    @IBOutlet weak var passwordField: UITextField!
    @IBOutlet weak var confirmPasswordField: UITextField!
    @IBOutlet weak var errorLabel: UILabel!
    
    
    override func viewDidLoad() {
        super.viewDidLoad()
    errorLabel.isHidden = true
    usernameField.text = "Joao"
    passwordField.text = "password"
    confirmPasswordField.text = "password1"
        
        }

    @IBAction func goButton(_ sender: UIButton) {
        guard let username = usernameField.text, let password = passwordField.text, let confirmPasswordField = confirmPasswordField.text else {
            return
        }
        
        if password == confirmPasswordField {
            print("yes they match")
            errorLabel.isHidden = false
            errorLabel.text = "passwords match"
        } else {
            print("no they do not match")
            errorLabel.isHidden = false
             errorLabel.text = "passwrod dont match, try again."
        }
        
       
    }
    
}


```


