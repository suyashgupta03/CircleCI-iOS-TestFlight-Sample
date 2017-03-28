#source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'
use_frameworks!


target 'CircleCI-Sample' do
pod "AFNetworking", "~> 2.5.0"
end

target 'CircleCI-SampleTests' do
pod "AFNetworking", "~> 2.5.0"
end
  
post_install do |installer|
    installer.pods_project.targets.each do |target|
        target.build_configurations.each do |config|
            config.build_settings['SWIFT_VERSION'] = '2.3'
        end
    end
end
