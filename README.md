# Handling Null or Undefined Values in React Native

This repository demonstrates a common error in React Native applications where attempting to access properties of null or undefined objects can cause crashes.  The example shows how to effectively handle these situations using optional chaining and the nullish coalescing operator.

## The Problem

When dealing with asynchronous data fetching, components might try to render before the data is fully loaded, resulting in attempts to access properties of `null` or `undefined` objects. This leads to runtime errors.

## The Solution

The recommended approach is to utilize optional chaining (`?.`) and the nullish coalescing operator (`??`) to safely access properties. Optional chaining prevents crashes if the object or a property in the chain is nullish.  The nullish coalescing operator provides a default value if the property is null or undefined.

## How to Run

1. Clone the repository.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `npx react-native run-android` or `npx react-native run-ios`.