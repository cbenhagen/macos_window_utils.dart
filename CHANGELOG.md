# 1.9.0
- Add `setWindowMinSize` and `setWindowMaxSize` methods to `WindowManipulator` to allow setting the minimum and maximum window size (thanks to [@defuncart](https://github.com/defuncart)).

# 1.8.5
- Prevent `_titlebarHeight` from being set to a negative value when drag resizing the window (thanks to [@CodeEagle](https://github.com/CodeEagle)).

## 1.8.4
- Migrate away from deprecated interfaces.
- Set Flutter version constraint to `">=3.27.0"`.

## 1.8.3
- Undo the migration away from deprecated interfaces, as it caused incompatibilities with older Flutter versions.

## 1.8.2
- Add support for Swift Package Manager. (Thanks to [@EchoEllet](https://github.com/EchoEllet)!)
- Migrate away from deprecated interfaces.
- Add missing documentation to `WindowManipulator.updateToolbarPassthroughView` and `WindowManipulator.removeToolbarPassthroughView`.

## 1.8.1
- Provide support for older Swift compiler versions.

## 1.8.0
- Add `miniaturizeWindow` method (thanks [@parkerhutchinson](https://github.com/parkerhutchinson)).

## 1.7.1
- Fix nil being found when unwrapping an Optional value when `reset` is called before `start` in `MainFlutterWindowManipulator.swift`.

## 1.7.0
- Add `MacosToolbarPassthrough` to allow for the creation of so-called “passthrough views” on the toolbar that relay mouse events to the Flutter application (thanks to [@Andre-lbc](https://github.com/Andre-lbc) and [@adiletcool](https://github.com/adiletcool)).

## 1.6.1

- Add instructions on how to setup macos_window_utils for macOS Monterey and earlier versions.

## 1.6.0

- Add support for a blocking toolbar, that is, a special kind of toolbar that blocks double clicks from the user and allows for UI elements to be placed inside a blocked area (thanks to @cbenhagen and @Andre-lbc).

## 1.5.0
- Add the following window methods:
  - `preventWindowClosure`
  - `allowWindowClosure`
  - `isWindowClosureAllowed`
  - `closeWindow`
  - `performClose`

## 1.4.0

- Add methods to retrieve or manipulate the window’s size and position.

## 1.3.0

- Add `overrideStandardWindowButtonPosition` and `getStandardWindowButtonPosition` to `WindowManipulator` to allow getting and setting the position of standard window buttons.

## 1.2.0

- Fix typo in README.
- Add `isMainWindow` getter to WindowManipulator.

## 1.1.3

- Fix multiple `FlutterViewController`s being created, which prevented the apps from exiting properly on Flutter 3.10.

## 1.1.2

- Make macos_window_utils work without modifications to `MainFlutterWindow.swift`.

## 1.1.1

- Hotfix: Fix accidental breaking change in directory structure in 1.1.0.

## 1.1.0 (retracted)

- Add an abstract `NSWindowDelegate` that can be used to listen to events provided by [NSWindowDelegate](https://developer.apple.com/documentation/appkit/nswindowdelegate) such as window resizing, moving, exposing, and minimizing. The following methods are currently supported:
  -  Managing Sheets
     - `windowWillBeginSheet`
     - `windowDidEndSheet`
  -  Sizing Windows
     - `windowWillResize`
     - `windowDidResize`
     - `windowWillStartLiveResize`
     - `windowDidEndLiveResize`
  -  Minimizing Windows
     - `windowWillMiniaturize`
     - `windowDidMiniaturize`
     - `windowDidDeminiaturize`
  -  Zooming Window
     - `windowWillUseStandardFrame`
     - `windowShouldZoom`
  -  Managing Full-Screen Presentation
     - `windowWillEnterFullScreen`
     - `windowDidEnterFullScreen`
     - `windowWillExitFullScreen`
     - `windowDidExitFullScreen`
  -  Moving Windows
     - `windowWillMove`
     - `windowDidMove`
     - `windowDidChangeScreen`
     - `windowDidChangeScreenProfile`
     - `windowDidChangeBackingProperties`
  -  Closing Windows
     - `windowShouldClose`
     - `windowWillClose`
  -  Managing Key Status
     - `windowDidBecomeKey`
     - `windowDidResignKey`
  -  Managing Main Status
     - `windowDidBecomeMain`
     - `windowDidResignMain`
  -  Exposing Windows
     - `windowDidExpose`
  -  Managing Occlusion State
     - `windowDidChangeOcclusionState`
  -  Managing Presentation in Version Browsers
     - `windowWillEnterVersionBrowser`
     - `windowDidEnterVersionBrowser`
     - `windowWillExitVersionBrowser`
     - `windowDidExitVersionBrowser`
- Add an `NSAppPresentationOptions` class that allows the window's fullscreen presentation options to be modified.

## 1.0.2

- Fix incompatibility with Flutter 3.7.0.

## 1.0.1

- Add `setLevel` method.
- Add the following `order*` methods:
  - `orderOut`
  - `orderBack`
  - `orderFront`
  - `orderFrontRegardless`
- Add methods to modify the window's `styleMask` property.
- Improve documentation.

## 1.0.0+1

- Improve “Getting started” section in the project's readme.
- Improve documentation formatting.

## 1.0.0

- Initial version.
