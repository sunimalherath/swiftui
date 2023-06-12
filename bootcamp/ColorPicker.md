## Usage/Examples

```swift
import SwiftUI

struct ColorPickerView: View {
    @State var backgroundColor: Color = Color.teal
    
    var body: some View {
        ZStack {
            backgroundColor.edgesIgnoringSafeArea(.all)
            ColorPicker("Pick a new color", selection: $backgroundColor, supportsOpacity: true)
        }
    }
}
```
