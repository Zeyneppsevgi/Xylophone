![App Brewery Banner](Documentation/AppBreweryBanner.png)

# Xylophone

## Our Goal

The goal of this tutorial is to dive into a simple iOS recipe - how to play sound and use an Apple library called AVFoundation. The most important skill of a great programmer is being able to solve your own problems. We’ll do that by exploring StackOverflow, Apple Documentation and learning how to search for solutions effectively. By learning to use these tools, you’ll be able to start adding custom features to an app and get it to do what you want it to.


## What you will create

You will be making your first musical instrument! Music apps are so popular on the App Store that they even get their own category. So in this module, we’re going to make a colourful XyloPhone app. Get it? Ok, the jokes are bad, but remember, I only wrote the good ones... 

## What you will learn

* How to play sound using AVFoundation and AVAudioPlayer.
* Understand Apple documentation and how to use StackOverflow.
* Functions and methods in Swift. 
* Data types.
* Swift loops.
* Variable scope.
* The ViewController lifecycle.
* Error handling in Swift.
* Code refactoring.
* Basic debugging.

* "It is a kalimba application, and when each color block is pressed, it produces different sounds."
  ![Screenshot](https://cdn.discordapp.com/attachments/800783429905940482/1131181788597858405/Simulator_Screenshot_-_iPhone_14_-_2023-07-19_at_14.00.09.png)

## Replacement Code

```
import UIKit
import AVFoundation

class ViewController: UIViewController {
    
    var player: AVAudioPlayer!

    override func viewDidLoad() {
        super.viewDidLoad()
    }

    @IBAction func keyPressed(_ sender: UIButton) {
        playSound()
    }
    
    func playSound() {
        let url = Bundle.main.url(forResource: "C", withExtension: "wav")
        player = try! AVAudioPlayer(contentsOf: url!)
        player.play()
                
    }
}
```



>This is a companion project to The App Brewery's Complete App Development Bootcamp, check out the full course at [www.appbrewery.co](https://www.appbrewery.co/)

![End Banner](Documentation/readme-end-banner.png)




