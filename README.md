# React Native AsyncStorage Promise Handling Bug

This repository demonstrates a common error in React Native applications when working with AsyncStorage. The issue arises from incorrect handling of promises returned by AsyncStorage's getItem and similar methods.

## Problem

AsyncStorage methods return promises.  Attempting to access the stored value before the promise resolves results in undefined or incorrect data being used.

## Solution

The solution involves correctly handling the promise using `.then()` to access the data after it's been retrieved from AsyncStorage.

## How to reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run the app using your preferred React Native method (e.g., `npx react-native run-android`).
4. Observe the console output to see the error and then the correct output once the bug is fixed.