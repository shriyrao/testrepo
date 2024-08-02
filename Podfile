source 'https://github.com/CocoaPods/Specs.git'

platform :ios, '16.0'

inhibit_all_warnings!

target 'ofcwork' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  	pod 'Firebase/Core'

end

target 'ofcworkTests' do
  inherit! :search_paths
  # Pods for testing
end

target 'ofcworkUITests' do
  # Pods for testing
end

post_install do |installer|
   installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '5.0'
            config.build_settings['PROVISIONING_PROFILE_SPECIFIER'] = ' '
            config.build_settings['CODE_SIGNING_ALLOWED'] = 'NO'
            config.build_settings['CODE_SIGNING_REQUIRED'] = 'NO'
            config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '16.4'
        end
    end
end