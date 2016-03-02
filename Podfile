source 'https://github.com/CocoaPods/Specs.git' 

platform :ios, '9.0'
use_frameworks!

plugin 'cocoapods-rome'

def common_pods_for_target
   pod 'test_pod_2', :git => 'https://github.com/ExoticObjects/test_pod_2.git'
end

target :test_use_frameworks_2 do
  common_pods_for_target
end

target :test_use_frameworks_2UITests do
  common_pods_for_target
end
