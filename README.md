# WavedTabView

[![](https://img.shields.io/endpoint?url=https%3A%2F%2Fswiftpackageindex.com%2Fapi%2Fpackages%2Fc-villain%2FWavedTabView%2Fbadge%3Ftype%3Dswift-versions)](https://swiftpackageindex.com/c-villain/WavedTabView)
[![](https://img.shields.io/endpoint?url=https%3A%2F%2Fswiftpackageindex.com%2Fapi%2Fpackages%2Fc-villain%2FWavedTabView%2Fbadge%3Ftype%3Dplatforms)](https://swiftpackageindex.com/c-villain/WavedTabView)
![](https://img.shields.io/github/license/c-villain/WavedTabView)

[![contact: @lexkraev](https://img.shields.io/badge/contact-%40lexkraev-blue.svg?style=flat)](https://t.me/lexkraev)
[![Telegram Group](https://img.shields.io/endpoint?color=neon&style=flat-square&url=https%3A%2F%2Ftg.sumanjay.workers.dev%2Fswiftui_dev)](https://telegram.dog/swiftui_dev)

Tutorial how tab bar can be customised and animated using SwiftUI

Full [demo video](https://t.me/swiftui_dev/194) you may find [here](https://t.me/swiftui_dev/194).

👨🏻‍💻 Feel free to subscribe to channel **[SwiftUI dev](https://t.me/swiftui_dev)** in telegram.

If you like this repository, please do :star: to make this useful for others.

## Quick start

- upside-waved variant:
<p align="left">
<img src="demo1.gif" alt="Example with leading and trailing swipes" height="427" width="280">
</p>

- inside-waved variant: 
<p align="left">
<img src="demo2.gif" alt="Example with leading and trailing swipes" height="427" width="280">
</p>

- without wave, classical variant: 
<p align="left">
<img src="demo3.gif" alt="Example with leading and trailing swipes" height="427" width="280">
</p>

## Installation

To install waved tab view attach [WavedTabView.swift](https://github.com/c-villain/WavedTabView/blob/main/WavedTabView.swift) file to your project and call:

```swift
import SwiftUI

@main
struct SUIChallengesApp: App {
    var body: some Scene {
        WindowGroup {
            WavedTabView() // <=== HERE!
        }
    }
}
```
or for example in SceneDelegate: 
```swift
func scene(_ scene: UIScene, willConnectTo session: UISceneSession, options connectionOptions: UIScene.ConnectionOptions) {
        let contentView = WavedTabView() // // <=== HERE!
       
        if let windowScene = scene as? UIWindowScene {
            let window = UIWindow(windowScene: windowScene)
            window.rootViewController = UIHostingController(rootView: contentView)
            self.window = window
            window.makeKeyAndVisible()
        }
    }
```
### Requirements
- iOS 13.0

## Special thanks

to [Dmitriy Soloshenko](https://github.com/DemonSoft) for his contributing.

## Communication

- If you **found a bug**, open an issue or submit a fix via a pull request.
- If you **have a feature request**, open an issue or submit a implementation via a pull request or hit me up on **lexkraev@gmail.com** or **[telegram](https://t.me/lexkraev)**.
- If you **want to contribute**, submit a pull request onto the master branch.
