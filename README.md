# MarkdownSwiftZee #
[![Swift](https://img.shields.io/badge/swift-3.0-orange.svg?style=flat)](https://developer.apple.com/swift/)
[![License](https://img.shields.io/badge/license-MIT-71787A.svg)](https://tldrlegal.com/license/mit-license)
[![Platforms](https://img.shields.io/badge/Platforms-OS--Linux-lightgray.svg?style=flat)](https://swift.org)

Markdown to HTML via discount.

## Installation

```swift
import PackageDescription

let package = Package(
    dependencies: [
        .Package(url: "https://github.com/ziligy/MarkdownSwiftZee.git", majorVersion: 0, minor: 1)
    ]
)
```

## Usage

```swift
import MarkdownSwiftZee

let markdown = "# MarkdownSwiftZee\n[![Swift](https://img.shields.io/badge/swift-3.0-orange.svg?style=flat)](https://developer.apple.com/swift/)\n[![License](https://img.shields.io/badge/license-MIT-71787A.svg)](https://tldrlegal.com/license/mit-license)\n[![Platforms](https://img.shields.io/badge/Platforms-OS--Linux-lightgray.svg?style=flat)](https://swift.org)\n\nMarkdown to HTML via discount."

let md = try Markdown(from: markdown)

print(md.html)
```

