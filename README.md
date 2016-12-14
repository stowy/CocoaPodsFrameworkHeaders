# CocoaPodsFrameworkHeaders
A sample iOS project showing cocoapod frameworks search paths not inherited issue

To replicate the issue, run pod install and try to build the app. You will see that the Realm dependency is found correctly, however the Firebase dependency is not because it is distributed as a framework (although we are not using the `use_frameworks!` cocoapods flag), and the framework search paths from the `SampleFramework` are not copied to `SampleApp`, despite having specified `inherit! :search_paths` in the Podfile.
