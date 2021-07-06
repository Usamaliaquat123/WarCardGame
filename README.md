# War Card Game

[![GitHub license](https://img.shields.io/github/license/obrienser/WarCardGame)](https://github.com/obrienser/WarCardGame/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/obrienser/WarCardGame)](https://github.com/obrienser/WarCardGame/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/obrienser/WarCardGame)](https://github.com/obrienser/WarCardGame/network)
[![visitors](https://visitor-badge.glitch.me/badge?page_id=obrienser.WarCardGame)](https://github.com/obrienser)

## About the game
///

## Technology
* Swift
* UIKit
* MVVM

## Screenshots

<p align="center">
  <img src="https://user-images.githubusercontent.com/50111192/124563568-d2c3f000-de48-11eb-9861-d7c0e94f462e.PNG" alt="" height="450"> &nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/50111192/124563577-d5264a00-de48-11eb-87b6-dfeb9522b0a7.PNG" alt="" height="450"> &nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/50111192/124563589-d788a400-de48-11eb-99b1-25b701fbc4f8.PNG" alt="" height="450"> &nbsp;&nbsp;<img src="https://user-images.githubusercontent.com/50111192/124563602-d9eafe00-de48-11eb-9945-2c096a96bbcd.PNG" alt="" height="450">
</p>

## Sample code
>dealTapped function

```swift
@IBAction func dealTapped(_ sender: Any) {
        
        // Randomize some numbers
        let leftNumber = Int.random(in: 2...14)
        let rightNumber = Int.random(in: 2...14)
        
        // Update the image views
        leftImageView.image = UIImage(named: "card\(leftNumber)")
        rightImageView.image = UIImage(named: "card\(rightNumber)")
        
        // Compare the random numbers
        if leftNumber > rightNumber {
            
            // Left side wins
            leftScore += 1
            leftScoreLabel.text = String(leftScore)
            
        }
        else if leftNumber < rightNumber {
            
            // Right side wins
            rightScore += 1
            rightScoreLabel.text = String(rightScore)
            
        }
        else {
            // Tie
        }
        
    }
```

## Requirements
* iOS 14.2
* Xcode 12.0
* Swift 5.3

## Install
Just open project and run :rocket:

<br>
<p align="center">
  <a href="https://www.buymeacoffee.com/obrienser">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me A Coffee" width="140">
  </a>
</p>
