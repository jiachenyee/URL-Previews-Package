# URL Previews

## Usage
```swift
import URL_Previews

// Replace this with any URL you want
let url = URL(string: "https://github.com/sst-inc/")!

// Fetching the page information
url.fetchPageInfo { (title, description, previewImage) -> Void in

    // 🥳 Things are going great
    print("Title : \(title)")
    print("Description : \(description)")
    print("Image URL : \(previewImage)")
    
} failure: { (message) in
    // 😭 An error occurred
    print(message)
}

```
