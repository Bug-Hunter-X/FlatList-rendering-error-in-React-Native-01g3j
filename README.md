# React Native FlatList Rendering Error

This repository demonstrates a common error encountered when using FlatList in React Native: attempting to render a property of an undefined item.  The issue arises when the data being passed to FlatList is not properly formatted or not yet loaded.

## Problem

The provided `bug.js` file contains a component that fetches data from an API.  If the API call fails or returns unexpected data,  the component attempts to access `item.name` which will result in the error:  'undefined' is not an object (evaluating 'item.name').

## Solution

The `bugSolution.js` file offers a solution by implementing proper error handling and data validation.  It checks for `null` or `undefined` values before accessing properties, preventing the error.

## How to reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run the application.
4. Observe the error if the API request fails or the data structure is invalid.   You can simulate this by commenting out the fetch call in `bug.js`.

## How to fix

Review the `bugSolution.js` for a robust solution that includes thorough error handling and data validation before rendering.
