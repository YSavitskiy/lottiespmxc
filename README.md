# lottie



## Getting started

BUILD_LIBRARY_FOR_DISTRIBUTION=YES (in project settings)

xcodebuild archive -scheme "Lottie (iOS)" -archivePath ~/temp/Lottie-iOS.xcarchive -sdk iphoneos SKIP_INSTALL=NO
 1021  xcodebuild archive -scheme "Lottie (iOS)" -archivePath ~/temp/Lottie-simulator.xcarchive -sdk iphonesimulator SKIP_INSTALL=NO
 1022  xcodebuild -create-xcframework -framework ~/temp/Lottie-iOS.xcarchive/Products/Library/Frameworks/Lottie.framework  -framework ~/temp/Lottie-simulator.xcarchive/Products/Library/Frameworks/Lottie.framework -output ~/temp/Lottie.xcframework
