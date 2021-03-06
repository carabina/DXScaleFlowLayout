# DXScaleFlowLayout

![CocoaPods](https://img.shields.io/cocoapods/v/DXScaleFlowLayout.svg)
![Platform](https://img.shields.io/badge/platforms-iOS%208.0+-333333.svg)
![Swift](https://img.shields.io/badge/Swift-4.2-orange.svg)

DXScaleFlowLayout is a subclass of the UICollectionViewFlowLayout allowing the display of scale up/down cells in a UICollectionView.

![Demo](https://github.com/SiriDx/DXScaleFlowLayout/blob/master/Resources/scaleflowlayout.gif)

1. [Requirements](#requirements)
2. [Integration](#integration)
3. [Usage](#usage)
- [Basics](#basics)
- [Property](#property)

## Requirements

- iOS 8.0+
- Xcode 8

## Integration

#### CocoaPods (iOS 8+)

You can use [CocoaPods](http://cocoapods.org/) to install `DXScaleFlowLayout` by adding it to your `Podfile`:

```ruby
platform :ios, '8.0'
use_frameworks!

target 'MyApp' do
pod 'DXScaleFlowLayout', '~> 1.0.0'
end
```

#### Manually (iOS 7+)

To use this library in your project manually, you may drag DXScaleFlowLayout.swift to the project tree

## Usage

#### Basics

Import DXScaleFlowLayout module

```swift
import DXScaleFlowLayout
```

Create an instance of DXScaleFlowLayout with transform scale you need to initialize your UICollectionView

```swift
let scaleLayout = DXScaleFlowLayout()
scaleLayout.transformScale = 0.15

UICollectionView(frame: .zero, collectionViewLayout: scaleLayout)
```

#### Property

- **transformScale**:

```swift
open var transformScale: CGFloat
```

- **isPagingEnabled**:

```swift
open var isPagingEnabled: Bool = true
```



