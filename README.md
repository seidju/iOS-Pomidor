## iOS-Pomidor
Here will be published different questions, that every iOS Developer should know. This questions was asked during different job interviews. I will divide them into different topics for convenience and also try to get every correct answer to all of it.

#### 1. Memory Management
 - [x] What is the difference between **weak** and **unowned** in terms of ARC?

So, as everyone knows, **weak** and **unowned** used to break reference cycles, so ARC could successfully dealloc unused class object. A **weak** reference is a reference that does not keep a strong hold on the instance it refers to, and so it’s possible for that instance to be deallocated while the **weak** reference is still referring to it. Therefore, ARC automatically sets a **weak** reference to nil when the instance that it refers to is deallocated. And, because **weak** references need to allow their value to be changed to nil at runtime, they are always declared as variables, rather than constants, of an optional type. You can check for the existence of a value in the **weak** reference, just like any other optional value, and you will never end up with a reference to an invalid instance that no longer exists.

FYI: Property observers aren’t called when ARC sets a weak reference to nil.
 
 
 - [x] Where **reference** and **value** objects are stored? What is **heap** and **stack**?
   https://medium.com/@abhimuralidharan/difference-between-value-type-and-a-reference-type-in-ios-swift-18cb5145ad7a
   https://stackoverflow.com/questions/27441456/swift-stack-heap-understanding
   https://medium.com/devslopes-blog/swift-data-structures-heap-e3fbbdaa3129
   
 - [x] Describe step-by-step how **ARC** works. Is there any differecnes between Objective-C and Swift?
   https://medium.com/computed-comparisons/garbage-collection-vs-automatic-reference-counting-a420bd4c7c81
   https://medium.com/@ITZDERR/ios-memory-management-history-high-level-part-1-118f57b613d6
   https://medium.com/@ITZDERR/ios-memory-management-arc-in-objective-c-and-swift-part2-f8d269c5e9c

 - [ ] What is **autoreleasepool** and when you should use it?
 - [ ] What is **shallow** and **deep** copying?

#### 2. Architectures
 - [ ] VIPER
 - [ ] Riblets
 - [ ] Clean Architecture
 - [ ] MVP
 - [ ] MVVM
 - [ ] 4V Engine
 
#### 3. UIKit
 - [ ] CALayer and UIView. Can UIView have no any layers? UIView hiearachy and corresponing CALayer hierarchy?
 - [ ] 10 Tips to prevent UITableView/UICollectionView from frame drop.
 - [ ] CALayers
 - [ ] XIB vs code layout
 - [ ] UIResponder chain
 - [ ] How to handle parent view interaction in complexe sub-view hierarchy?
 
#### 4. Swift lang
 - [ ] Type erasure, type inference
 - [ ] Method swizzling
 - [ ] What is **method dispatch**? When you should use **dynamic**, **@objc**, **@nonobjc**, **final**?
