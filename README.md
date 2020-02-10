# Project

## Setup

Steps to setup this project.

- Create project with Expo cli: `expo init <project>`
- Run project with expo: `npm start`
    This is a plain, non-native, react-native webapp
- Eject application to a bare application which generated iOS and Andriod native code: `expo eject`
- Download and install cocoapods for iOS dependencies.
- Run `pod install`
- Builing the app failed because of errors.
- Solution was to remove pods and do install again:
  - `pod deintegrate`
  - `pod install`
- In XCode build still failing
  - In settings, login with Apple Account of IPOS
  - select 'personal' team
  - Still build failing because need to select team in 'Signing and Capabilities'.
  - Select project -> select target (not project) -> 'Signing and Capabilities' -> select correct team

- Start iOS build: `npm run ios`

## Using

### iOS

Running in ios simulator: `npm run ios`
_Note: it can take a long time for 'Metro Bundler' to bundle index.js the first time which can cause the app to fail. Wait for bundler to finish and then refresh._

Any change in App.tsx is almost instantly reflected in simulator.

### Android

Have not tested Android yet

