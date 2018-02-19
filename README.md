### Capabilities
http://appium.io/docs/en/writing-running-appium/web/mobile-web/#android-mobile-web-automation

## Host setup
- Start selenium server on host as the hub
` composer selenium-server-hub`

## Running a browser on this box
### Steps - https://www.guru99.com/introduction-to-selenium-grid.html

- Open cmd window here and execute `composer selenium-node`

- On hub, reload page http://192.168.1.3:4444/grid/console to see multiple browsers are now defined

## Running on Android via USB
### Steps
- Open  cmd window and run `composer appium-android`
- On hub, reload page http://192.168.1.3:4444/grid/console to mobile
- From server hub, execute `composer testLocally`

## Running iOS via USB
### Steps
*  Verify the `uuid` in `android-config.json` - run `adb`
-  run `composer appium-android` once device is attached