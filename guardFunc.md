```swift
func userRegistration(name: String?, email: String?, age: Int?){

    // check if user's age is provided
    guard let userAge = age else {
        fatalError("Age is required")
    }

    guard let userName = name, let userEmail = email else {
        fatalError("Email and Password is required")
    }

    print("Hello, \(userName)! Your email is \(userEmail), and your age is \(userAge)")
}

userRegistration(name: "Adesh", email: "shaha@algonquincollege.com", age: 30)
```
