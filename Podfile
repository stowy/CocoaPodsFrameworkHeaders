# Implicit sources are deprecated.
# This line adds the cocoapods as an explicit source

source 'https://github.com/CocoaPods/Specs.git'

# The version number specified here is the minimum
platform :ios, '9.0'

# ignore all warnings from all pods
inhibit_all_warnings!

project 'SampleApp.xcodeproj'

abstract_target :pods do
    pod 'Firebase/Core'
    pod 'Firebase/RemoteConfig'
    pod 'Realm', '2.1.1'
    
    target :SampleFramework do

    end

    target :SampleApp do
        inherit! :search_paths
    end
end
