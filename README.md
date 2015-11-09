# ABCircularProgressView

`ABCircularProgressView` is a simple circular progress view written in Swift 2, it draws the circular progress and a stop button (App store look like)


#### `ABCircularProgressView` an example in one of my apps. [link](https://itunes.apple.com/en/app/id994829561):
<img src="https://raw.githubusercontent.com/adilbenmoussa/ABCircularProgressView/master/ABCircularProgressView/screenshot.png" width="400">

`ABCircularProgressView` inherits from UIView, so you can just use it as a normal view in the `Interface builder`

<img src="https://raw.githubusercontent.com/adilbenmoussa/ABCircularProgressView/master/ABCircularProgressView/interface-builder.png" width="400">

```swift
//define it
@IBOutlet weak var progressView: ABCircularProgressView!

//use it
progressView.progress = CGFloat(downloadProgress)
```

## Properties

####tintCGColor: `CGColor`
The color of the progress view and the stop icon.

####stopSizeRatio: `CGFloat`
 Size ratio of the stop button related to the progress view, default 1/3 of the progress view

####progressBackgroundOpacity: `Float`
The Opacity of the progress background layer

####lineWidth: `CGFloat`
The width of the line used to draw the progress view.

## Playgroud example
<img src="https://raw.githubusercontent.com/adilbenmoussa/ABCircularProgressView/master/ABCircularProgressView/playground.png" width="600">

```swift
// Test the ABCircularProgressView component
let progressIndicatorView = ABCircularProgressView(frame: CGRect(x: 0.0, y: 0.0, width: 600.0, height: 600.0))
var progress: CGFloat = 0
for i in 0..<101 {
    progress = CGFloat(Float(i) / 100.0)
    progressIndicatorView.progress = progress
}
```

##ToDo list
- [x] Playground example
- [] Project example
- [] Add spin progress
- [] Cocoapods support

##Contact
Mail me at [adil.benmoussa@gmal.com](adil.benmoussa@gmal.com)


##License

The MIT License (MIT)

Copyright (c) 2015 Adil Ben Moussa

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.




