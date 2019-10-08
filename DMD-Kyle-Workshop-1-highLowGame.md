# High-Low-Game

```swift
import UIKit

class ViewController: UIViewController {

    @IBOutlet weak var ScoreLabel: UILabel!
    
    @IBOutlet weak var TargetLabel: UILabel!
    
    var score = 0
    var target = 0
    var newTarget = 0
    
    override func viewDidLoad() {
        super.viewDidLoad()

        print("hello world")
        
    }

    @IBAction func HigherGuess(_ sender: Any) {
    generateNumber()
        if newTarget > target {
            correctGuess()
        } else {
            wrongGuess()
        }
    }
    
    @IBAction func GuessLower(_ sender: Any) {
   generateNumber()
          if newTarget < target {
              correctGuess()
          } else {
              wrongGuess()
        }
    }
  
    func generateNumber() {
        newTarget = Int.random(in: 0...100)
        }
    func correctGuess() {
       
        score += 1
        target = newTarget
        ScoreLabel.text = "Score: \(score)"
        TargetLabel.text = "\(target)"
    }
    func wrongGuess() {
        score = 0
        target = 0
        newTarget = 0
        ScoreLabel.text = "Score: \(score)"
               TargetLabel.text = "\(target)"
        
        
    }
    

}


```
