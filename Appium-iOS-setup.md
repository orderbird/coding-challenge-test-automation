# Appium iOS setup:

1. brew install libimobiledevice

2. brew install ios-deploy

3. brew install carthage

4. Download latest Appium desktop version

5. cd to wda (/Applications/Appium.app/Contents/Resources/app/node_modules/appium/node_modules/appium-webdriveragent)

6. mkdir -p Resources/WebDriverAgent.bundle
    ./Scripts/bootstrap.sh -d

7. Open simulators in Xcode and select simulator and copy iOS version, model (device name), udid (identifier)

8. being in wda folder -> open WebDriverAgent.xcodeproj file in Xcode

9. Open Xcode -> Preferences -> Accounts -> Click on (+) -> Apple ID -> Continue -> Type Apple ID credentials -> Next -> Select just added Apple ID -> Click Manage Certificates -> Click on (+) -> Apple Development -> Wait new cert. will be added in the table -> Click Done -> Close window pop up

10. Click on folder top left corner -> select root parent object WebDriverAgent

11. For each Targets items: Click on target item -> Click on Build Settings on the right -> Select Basic below -> Search for Product Bundle Identifier -> add at then end of Bundle Identifier smth like .{AppName_random_digits}

12. For each Targets items: Click on Signing and Capabilities -> Check 'Automatically manage signing' and select team profile (added in step 9)

13. Click on folder top left corner -> select root parent object WebDriverAgent; At the top (left from device selection click on project target and select WebDriverAgentRunner)

14. Select simulator from step 7 on the right to target project selection

15. Click |> Play button (if fail for some reason, try to enable "Validate Workspace" in Build Settings for each Project Target)

16. On real devices -> repeat step 13 and 14 (selecting real device) and click Play (step 15) - first attempt will fail -> Go to Settings -> General on real device -> open device management -> Click on webdriver agent app -> click trust. Repeat step 15 again - should be success

17. terminal: -> "   wda   " and run this command "     xcodebuild -project WebDriverAgent.xcodeproj -scheme WebDriverAgentRunner -destination 'id=<udid>' test     "

http://appium.io/docs/en/drivers/ios-xcuitest-real-devices/

Appium Pro: How To Test On Real iOS Devices With Appium, Part 1
Connecting an iOS device to your computer and setting it up to be automated by Appium for the first time can be challenging; follow along with this post to get all the details you need for a first-time installation

https://appiumpro.com/editions/40-how-to-test-on-real-ios-devices-with-appium-part-1

Appium Pro: How To Test Real iOS Devices With Appium, Part 2
This is the second part in a full tutorial on getting real iOS devices to work with Appium. Assuming everything is installed and set up correctly, this is what you need to do to make Appium work its magic.

https://appiumpro.com/editions/41-how-to-test-real-ios-devices-with-appium-part-2