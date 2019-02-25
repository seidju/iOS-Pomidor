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

 - [ ] Composition vs Inheritance
 - [x] Abstract factory, factory method
   * https://github.com/ochococo/Design-Patterns-In-Swift#creational

 - [ ] Observer
 
#### 4. UIKit
 - [ ] CALayer and UIView. Can UIView have no any layers? UIView hiearachy and corresponing CALayer hierarchy?
 - [ ] 10 Tips to prevent UITableView/UICollectionView from frame drop.
 - [ ] CALayers
 - [ ] XIB vs code layout
 - [ ] UIResponder chain
 - [ ] How to handle parent view interaction in complexe sub-view hierarchy?
 - [ ] CALayer vs CGLayer
 - [ ] Frame vs bounds. Cases when change frame and when bounds.
 
 
#### 5. Swift lang
 - [x] Performance improvements
   * https://developer.apple.com/videos/play/wwdc2016/416/
   * https://developer.apple.com/videos/play/wwdc2018/407

 - [ ] Type erasure
 - [ ] Type inference
 - [ ] Method swizzling
 - [ ] What is **method dispatch**? When you should use **dynamic**, **@objc**, **@nonobjc**, **final**?
 
 #### 6. Testing
   * https://github.com/seidju/unit-testing-swift
   * https://www.youtube.com/watch?v=ny2ygMN8waE&feature=youtu.be
   * https://habr.com/ru/company/rambler-co/blog/263087/
