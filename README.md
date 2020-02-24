import UIKit

class ViewController: UIViewController {
    @IBOutlet weak var diceImageView1: UIImageView!
    @IBOutlet weak var diceImageView2: UIImageView!
    let diceArray = [#imageLiteral(resourceName: "DiceOne"),#imageLiteral(resourceName: "DiceTwo"),#imageLiteral(resourceName: "DiceThree"),#imageLiteral(resourceName: "DiceFour"),#imageLiteral(resourceName: "DiceFive"),#imageLiteral(resourceName: "DiceSix")]
       
    @IBAction func rollButtonPressed(_ sender: UIButton) {
        
        
        
        diceImageView1.image = diceArray.randomElement()
        diceImageView2.image = diceArray.randomElement() //choses which of the dices by random or could've kept the  diceArray[Int.random(in: 0...5) - that's too specific b/c I may want to change the image literal to or modify]
                     
        
    }
     
    
}
