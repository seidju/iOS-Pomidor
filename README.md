## iOS-Pomidor
Here will be published different questions, that every iOS Developer should know. This questions was asked during different job interviews. I will divide them into different topics for convenience and also try to get every correct answer to all of it.

#### 1. Memory Management
 - [x] What is the difference between **weak** and **unowned**?

So, as everyone knows, **weak** and **unowned** used to break reference cycles, so ARC could successfully dealloc unused class object. A **weak** reference is a reference that does not keep a strong hold on the instance it refers to, and so it’s possible for that instance to be deallocated while the **weak** reference is still referring to it. Therefore, ARC automatically sets a **weak** reference to nil when the instance that it refers to is deallocated. And, because **weak** references need to allow their value to be changed to nil at runtime, they are always declared as variables, rather than constants, of an optional type. You can check for the existence of a value in the **weak** reference, just like any other optional value, and you will never end up with a reference to an invalid instance that no longer exists.

#### FYI:

Property observers aren’t called when ARC sets a weak reference to nil.
 
 
 - [ ] Where **reference** and **value** objects are stored? What is **heap** and **stack**?
 - [ ] Describe step-by-step how **ARC** works. Is there any differecnes between Objective-C and Swift?
 - [ ] What is **autoreleasepool** and when you should use it?
 - [ ] What is **method dispatch**? When you should use **dynamic**, **objc**, **nonobjc**, **final**?
 - [ ] What is **shallow** and **deep** copying?
