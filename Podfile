  platform :ios, '9.0'
  use_frameworks!

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

  target 'ECCoreKit' do
    project 'Frameworks/ECCoreKit/ECCoreKit.xcodeproj'

     # Pods for CoreKit
     import_corekit
  end

  target 'ECTutorKit' do
    project 'Frameworks/ECTutorKit/ECTutorKit.xcodeproj'

    # Pods for TutorKit
    import_tutorkit

    # local pods
    import_corekit
  end

  target 'EnglishCentralApp' do
    project 'EnglishCentralApp/EnglishCentralApp.xcodeproj'

    # Pods for EnglishCentralApp

    # Local pods
    import_corekit
    import_tutorkit
  end

  target 'EnglishCentralAppTests' do
    inherit! :search_paths
    # Pods for testing
  end




