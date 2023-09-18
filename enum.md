```swift
enum ProductCategory{
    case electronics
    case clothing
    case books
}

struct Product{
    let name: String
    let price: Double
    let category: ProductCategory
}

let iPhone = Product(name: "iPhone 15", price: 999.99, category: .electronics)
let androidPhone = Product(name: "Google Pixel", price: 599.99, category: .electronics)

let books = Product(name: "Swift Programming", price: 34.99, category: .books)

func calTotalPrice(products: [Product], inCategory: ProductCategory) -> Double {
    var total = 0.0
    for product in products{
        if product.category == inCategory{
            total += product.price
        }
    }
    return total
}

let products = [iPhone, books, androidPhone]

let totalPriceElectronics = calTotalPrice(products: products, inCategory: .electronics)

print(totalPriceElectronics)
```
