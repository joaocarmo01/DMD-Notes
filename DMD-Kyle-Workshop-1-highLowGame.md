# High-Low-Game

```swift
import UIKit

class ViewController: UIViewController {

    var target = 0
    var newTarget = 0
    var score = 0
    
    @IBOutlet weak var scoreLabel: UILabel!
    
    @IBOutlet weak var targetLabel: UILabel!
    
    
    override func viewDidLoad() {
        super.viewDidLoad()
        generateRandomNumber()
    }

    func generateRandomNumber() {
        newTarget = Int.random(in: 0...100)
    }

    @IBAction func higherGuess(_ sender: Any) {
    generateRandomNumber()
        if newTarget > target {
            correctGuess()
        } else {
            wrongGuess()
        }
    }
    
    
    @IBAction func lowerGuess(_ sender: Any) {
    generateRandomNumber()
    if newTarget < target {
        correctGuess()
    } else {
        wrongGuess()
      }
    }
    
    func correctGuess() {
        score += 1
       target = newTarget
        scoreLabel.text = "Score: \(score)"
        targetLabel.text = "\(target)"
    }
    
    func wrongGuess() {
        score = 0
        target = 0
        newTarget = 0
        scoreLabel.text = "Score: \(score)"
        targetLabel.text = "\(target)"
    }
}

```
