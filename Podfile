# Uncomment the next line to define a global platform for your project
platform :ios, '8.0'

target 'Instamojo' do
  # Comment the next line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!
  pod 'JuspaySafeBrowser', '~> 0.1.57'
end

post_install do |installer|
  installer.pods_project.build_configurations.each do |config|
    config.build_settings["EXCLUDED_ARCHS[sdk=iphonesimulator*]"] = "arm64"
  end
end
