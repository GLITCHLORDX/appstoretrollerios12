iOS 12.5.8 rootful fix notes:
- Removed THEOS_PACKAGE_SCHEME = rootless. iOS 12 jailbreaks are normally rootful.
- Changed target to iphone:clang:12.4:12.0.
- Kept ARCHS = arm64 for iPhone 6.
- Added preferenceloader dependency.
- Added /Library/PreferenceLoader/Preferences/appstoretrollerPrefs.plist so the Settings page appears.
- Build with: make clean package FINALPACKAGE=1
