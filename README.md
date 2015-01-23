# Bundle-Error

Bundle Error on Building App
============================

I had an error as below:-

ld: file not found: /Users/Username/Library/Developer/XCODE/DerivedData/AppNameRandomCode/Build/Products/Debug-iphoneos/Appname.app/Appname

clang: error: linker command failed with exit code 1 (use -v to see invocation)

File not found: /Users/Username/Library/Developer/XCODE/DerivedData/AppNameRandomCode/Build/Products/Debug-iphoneos/Appname.app/Appname

Solution
========
Remove all entries in the following paths and XCODE will regenerate them.

Xcode Target -> App       -> Build Settings -> Linking -> Bundle Loader -> Debug and Release

Xcode Target -> Apptests  -> Build Settings -> Linking -> Bundle Loader -> Debug and Release
