0.7.2 / 2013-11-6
=================
* Fixes critical issue #60 with NSContainer array subscripting, many thanks to @lhasiuk

0.7.1 / 2013-11-6
=================
* Fixing issue with Localytics not accepting booleans or integers, only strings.

0.7.0 / 2013-10-29
==================
* Changing debug to a class method
* Updating the internals so that reset method is unnecessary
* Fixing issue with cached settings
* Updating Mixpanel SDK to 2.0.4

0.6.6 / 2013-10-21
==================
* Updating Google Analytics SDK
* Fixing internal version number

0.6.5 / 2013-10-14
==================
* Updating Google Analytics, Chartbeat, Flurry and Amplitude SDKs
* Fixes common linker issue with old Google Analytics SDK

0.6.4 / 2013-10-2
=================
* Fixed identify to allow nil userId

0.6.3 / 2013-9-13
=================
* Fixing backgrounding crash issue
* Improving Countly logging
* Merging @cristianbica's pull request to fix literals syntax for iOS 5

0.6.2 / 2013-9-10
=================
* Queueing before settings cache is loaded the first time
* Flushing data to Segment.io on app close
* Using a custom store in NSUserDefaults to maintain user identity
* Prefixing internal classes to prevent compilation time conflicts
* Updating the Flurry and Mixpanel SDKs (iOS 7 support)
* Adding support for Mixpanel push notifications

0.5.3 / 2013-7-31
=================
* Adding comments, documentation and setup guide to Analytics.h
* Automatically handling app state hooks internally

0.5.2 / 2013-7-12
=================
* Adding Cocoapod podspec, with testing project
* Updating podspec to download from AWS rather than Github Raw

0.5.1 / 2013-7-11
=================
* Fixing build settings to include an armv7s slice, optimized for iPhone 5
* Moving version number to be visible externally from the library

0.5.0 / 2013-7-5
================
* Fixing compile and run-time bugs
* Adding a complete testing app, including for crash reporting tests
* Adding debug logging setting to reduce debug log output by default

0.4.0 / 2013-6-18
================
* Adding provider headers and binaries to project
* Restructuring project for Framework Builds vs CocoaPod builds

0.3.4 / 2013-6-16
================
* Removing Crittercism to avoid HockeySDK PLCrashReporter collisions
* Adding support for context.providers to ProviderManager

0.3.3 / 2013-6-5
================
* Implementing the reset method to help with debugging

0.3.2 / 2013-6-2
================
* Cleaning up NSLogs everywhere

0.3.1 / 2013-6-1
================
* Removing OS X Platform from podfile

0.3.0 / 2013-6-1
================
* Re-architecting the library to bundle providers
* Adding support for Amplitude
* Adding support for Bugsnag
* Adding support for Chartbeat
* Adding support for Countly
* Adding support for Crittercism
* Adding support for Flurry
* Library now downloads the provider settings from the Segment.io server

0.2.2 / 2013-4-24
=================
* Fixing timestamps to include millisecond precision


0.2.1 / 2013-4-16
=================
* Fixing initWithSecret method signature in header file

0.2.0 / 2013-4-16
=================
* Simplifying sessionId to behave the same on iOS 6 as on iOS 5 and OS X
* Fixing reset function to actually destroy userId and roll sessionId

0.1.1 / 2013-4-11
=================
* Added a getSessionId method

0.1.0 / 2013-4-11
=================
* Added a testing suite
* Added context variable, which includes device info and metadata for Segment.io
* Added alias method


0.0.5 / 2013-4-1
================
* Merged fix from @pkamb to fix types in logging statements.

0.0.4 / 2013-3-23
==================
* Removed UDID usage after Apple's announcement that it will no longer be accepted in the app store https://developer.apple.com/news/?id=3212013a
* Renamed repo to analytics-ios-osx

0.0.3 / 2013-3-13
==================
* Made timestamp more accurate
* Added max batch size

0.0.2 / 2013-3-12
==================
* Merged in numerous improvements from [tonyxiao](https://github.com/tonyxiao)
    * support for OSX apps
    * a shared dispatch queue and async flushing
    * removed JSON library dependency to use native JSON support
* Added enqueueAction to DRY things up
* Added an optional initialization method that reveals flushAt and flushAfter
* Added Cocoapods podspec

0.0.1 / 2013-3-9
==================
* Added working library for iOS
* Added README