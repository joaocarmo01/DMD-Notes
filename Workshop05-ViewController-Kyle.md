## Workshop 05 - View Controllers

: (means of type)

**Generally describe what a View Controller is.**

View Controller is a new "screen" on the app

**All your view controllers are "sub classes" of what?**

All or view controllers are subcalsses of the main screen, the starting screen

**What is the life cycle of the view controller?**

It is where the braket of theat view controller sarts and ends

**Name at least two (other than the one given) of the functions we can use in this life cycle.**
  
```swift
  viewDidLoad()

override func viewWillAppear(_ animated: Bool) {
    super.viewWillAppear(animated)
    resetGame()
  }
```
 
**What is a segue?**

is what cnectcts each screen together and teh order they should be arranged

**What is the segue "Identifier"?**

An identifier is a name that we give to an object

**How do you setup a segue from a button in your storyboard?**

control and drag to the next viewcontroller

**How do you setup a segue between view controllers (ie without using a button)?**

use the viewcontroller on the privious scren base and control and drag it to the next scree (new view controller)

**How do you call a segue programatically?**



**Briefly describe how you pass data between two view controllers (you may want to save some snippets of code here)?**

```swift
 
 override func prepare(for segue: UIStoryboardSegue, sender: Any?) {
        let vc = segue.destination as! GameOverViewController
        vc.score = score
    }
 
 override func viewDidLoad() {
        super.viewDidLoad()
        scoreLabel.text = "\(score)"
        dismiss(animated: true, completion: nil)
    }
```
