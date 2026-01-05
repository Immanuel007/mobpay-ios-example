# Uncomment the next line to define a global platform for your project
platform:ios, '13.0'

target 'frameworktest' do
  # Comment the next line if you don't want to use dynamic frameworks
  use_frameworks!
  pod 'MobpayiOS', :git => 'https://github.com/Immanuel007/mobpay-ios-lib.git', :branch => 'master'
  pod 'Eureka', '~> 5.4'
  # Pods for frameworktest
  # pod 'MobpayiOS' , :path => '/Users/immanuelbarboi/Desktop/PROJECTS/mobpay-ios-lib'
  pod 'CocoaMQTT/WebSockets'
  

  target 'frameworktestTests' do
    inherit! :search_paths
    # Pods for testing
  end

  target 'frameworktestUITests' do
    inherit! :search_paths
    # Pods for testing
  end

end

post_install do |installer|
  installer.pods_project.targets.each do |target|
    target.build_configurations.each do |config|
      config.build_settings['IPHONEOS_DEPLOYMENT_TARGET'] = '13.0'
    end
  end
end
