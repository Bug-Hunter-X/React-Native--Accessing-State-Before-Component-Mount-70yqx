# React Native: Accessing State Before Component Mount

This repository demonstrates a common error in React Native: attempting to access a component's state before the component has mounted.  The `Bug.js` file showcases the error, while `BugSolution.js` provides the corrected code.

## Problem

Asynchronously fetching data within `componentDidMount` and immediately attempting to access and utilize that data often leads to undefined state values, causing crashes or incorrect display behavior.

## Solution

The solution involves ensuring that state updates are handled after the component is fully mounted. This can be achieved by conditionally rendering content or utilizing the state values within the effect's callback function after the state has been updated. 

## How to run

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `npm install`.
4. Run `npx react-native run-android` or `npx react-native run-ios` depending on your platform.