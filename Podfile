# Uncomment the next line to define a global platform for your project
platform :ios, '9.0'


  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for EnglishCentralApp
workspace 'ECWorkspace'
project 'Frameworks/ECCoreKit/ECCoreKit.xcodeproj'
project 'Frameworks/ECTutorKit/ECTutorKit.xcodeproj'
project 'EnglishCentralApp/EnglishCentralApp.xcodeproj'

def import_corekit
    pod 'ECCoreKit', :path => "Frameworks/ECCoreKit"
end

def import_tutorkit
    pod 'ECTutorKit', :path => "Frameworks/ECTutorKit"
end

#def import_loginkit
#   pod 'ECLoginKit', :path => "Frameworks/ECLoginKit"
#end

target 'ECCoreKit' do
project 'Frameworks/ECCoreKit/ECCoreKit.xcodeproj'
# Pods for CoreKit
# ...
end

target 'ECTutorKit' do
project 'Frameworks/ECTutorKit/ECTutorKit.xcodeproj'
# Pods for TutorKit
# ...

# Relies on Core Kit
import_corekit
end

#target 'ECLoginKit' do
#project 'Frameworks/ECLoginKit/ECLoginKit.xcodeproj'
# Pods for CoreKit
# ...
#import_corekit
#end

target 'EnglishCentralApp' do
project 'EnglishCentralApp/EnglishCentralApp.xcodeproj'

# Pods for EnglishCentralApp
import_corekit
import_tutorkit
#import_loginkit
end

  target 'EnglishCentralAppTests' do
    inherit! :search_paths
    # Pods for testing
  end




