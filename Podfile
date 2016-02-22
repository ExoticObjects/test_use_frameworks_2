
source 'https://github.com/ExoticObjects/eo-attributed-markdown-podspec.git' # Private repo because these guys can't submit their repo to cocoapods for some reason...
source 'https://github.com/CocoaPods/Specs.git' 

platform :ios, '9.0'
use_frameworks!

plugin 'cocoapods-rome'

def common_pods_for_target

  # Use this to build project from source files (.h ,.m)
  # pod 'test_pod_2', :git => 'https://github.com/ExoticObjects/test_pod_2.git'

    pod 'test_pod_2', :path => '../test_pod_2'

  # Use this to build project from a framework made from that pod with Cocoapods packager
  # pod 'test_pod_2', :git => 'https://github.com/ExoticObjects/test_pod_2_framework.git'
end

# post_install do |installer|

#   files = Dir.glob("*.xcodeproj")
#   proj_file = files[0]
#   app_project = Xcodeproj::Project.open(proj_file);

#   app_project.native_targets.each do |target| #Set allow non modular includes on app target to 'yes'

#     # puts 'native_targets: ' + target.inspect
#     target.build_configurations.each do |config|
#       config.build_settings['CLANG_ALLOW_NON_MODULAR_INCLUDES_IN_FRAMEWORK_MODULES'] = 'YES'
#       # puts 'MAIN target.config.build_settings.name: ' + config.name + ', settings: ' + config.build_settings.inspect
#     end
#   end

#   app_project.save # Can't forget this or nothing will happen! (See https://github.com/CocoaPods/CocoaPods/issues/4618)

#   installer.pods_project.build_configuration_list.build_configurations.each do |configuration| #Set allow non modular includes on POD target to 'yes'
#     configuration.build_settings['CLANG_ALLOW_NON_MODULAR_INCLUDES_IN_FRAMEWORK_MODULES'] = 'YES'
#     # puts 'POD target.config.build_settings.name: ' + configuration.name + ', settings: ' + configuration.build_settings.inspect
#   end
# end


target :test_use_frameworks_2 do
  common_pods_for_target
end

target :test_use_frameworks_2UITests do
  common_pods_for_target
end






