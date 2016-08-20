# Uncomment this line to define a global platform for your project
# platform :ios, '9.0'

target 'MsgNotFree' do
  # Comment this line if you're not using Swift and don't want to use dynamic frameworks
  use_frameworks!

  # Pods for MsgNotFree
  pod 'Koloda', :git => 'git@github.com:Yalantis/Koloda.git'

end

post_install do |installer|
  `find Pods -regex 'Pods/pop.*\\.h' -print0 | xargs -0 sed -i '' 's/\\(<\\)pop\\/\\(.*\\)\\(>\\)/\\"\\2\\"/'`
end
