# Unhandled JS Exception: Cannot read properties of undefined (reading '...') in React Native

This repository demonstrates a common error in React Native applications: "Unhandled JS Exception: Cannot read properties of undefined (reading '...')." This occurs when attempting to access a property of an object that is currently undefined.

The `bug.js` file shows the problematic code, and `bugSolution.js` presents the corrected version.

## Bug
The bug arises from trying to access a property of an object before it's properly assigned a value.  Often, this is due to asynchronous operations like fetching data from an API that haven't completed.

## Solution
The solution involves checking for the existence of the property (or the object itself) before attempting to access it.  Conditional rendering using optional chaining (?.) is a concise and effective approach.