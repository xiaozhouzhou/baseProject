source 'https://github.com/CocoaPods/Specs.git'
platform :ios, ‘9.0’
use_frameworks!

def pods
pod 'Alamofire', '4.0.0'
pod 'SnapKit',  '3.0.0'
pod 'ObjectMapper', '2.2.1'
pod 'AlamofireObjectMapper', '4.0'
# pod 'RealmSwift'
pod 'SwiftyJSON','3.1.1'
pod 'SVProgressHUD', '2.0.3'
pod 'Reachability', '3.2'

pod 'ReflectionView', '1.2'
pod 'iCarousel', '1.8.3'
pod 'ALMoviePlayerController', '0.3.0'

end

target 'baseProject’ do
pods
end

target 'baseProjectTests' do
pods
#  pod 'Nimble', '~> 3.0.0'
#  pod 'Quick', '~> 0.9.3'
end

post_install do |installer|
installer.pods_project.targets.each do |target|
target.build_configurations.each do |config|
config.build_settings['ENABLE_BITCODE'] = 'NO'
config.build_settings['SWIFT_VERSION'] = '4.0'
end
end
end

