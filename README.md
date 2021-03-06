# JCCheckBox

<!--[![CI Status](https://img.shields.io/travis/JasonHan1990/JCCheckBox.svg?style=flat)](https://travis-ci.org/JasonHan1990/JCCheckBox)-->
[![Version](https://img.shields.io/cocoapods/v/JCCheckBox.svg?style=flat)](https://cocoapods.org/pods/JCCheckBox)
[![License](https://img.shields.io/cocoapods/l/JCCheckBox.svg?style=flat)](https://cocoapods.org/pods/JCCheckBox)
[![Platform](https://img.shields.io/cocoapods/p/JCCheckBox.svg?style=flat)](https://cocoapods.org/pods/JCCheckBox)

## Example

JCCheckBox is simple and beautiful checkbox module written in ObjC. It is a subclass of UIControl. You can either use `addTarget(_:action:for:)` function to handle touch event or use block callback `checkCompletion` and `uncheckCompletion` to handle touch event.

![Example Image](https://github.com/JasonHan1990/JCCheckBox/blob/master/ExampleImages/Example.gif)

```objc
// DEFAULT SIZE INIT
JCCheckBox *ovalCheckBox = [JCCheckBox checkBox]; // default size 24 by 24
// SET STYLE
self.ovalCheckBox.checkBoxStyle = JCCheckBoxStyleOval; // square is the default
// CHANGE COLOR
self.ovalCheckBox.innerColor = [UIColor greenColor];
self.ovalCheckBox.outerColor = [UIColor greenColor];
// SET COMPLETION
self.ovalCheckBox.checkedCompletion = ^{
    NSLog(@"Checked");
};
self.ovalCheckBox.uncheckedCompletion = ^{
    NSLog(@"Unchecked");
};
[view addSubview:ovalCheckBox];
```

## Installation

JCCheckBox is available through [CocoaPods](https://cocoapods.org). To install
it, simply add the following line to your Podfile:

```ruby
pod 'JCCheckBox'
```

or

Manually installation. Download the code and drag `JCCheckBox.h` and `JCCheckBox.m` into your project.

## Author

Juncheng Han, namrie1990@gmail.com

My Blog:
https://junchenghan.com/

## License

JCCheckBox is available under the MIT license. See the LICENSE file for more info.
