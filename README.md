# Internet Pro for iOS (Xcode)

This is the native SwiftUI/WebKit iPhone and iPad browser project. It is separate from the Avalonia iOS project in `../iOS` and from the Windows, Android, Linux, and Darwin builds.

Open `InternetPro.xcodeproj` on a Mac with Xcode installed, select an iOS Simulator or signed iPhone/iPad destination, then build and run the `Internet Pro iOS` scheme. This Windows workspace cannot run `xcodebuild` or an iOS Simulator, so the native target still needs validation on macOS.

The browser includes multiple `WKWebView` tabs, known-domain navigation blocks, YouTube Restricted Mode preference, YouTube fullscreen suppression, and a touch slider that closes inactive tabs after 30, 10, or 2 minutes. The selected tab is kept open. Tab cleanup releases WebKit views but cannot guarantee a specific RAM saving, a 9 GB allocation, or the absence of native WebKit memory leaks.