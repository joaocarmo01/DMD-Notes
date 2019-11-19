# High-Low-Game

```swift
//
//  ViewController.swift
//  App 1 try 6
//
//  Created by Joao  Carmo on 09/10/2019.
//  Copyright © 2019 Joao  Carmo. All rights reserved.
//

import UIKit

class ViewController: UIViewController {

    var score = 0
    var target = 0
    var  newTarget = 0
    
    @IBOutlet weak var scoreLabel: UILabel!
    
    @IBOutlet weak var targetLabel: UILabel!
    
    
    
    override func viewDidLoad() {
        super.viewDidLoad()
        generateRandomNumber()
    }

    func generateRandomNumber() {
        newTarget = Int.random(in: -50...50)
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
        targetLabel.textColor = UIColor.black
        scoreLabel.text = "Score \(score)"
        targetLabel.text = "\(target)"
    }
    
    func wrongGuess(){
        score = 0
        target = 0
        newTarget = 0
        targetLabel.textColor = UIColor.red
        scoreLabel.text = "Score \(score)"
        targetLabel.text = "\(target)"
    }

}




```
High low helped e understand the use of fuctions an dwhen they should be utelized.
Also allowed me to see thta it is possibel to create something with very minimal code.
Learned how to conect actions.
