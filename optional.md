```swift
var name: String?
var email: String?
var age: Int?

// Stimulate user input
name = "Adesh"
email = "shaha@algonquincollege.com"
// Age is not provided


// check if user's age is provided
if let userAge = age {
    print("User's age is \(userAge)")
} else{
    print("User's age is not provided")
}

// Later in the code, use the provided values

if let userName = name, let userEmail = email{
    print("Hello, \(userName)! Your email is \(userEmail).")
} else{
    print("Print fill in your name and email")
}
```
