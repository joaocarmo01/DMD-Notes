# DMD GRACE WORKSHOP 2

## Person creation

class always uper case, no camle casing
String always uper case, "  ""   """
Intergete a;ways uper case, " "" """

Init = Initialize (means) to turn on the fucntions makes the computer ware of the variables (var)

Speech marks around characters not numbers

**Project**

```swift

import UIKit

class ViewController: UIViewController {
    
    let me = Person(name: "Joao", age: 18)

    override func viewDidLoad() {
        super.viewDidLoad()
        nameLabel.text = me.name
        }
     @IBOutlet weak var nameLabel: UILabel!    
}
```
