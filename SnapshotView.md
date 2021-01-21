iPhone 7 plus snapshot view

Key | Value
--- | ---
Device | iPhone 7 Plus
Software version | 14.2
Xcode version | Version 12.3 (12C33)


My code:
```swift
override func viewDidAppear(_ animated: Bool) {
    super.viewDidAppear(animated)
        
    let snapview = UIScreen.main.snapshotView(afterScreenUpdates: true)
        
    snapview.frame = view.frame
    view.addSubview(snapview)
        
    snapview.transform = CGAffineTransform(scaleX: 0.8, y: 0.8)
        
}
```

Result:

<img src="https://raw.githubusercontent.com/aheze/DeveloperAssets/master/IMG_9560.PNG" width="300">

