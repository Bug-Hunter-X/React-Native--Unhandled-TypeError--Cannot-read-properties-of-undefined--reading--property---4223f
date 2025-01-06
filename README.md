# React Native: Unhandled TypeError: Cannot read properties of undefined (reading 'property')

This repository demonstrates a common React Native error: attempting to access a property of an undefined or null object.  The error typically arises when dealing with asynchronous data fetching or improperly initialized component state.

## Problem

The `bug.js` file shows how trying to access a property (`user.name`) of an object (`user`) that is initially null or undefined can cause the error.  This frequently occurs before asynchronous operations, like data fetching, have completed.

## Solution

The `bugSolution.js` file presents solutions to mitigate this issue.  The primary approach is to use optional chaining (`?.`) and nullish coalescing (`??`) to safely access properties.  Additional defensive programming techniques, such as conditional checks, are also shown.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install the dependencies.
4. Run `npx react-native run-android` or `npx react-native run-ios` to run the app (depending on your platform).
5. Observe the error and then the successful execution after applying the solution.