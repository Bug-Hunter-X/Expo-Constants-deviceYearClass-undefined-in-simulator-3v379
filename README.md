# Expo Constants.deviceYearClass Undefined in Simulator

This repository demonstrates a bug and its solution related to the Expo Constants API.  Specifically, the `Constants.deviceYearClass` property returns `undefined` when the app is running within a simulator or emulator. This can lead to unexpected app behavior or crashes if not handled correctly.

## Bug Description
The `Constants.deviceYearClass` API call in Expo is expected to provide information about the device's year class. However, when running within a simulator or emulator, this property often returns `undefined`, resulting in runtime errors in applications that rely on this property.

## Solution
The solution involves adding a check to verify if `Constants.deviceYearClass` is defined before attempting to use it. If it's undefined, provide a default value or alternative behavior to prevent crashes.

## How to Reproduce
1. Clone this repository.
2. Run the app in a simulator or emulator (e.g., using Expo Go).
3. Observe the error message.
4. Modify the code as described in the solution section.
5. Run the app again to verify the fix.