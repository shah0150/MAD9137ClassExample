```swift
var name: String?
var email: String?
var age: Int?

// Stimulate user input
name = "Adesh"
email = "shaha@algonquincollege.com"
// Age is not provided
//age = 30


// check if user's age is provided
guard let userAge = age else {
    print("User's age is not provided")
    fatalError("Age is required")
}

// Later in the code, use the provided values

guard let userName = name, let userEmail = email else {
   print("Print fill in your name and email")
    fatalError("Email and Password is required")
}

print("Hello, \(userName)! Your email is \(userEmail)")
```
