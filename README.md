# hc-hotels-ios-sdk
Hotel Price Freeze iOS SDK

## Purpose
This is presently a placeholder project. The intent is to utilize this branch and [this public repo](https://github.com/robomex/TestSDK) together. This repo contains the source which is compiled to an `.xcframework`. That `.xcframework` is then dropped into the public repo and committed to serve as a new release for the CocoaPods source.

## Instructions for updating the CocoaPod derived from this source code
1. In Terminal navigate to this project's root folder
2. Delete any existing `archives` or `HCHotels.xcframework` folders
3. In Terminal run `sh build_xcframework.sh` to build this project
4. Delete the existing `HCHotels.xcframework` folder in the [public CocoaPod repo](https://github.com/robomex/TestSDK)
5. Drag the `HCHotels.xcframework` created by `build_xcframework.sh` to the root of the public repo
6. Update the public repo's `.podspec` version
7. Commit changes from last two steps to the public repo
8. Create a new release for the public repo
9. Update any Podfiles that request a specific tag of the `HCHotels-Testing` pod (e.g. `:tag => '0.0.2'`) to the latest release

### Instructions Note
The instructions above are at their most basic and unstreamlined. There are certainly steps to cut out, simplifications to be made, and hopefully automation to be implemented. This is a starting point.

## Usage
This is a placeholder version of the SDK; there are two things you can do with this placeholder:
### Initialize an instance of the HCHotels class
`let sdk = HCHotels()`
### Print "Hello, World!" to the console
`sdk.helloWorld()`
