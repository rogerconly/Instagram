# Uncomment the next line to define a global platform for your project
# platform :ios, '9.0'

target 'Instagram' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!

  # Pods for Instagram
pod 'Appirater'

# Firebase
# Add the Firebase pod for Google Analytics

pod 'Firebase/Analytics'
pod 'Firebase/Auth'
pod 'Firebase/Database'
pod 'Firebase/Core'
pod 'Firebase/Firestore'
pod 'Firebase/Crashlytics'
pod 'Firebase/Storage'

end
post_install do |installer|
     installer.pods_project.targets.each do |target|
         target.build_configurations.each do |config|
             config.build_settings['DEBUG_INFORMATION_FORMAT'] = 'dwarf'
             config.build_settings.delete 'IPHONEOS_DEPLOYMENT_TARGET'
             config.build_settings['ONLY_ACTIVE_ARCH'] = 'YES'
         end
     end
  end
