## iOS-Pomidor
Here will be published different questions, that every iOS Developer should know. This questions was asked during different job interviews. I will divide them into different topics for convenience and also try to get every correct answer to all of it.

#### 1. Memory Management
 - [x] What is the difference between **weak** and **unowned** in terms of ARC?

So, as everyone knows, **weak** and **unowned** used to break reference cycles, so ARC could successfully dealloc unused class object. A **weak** reference is a reference that does not keep a strong hold on the instance it refers to, and so it’s possible for that instance to be deallocated while the **weak** reference is still referring to it. Therefore, ARC automatically sets a **weak** reference to nil when the instance that it refers to is deallocated. And, because **weak** references need to allow their value to be changed to nil at runtime, they are always declared as variables, rather than constants, of an optional type. You can check for the existence of a value in the **weak** reference, just like any other optional value, and you will never end up with a reference to an invalid instance that no longer exists.

FYI: Property observers aren’t called when ARC sets a weak reference to nil.
 
 - [x] Where **reference** and **value** objects are stored? What is **heap** and **stack**?
   * https://medium.com/@abhimuralidharan/difference-between-value-type-and-a-reference-type-in-ios-swift-18cb5145ad7a
   * https://stackoverflow.com/questions/27441456/swift-stack-heap-understanding
   * https://medium.com/devslopes-blog/swift-data-structures-heap-e3fbbdaa3129
   
 - [x] Describe step-by-step how **ARC** works. Is there any differecnes between Objective-C and Swift
   * https://medium.com/computed-comparisons/garbage-collection-vs-automatic-reference-counting-a420bd4c7c81
   * https://medium.com/@ITZDERR/ios-memory-management-history-high-level-part-1-118f57b613d6
   * https://medium.com/@ITZDERR/ios-memory-management-arc-in-objective-c-and-swift-part2-f8d269c5e9c

 - [x] What is **autoreleasepool** and when you should use it?
   * https://en.swifter.tips/autoreleasepool/
   * https://medium.com/fueled-engineering/memory-management-in-swift-common-issues-90dd7c08b77

 - [x] What is **shallow** and **deep** copying?
   * https://medium.freecodecamp.org/deep-copy-vs-shallow-copy-and-how-you-can-use-them-in-swift-c623833f5ad3

#### 2. Architectures
 - [x] VIPER
   * https://github.com/strongself/The-Book-of-VIPER

 - [x] RIBs
   * https://github.com/uber/RIBs
  
 - [x] Feedback loop, RxFeedback
   * https://github.com/NoTests/RxFeedback.swift

 - [ ] 4V Engine

#### 3. Design Patterns
 - [x] SOLID, DRY principles
   * https://marcosantadev.com/solid-principles-applied-swift/
   * https://code.tutsplus.com/tutorials/3-key-software-principles-you-must-understand--net-25161
   * https://www.scaledrone.com/blog/solid-principles-for-becoming-a-better-ios-swift-developer/

 - [x] Adapter
   * https://github.com/ochococo/Design-Patterns-In-Swift#-adapter

 - [x] Mediator
   * https://github.com/ochococo/Design-Patterns-In-Swift#-mediator

 - [x] Composition vs Inheritance
   * https://medium.com/ios-os-x-development/protocol-oriented-programming-in-swift-daba92bc9c98

 - [x] Abstract factory, factory method
   * https://github.com/ochococo/Design-Patterns-In-Swift#creational

 - [ ] Observer
 
#### 4. UIKit
 - [x] CALayer and UIView. Can UIView have no any layers? UIView hiearachy and corresponing CALayer hierarchy?
   * https://developer.apple.com/library/archive/documentation/Cocoa/Conceptual/CoreAnimation_guide/BuildingaLayerHierarchy/BuildingaLayerHierarchy.html
 
 - [x] 10 Tips to prevent UITableView/UICollectionView from frame drop.
   * https://www.raywenderlich.com/2752-25-ios-app-performance-tips-tricks#shadowpath
   * https://sohabr.net/habr/post/264817/
   * https://medium.com/capital-one-tech/smooth-scrolling-in-uitableview-and-uicollectionview-a012045d77f
 
 - [x] XIB vs code layout
   * https://www.toptal.com/ios/ios-user-interfaces-storyboards-vs-nibs-vs-custom-code

 - [x] UIResponder chain
   * https://developer.apple.com/documentation/uikit/touches_presses_and_gestures/using_responders_and_the_responder_chain_to_handle_events
   * https://medium.com/ios-os-x-development/understanding-cocoa-and-cocoa-touch-responder-chain-12fe558ebe97
 - [ ] How to handle parent view interaction in complexe sub-view hierarchy?
 - [x] CALayer vs CGLayer
   * https://stackoverflow.com/questions/4458812/whats-the-difference-and-compatibility-of-cglayer-and-calayer
   * https://blog.spacemanlabs.com/2011/07/calayers-v-cglayers-or-which-layer-player/
 
 - [x] Frame vs bounds. Cases when change frame and when bounds.
   * https://stackoverflow.com/questions/1210047/cocoa-whats-the-difference-between-the-frame-and-the-bounds
   * https://medium.com/@GanChau/uiview-frame-vs-bounds-195b9688bde3
   * https://www.hackingwithswift.com/example-code/uikit/whats-the-difference-between-frame-and-bounds
   
 
 
#### 5. Swift lang
 - [x] Performance improvements
   * https://developer.apple.com/videos/play/wwdc2016/416/
   * https://developer.apple.com/videos/play/wwdc2018/407

 - [x] Type erasure
   * https://www.bignerdranch.com/blog/breaking-down-type-erasures-in-swift/
 
 - [x] Type inference
   * https://www.aidanf.net/learn-swift/types_and_type_inference
  
 - [ ] Method swizzling
 - [x] What is **method dispatch**? When you should use **dynamic**, **@objc**, **@nonobjc**, **final**?
   * https://www.raizlabs.com/dev/2016/12/swift-method-dispatch/
   
 
 #### 6. Testing
   * https://github.com/seidju/unit-testing-swift
   * https://www.youtube.com/watch?v=ny2ygMN8waE&feature=youtu.be
   * https://habr.com/ru/company/rambler-co/blog/263087/
