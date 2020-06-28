# core-data-ios-14-swift-ui-lifecycle
Setup core data in iOS 14 Swift UI lifecycle


More info on Apple forums: https://developer.apple.com/forums/thread/650173

Use Core data in UI

```
import SwiftUI
import CoreData
@main
struct TestApp: App {
    let context = PersistentCloudKitContainer.persistentContainer.viewContext
    
    var body: some Scene {
        WindowGroup {
            ContentView().environment(\.managedObjectContext, context)
        }
    }
}
```
