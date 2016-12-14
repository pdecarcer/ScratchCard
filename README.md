# ScratchCard
<img src="https://raw.githubusercontent.com/joehour/ScratchCard/master/ScratchCard/result.jpg" width="400" height="800" />

Requirements
----------

- iOS 8.0+
- Xcode 8.0+ Swift 3


## Installation

#### CocoaPods

Check out [Get Started](https://guides.cocoapods.org/using/getting-started.html) tab on [cocoapods.org](http://cocoapods.org/).

To use ScratchCard in your project add the following 'Podfile' to your project

	source 'https://github.com/joehour/ScratchCard.git'
	platform :ios, '8.0'
	use_frameworks!

	pod 'ScratchCard', '~> 1.0.7’

Then run:

    pod install

#### Source Code

Copy the ScratchView.swift and ScratchUIView.swift to your project.

Go ahead and import ScratchCard to your file.


Example
----------

####Please check out the Example project included.


Usage
----------

* Sample:
```swift
    import ScratchCard
    
    class ViewController: UIViewController {

    var scratchCard: ScratchUIView!
    override func viewDidLoad() {
        super.viewDidLoad()
        
        scratchCard  = ScratchUIView(frame: CGRect(x:50, y:80, width:320, height:480),Coupon: "image", MaskImage: "mask", ScratchWidth: CGFloat(40))
        
        self.view.addSubview(scratchCard)
        }
    }
```

Scratched Percent
----------

It is easy to get the scratched percent.
 
* Sample:
```swift
   let scratchPercent: Double = scratchCard.getScratchPercent()
```

##License
ScratchCard is available under the MIT License.

Copyright © 2016 Joe.
